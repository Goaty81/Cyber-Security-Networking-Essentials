<ins>IPv4</ins>

So first of all i want to talk about what does IPv4 actually stand for?

Its simply Internet Protocol version 4, meaning that its the 4th iteration of the IP protocol. 

So what happened to IPV1, 2 and 3?

These IP versions were not released to the public and was just experiments into creating the success of IPv4. So if (like me) you was wondering why it went straight to IPv4, now you know why!

<ins>What is an IPv4 address and how does it work?</ins>

IPv4 addresses are numerical identifiers exactly like a door number only instead of doors its devices assigned to networks. Its made up of two Components: Host addresses and network addresses.
Network address is the main IP address with the Host address which are devices are attached to. 
We divide the host address apart through what we call Subnets (i have a document on Sub-netting) by using a net mask which defines the number of hosts connected to the network.

IPv4 addresses are 32-bits long, expressed through 4 decimal numbers separated by periods which is called an Octet.

<img width="738" height="387" alt="image" src="https://github.com/user-attachments/assets/80b20ec5-80ce-40c2-b2c1-f4b441a82ab5" />

Each of the octets can range from 0 to 255 which gives 4.3billion unique addresses.

The way IPv4 forwards data is through routers, when a device in the network sends data to another device it first of all has to be broken down into smaller packets, each containing the sources and destinations address.
Routers will examine the destinations IP address and uses its routing table to determine the appropriate path to send the packets of data. Then the packets are forwarded to the destination router which then the logical mechanics of the OSI table goes in reverse! (from layer 1 through 7)
