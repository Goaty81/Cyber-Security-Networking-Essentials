<ins>Subnetting</ins>

A subnet is usually equivalent to one or more network segments connected to one router. Network segments are the physical connection and subnets or the logical connections.

Each subnet has its own IP address range and its connected to the internet via a router. Additionally, the router may have a firewall between network segments to filter and enforce security policies on the traffic that passes between them.

Below is a Example of a subnet split into two network segments:

<img width="463" height="662" alt="image" src="https://github.com/user-attachments/assets/fd617398-3cca-4f0f-b7a0-4292f1e7b385" />

There are three different types of subnet classes:

Class A - The biggest subnet class, this will be shown as 255.0.0.0 or /8. Meaning it is capable of have 16 million hosts.

Class B - This will be shown as 255.255.0.0 or /16, Capable of having 65,534 hosts and is often used for enterprises and campus networks.

Class C - The smallest class which will be shown as 255.255.255.0 or /24. This is capable of holding up to 254 hosts and is commonly used in homes or small businesses. The example above has two IPs with this attached.

Subnets will allow you to communicate with each other isolated in your own subnet environment. For example if you would like to know if someone else in your subnet is online you would simply send a ARP Request to the subnet. 

Without subnets you will come into quite alot of problems like :

  - All departments would have the same network
  - Only 80 IP address could be used leaving 176 unused
  - More chance of broadcast traffic flooding the network
  - Devices from other departments can easily access each other

With subnets you could:

  - Divide the network into three smaller subnets
  - Each department receives only the IP they need
  - Traffic remains within each subnet, improving performance
  - Departments are logically separated therefore improving security
  - IP addresses are used efficiently therefore have room for growth

