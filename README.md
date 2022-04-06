# Two-Interconnected-Networks

![Topology](https://user-images.githubusercontent.com/98745874/162010865-34952f2e-ecd4-45aa-a5e0-9f3e6a62b972.PNG)

Networks: 'PDL' and 'ANGRA' connected to each other through an encrypted tunnel.

Both networks will be able to ping each other.

Both networks will be able to make VOIP connections to each other.

'PDL' will be able to access the 'ANGRA' WEB Server and 'ANGRA' will be able to access the HTTP WEB SERVER and HTTPS WEB SERVER of 'PDL'.

PDL:
1. DHCP and VOIP;
2. LACP Protocol between 2 switches with 4 cables;
3. OSPF Protocol;
4. VTP (VLan Trunk Protocol);
5. STP (Spanning Tree Protocol);
6. HSRP (Hot Standby Router Protocol);
7. Web Server;
8. ACL.

All traffic goes through 'PDL2', when 'PDL2' is down, traffic goes through 'PDL1'.

When 'PDL1' is down, the equipment continues to connect to the internet through the interface (1.0.0.8/30).

ANGRA:
1. 'DHCP and VOIP Helper' between ANGRA1 <-> ANGRA2;
2. WireLess Router Configuration;
3. EIGRP Protocol;
4. Web Server;
5. ACL.

Tunnel 100:
1. Encrypted;
2. RIP Protocol.
