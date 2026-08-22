<ins>Subnetting</ins>

In this document i will briefly discuss subnetting.

A subnet is usually equivilant to one or more network segments connected to one router. Network segments are the physical connection and subnets or the logical connections.

Each subnet has its own IP address range and its connected to the internet via a router. Additionally, the router may have a firewall between network segments to filter and enforce security policies on the traffic that passes between them.

Below is a Example of a subnet split into two network segments:

<img width="463" height="662" alt="image" src="https://github.com/user-attachments/assets/fb2df15e-f043-43d1-ab24-c13d380d71bc" />


There are three different types of subnet classes:

Class A - The biggest subnet class, this will be shown as 255.0.0.0 or /8. Meaning it is capable of have 16 million hosts.

Class B - This will be shown as 255.255.0.0 or /16, Capable of having 65,534 hosts and is often used for enterprises and campus networks.

Class C - The smallest class which will be shown as 255.255.255.0 or /24. This is capable of holding up to 254 hosts and is commonly used in homes or small businesses. The example above has two IPs with this attached.

Subnets will allow you to communicate with each other isolated in your own subnet enviroment. For example if you would like to know if someone else in your subnet is online you would simply send a ARP Request to the subnet. 

However if your target is out of your subnet you will have to use what we call "Active network scanning" which i will cover on another topic.
