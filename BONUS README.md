BONUS README

I created multiple networks, all networks have different ip addresses with multiple terminals and two servers on alternate networks.
All connected devices can talk to each other and the network routing protocol is OSPF.

User Networks 192.168.1.0, 192.168.2.0, 192.168.4.0 and 192.168.4.0.all network terminals with net mask of 255.255.255.0 or /24

Server networks 192.168.20.0 and 192.168.30.0 both with net mask of 255.255.255.252 or /30

All serial connections between routers are on the 10.0.0.0 network as follows:

| Network Address | Net Mask | IP Range |
|-----------------|----------------------|----------------------------------------
10.10.0.0        | 255.255.255.252 | .0 to .3 
10.10.1.0        | 255.255.255.252 | .0 to .3 
10.10.2.0        | 255.255.255.252 | .0 to .3 
10.10.4.0        | 255.255.255.252 | .0 to .3 
10.10.10.0       | 255.255.255.252 | .0 to .3 
10.10.11.0       | 255.255.255.252 | .0 to .3 
10.10.12.0       | 255.255.255.252 | .0 to .3 
10.10.13.0       | 255.255.255.252 | .0 to .3 
10.10.20.0       | 255.255.255.252 | .0 to .3 
10.10.30.0       | 255.255.255.252 | .0 to .3 

All network addresses have a 255.255.255.252 or /30 mask as this is the most efficient use of ip addresses.
The .0 is the network address
The .1 and .2 are the serialport addresses
The .3 address is tthe broadcast address for that network.
