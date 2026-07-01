
Answers for DEEP-IN-NET

Ex 1
1) Havnig a network mask of /24 or 255.255.255.0 you have 256 ip addresses at your disposal.
the first and last would not be used as 255.255.255.0 would be used as the next 
network address and 255.255.255.255 is the final broadcast address leaving 
you with 254 useable addresses.

2) Having a network mask of /29 or 255.255.255.248 you have only 8 usable addresses at your
disposal. so 192.168.13.81 would be your network address and 192.168.13.88 would
be your broadcast address leaving you 6 usable addresses. This range would be
192.168.13.82 to 192.168.13.87

3) Having a network mask of /29 or 255.255.255.248 you have only 8 usable addresses at your
so 255.255.255.248 would be your network address and 255.255.255.255 would
be your broadcast address leaving you 6 usable addresses. This range would be
192.168.13.249 to 192.168.13.254

An RJ45 cable comes in two forms a straight through and a crossover variety.
A crossover cable is used to connect two computers together whereas a straight through cable would
be used to connect computers to hubs or switches.

Ex2
Hubs work at layer 1 (The Physical L:ayer) of the OSI model. They take in a signal and broadcst it out of all 
ports and the receiving maachine decides wether to retain or drop the data. The use of hubs has largely dissappeared 
from networks although there are a few cases where they are still used 
A Switch functions at layer 2 (Data Link Layer of the OSI model. It learns mac addresses form connected devices so it 
can either send the data tol the correct receipient orto the next device in the journey.

Ex 3
Define a 'server' and it's purpose in networking.
A servers purpose is to provide differing services depending upon it's configuration.
it receives requests from users for it's differing services, these can be either data,
servicees or resoirces.

Explain DHCP and how it operates in a network.
DHCP is a network protocol that dynamically assigns network configuration data to 
devices connected to its network.
DHCP works by the following four step process:

|---------------|--------------------------------------------------------------------------------------------------------|
|Discover:	    	|The client sends a DHCP Discover message to find available servers.
|---------------|--------------------------------------------------------------------------------------------------------|
|Offer:	    	  	|A DHCP server responds with a DHCP Offer, proposing an available IP address and configuration settings.
|Request:     		|The client sends a DHCP Request indicating that it wants to use the offered address.
|Acknowledge:	  |The server sends a DHCP Acknowledgment (ACK) confirming the assignment.



Define DNS and its roles in network communications.

DNS is a distributed naming system that translates readable names into numerical 
addresses. The role of DNS is to allow devices to communicate with each other using domain names. 
it works like the internets phone book.

What is the purpose of HTTP and how is it used in networking.

HTTP is the foundation of data communication on the world wide web. It defines how messages are
formatted between client and server.
HTTP works by using a client-server model over a network.
HTTP allopws browsers and servers to communicate 
and deliver web content over a network.

Explain the difference between HTTP and HTTPS.
They are both protocols for the transfer of data between client and server, although HTTPS is encrypted whereas HTTP sends data in plain text.
 
What is the purpose of FTP and how it operates in network communication.
FTP is a standard network protocol used to transfer data between clients and servers across networks.
It works by using a control channel for commands and a separate data channel for file transfers, allowing
users to upload, download, and manage files remotely.

Define TCP and UDP communication and differentiate between them.
TCP and UDP are two core transport-layer protocols used to send data across networks. they provide different
approaches to communication depending whether reliability or speed is more important.


|Feature				  |TCP						  |UDP
| ----------------------- |---------------------------|-----------------------|
|Reliability		   	  |Connection-orientated	  |Connectionless
|Error Checking		   	  |Reliable					  |Unreliable
|Packet Ordering		  |Guaranteed				  |Not guaranteed
|Retransmission			  |Yes						  |No
|Speed					  |Slower					  |Faster
|Overhead				  |Higher					  |Lower
|Typical Uses			  |Web, Email, File Transfer  |Streaming, Gaming, DNS


Identify the OSI model layer where TCP and UDP operate
Both TCP and UDP work at layer 4 of the OSI model, this is the transport layer.

Define a port in networking and it's function.
A port in networking is a logical communication endpoint used by a device to identify a specific application or service that is sending or receiving data.

Identify the port and OSI model layer for each protocol used.


|Port no		|Protocol			|OSI Layers	
|---------------|-------------------|-------------------------|
|20				|FTP Data			|4 and 7	
|21				|FTP Control		|4 and 7
|22				|SSH				|4 and 7
|23				|Telnet				|4 and 7	
|25				|SMTP				|4 and 7
|53				|DNS				|4 and 7
|67,68			|DHCP				|4 for TCP,UPD 7 for DNS
|69				|TFTP				|4 and 7		
|80				|HTTP				|4 and 7		
|110			|POP3				|4 and 7			
|161			|SNMP				|4 and 7		
|443			|HTTPS,SSL,TLS		|4,6 and 7
|---------------|-------------------|-------------------------|

they all use layer 7 so as the user has an onscreen response to the protocls use.
for port 443 layer 6 6is used for encryption and decryption.

What are the different types of DNS records.

| Record Type | Description |
|-----------------------|------------------------------------------------------------------------------------------------------------------------------------|
|A					                	|Maps a domain to an IPv4 address.
|AAAA				              	|Maps a domain to an IPv6 address.
|CNAME				             	|Aliases one domain name to another.
|MX					               	|Directs email to mail servers.
|NS					               	|Specifies the authoritative nameserver for a domain.
|SOA				               	|Contains administrative information about the domain, like the primary nameserver and zone update settings.
|TXT	                   |Stores text information, often used for verification.
|SRV	                   |Specifies a service location for certain services, like servers handling VoIP.
|PTR	                   |Maps an IP address to a domain name for reverse DNS lookups.
|AFSDB					             |Specifies the location of Andrew File System (AFS) cells.
|ATMA				              	|Maps a domain name to an ATM address used for ATM networks.
|CAA	                   |Specifies which certificate authorities (CAs) are allowed to issue certificates for a domain.
|CERT				       	       |Stores certificates and certificate-related information, such as public keys.
|DHCID				             	|Used in DHCP to associate DNS names with dynamically assigned IP addresses.
|DNAME				             	|Provides redirection of a subtree of the DNS namespace to another domain.
|DNSKEY				            	|Contains public keys used to verify DNSSEC signatures.
|DS					               	|Used in DNSSEC to identify a DNSKEY record in the delegated zone.
|HINFO				             	|Provides information about the hardware and operating system used by a host.
|ISDN					              |Stores ISDN addresses associated with a domain name.
|MB, MG, MINFO, MR	    	|Legacy records related to mailbox information, with specific uses for mapping and informational purposes.
|NAPTR			  	           	|Used for Uniform Resource Identifier (URI) and E.164 Number Mapping (ENUM) applications to define rules for rewriting domain names.
|NSAP		                 |Maps a domain name to an NSAP address used in OSI networks.
|NSEC					              |Used in DNSSEC to prove the non-existence of a DNS record by listing the next record in the zone.
|NSEC3					             |An enhanced version of NSEC for DNSSEC that includes hashed domain names to prevent enumeration.
|NSEC3PARAM				         |Stores parameters for NSEC3 records, including hashing algorithms and iterations.
|RP						               |Provides information about the person responsible for a domain, including contact details.
|RRSIG					             |Contains a cryptographic signature used to verify DNSSEC-signed data.
|RT						               |Specifies a route through a specific intermediate host, used for non-IP networks.
|TLSA					              |Links a domain name with a TLS certificate, used in DNS-based Authentication of Named Entities (DANE).
|X25				               	|Stores an X.25 network address used in older packet-switched networks.



Ex 4
What is a "router" and what is it's role?
A router in a networking device that connects different networks together.
It acts as a traffic director sending packets to the correct destination.
Differentiate betwqeen a router and a switch?
A router is used to send packets between networks whereas i switch works with a netork.
Identify the OSI model layer where a router operates?
A router works at layer 3 of the OSI model by directing packets using their starting IP address
and either their destination IP address or the address of the next hop router, whereas a switch
works at layer 2 of the OSI model and directs traffic by learninig mac address of attached devices.
Understand the term"defaukt gateway".
A default gateway is the device used to access other networks or the internet.

Ex 6
What is a routing table and explain its role in routing network traffic.
The routing table is a list of directly connected and next hop routers 
and networks. It is governed by a set of rules governing hops, subnet masks
and gateways to direct trafic to its destination

