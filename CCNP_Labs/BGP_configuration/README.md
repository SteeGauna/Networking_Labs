# BGP Configuration

## Suva Office
 - The Suva Office comprises of a network that includes 2x 2911 Cisco routers, 2x 2960 Cisco switches and 3x PCs.
#### The configurations are as follows
 - Configured a 10.0.0.0/24 network within the Suva LAN and configured static IP addresses on the PCs
 - Configured HSRP between the 2 routers with R1 having the higher priority. I've tested the configuration by shutting down the link to R1 and R2 successfully became the active router. As both routers have uplinks to the "Provider Edge Router"
  and R1 is configured as the preferred router in the LAN, I have configured tracking on R1 to track the uplink its gigabitethernet 0/1 interface that if it goes down, it will decrement its HSRP priority by 10 so that it allows R2 to use 
  preemption to take the active role.
 - I have configured OSPF between the Suva LAN routers and the Provider edge router.
 - Configured default routes from the LAN routers using the corresponding Provider edge router interface as the gateway
 - I also configure a summary route on the Provider edge router to route traffic destined for the Suva LAN
 - On the Provider Edge router I redistributed all static and OSPF routes onto BGP so that it is reachable on the "WAN"
 - I can confirm that that all Suva LAN devices have full connectivity to each other

## Navua Office
 - Navua Office took more of a simpler approach as I just wanted to replicate remote small offices across the WAN, as the focus of this LAB was the BGP configurations between the routers
#### The configurations are as follows
 - Configured a 172.16.0.0/24 network within the LAN and configured a static IP address on the PC
 - I configured a default route on the Navua LAN router using the corresponding Provider edge router interface as the gateway
 - Configured a summary route on the Provider edge router to route traffic destined for the Navua LAN
 - Redistributed the static summary route onto BGP so that the Navua LAN is reachable on the "WAN"

## Nadi Office
 - Just like the Navua Office, I configured the Nadi office to be more of a simpler network
#### The configurations are as follows
 - Configured a 192.168.0.0/24 network on the LAN
 - Configured a default route on the Nadi LAN router using the Provider edge router internal facing interface as the gateway
 - Configured a summary route on the Provider edge router to route traffice destined for the Nadi LAN
 - Redistributed the static route to BGP to so that the Nadi LAN is reachable on the "WAN"

## BGP Configuration
 - I configured a total of 6 routers to replicate the idea of service provider routers. I configured BGP on all routers using different AS numbers for every configuration. This means that all routers are eBGP neighbors. I configured the networks
 between the routers in ascending order just to help in memorizing the networks.
 - I can confirm that all BGP routers are able to communicate with each other
 - I have designed the network in a way where the remote sites have two routes across the BGP routers
 - I conducted a tracert between the Suva and the Nadi office and the traffic was following the shortest path (PC->R1->Vodafone1->Vodafone2->Telecom2->Telecom1->R4->PC4). As I shut down the link between Vodafone2 and Telecom2, the traffic automatically
 followed the alternate path(R1->Vodafone1->Vodafone2->Digicel1->Digicel2->Telecom1->R4
 - After all the configurations, I can confirm that all sites have achieved inter-connectivity.

 "Appreciate feedback if there are any"
