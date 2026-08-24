<ins> Network Address Translation </ins>

In my document subnetting we talked about how we will control traffic inside the network by separating the network into groups, in this document we will be talking about how those groups talk to the external internet however only working with one IP address.

One popular way we do this is through Network Address Translation (NAT), This allows multiple devices to work off of one IP address. For instance, A desktop and a laptop in a household are connected to the same router however having 2 devices mean 2 IP addresses correct? Having NAT enabled will make the routers outbound traffic whether it be from the desktop or laptop it will have the same IP.

<ins>How NAT works</ins>

So you'll see on each device it will have its own private IP address, this will stay the same and wont change. The one that can be changed is the public IP address and that’s the one the router will change so all of the devices are using one IP address.
What will happen is the device will try to send out data through the router from its private IP however when it gets to the router, the router will change it to the public IP address and send it to its destination, once it reaches its destination and receives data to go back to the origin device it will check the data and send it back to the device that correlates with the private IP address it was sent from.

