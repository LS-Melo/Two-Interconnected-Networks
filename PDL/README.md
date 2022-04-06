![PDL-SIDE](https://user-images.githubusercontent.com/98745874/162018107-f9c1bbcb-308e-4b34-a17f-6d26996a7e6b.PNG)

All traffic sent out of the network, passes through PDL2 (when PDL2 is down, it passes through PDL1)

All traffic coming off the network, goes through PDL1 and is redirected to SWITCH 5 and then to the equipment.

Each device receives IP and telephony number via DHCP

All packets to port 80 are redirected to the 'V40-HTTP' web server

All packets to port 443 are redirected to the 'HTTPS' web server
