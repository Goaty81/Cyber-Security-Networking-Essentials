<ins> Network Address Translation </ins>

In my document subnetting we talked about how we will control traffic inside the network by separating the network into groups, in this document we will be talking about how those groups talk to the external internet however only working with one IP address.

One popular way we do this is through Network Address Translation (NAT), This allows multiple devices to work off of one IP address. For instance, A desktop and a laptop in a household are connected to the same router however having 2 devices mean 2 IP addresses correct? Having NAT enabled will make the routers outbound traffic whether it be from the desktop or laptop it will have the same IP.

<ins>How NAT works</ins>

So you'll see on each device it will have its own private IP address, this will stay the same and wont change. The one that can be changed is the public IP address and that’s the one the router will change so all of the devices are using one IP address.
What will happen is the device will try to send out data through the router from its private IP however when it gets to the router, the router will change it to the public IP address and send it to its destination, once it reaches its destination and receives data to go back to the origin device it will check the data and send it back to the device that correlates with the private IP address it was sent from.

<img width="1024" height="768" alt="image" src="https://github.com/user-attachments/assets/2f81c7bc-3946-4f48-8f43-e7c1458a1ad5" />

What the router does is hides the private IP addresses which acts as another layer of security!

<ins>Why is NAT important in Cyber Security?</ins>

NAT can provide a measure of security by hiding the private IP addresses. This can be useful for preventing attacks to a specific IP address or making the devices within the network vulnerable directly from the outside internet. It can also help in negating the fact of internal devices access unwanted or malicious sites. Not by website filtering (which is what a firewall does) but by blocking inbound traffic.

It also makes it easier to administrate due to it cutting the number of IP addresses needed for one network. This benefits large organisations due to the fact its less attack surface for the attackers and reduce the amount of time and effort required for if an incident was to occur.

<ins>Three types of Network Address Translation</ins>

The three NAT types are:

  1. Static NAT - This type of NAT is where every private IP address is mapped to a unique global IP address, When outgoing traffic arrives at the router, the router will change the destination IP address with the mapped global IP, When the data returns it will be reverted back to the source IP address and sent to the private IP.

  2. Dynamic NAT - In Dynamic NAT the source IPs are mapped to a pool of global IPs. This is where instead on mapping it to one global IP, its got a pool of them to choose from. The router remember which source IP used the global IP and then data being sent back to the inbound data for the global IP goes through the router and then back to the private IP.

  3. Port Address Translation (PAT) - PAT is a type of dynamic NAT, it maps multiple IP addresses to one global IP address via port numbers, Meaning when a computer connects to the internet, the router assigns it a port number then attaches it to the devices private IP, which gives it a unique IP. When multiple devices connect to the same router, the router will just assign them with different port numbers.
