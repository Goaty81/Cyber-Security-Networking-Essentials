<ins>Dynamic host configuration protocol DHCP</ins>

OK, we have talked about What an IP is, How it works and how DNS servers use it but where does the IP address get created?

It gets created in the DHCP (Dynamic host configuration protocol), DHCP is a standard networking protocol with a pool of IP addresses ready to give out to new devices.

<ins>How does the DHCP work?</ins>

Ever think of manually finding an IP address until one isn’t getting used? it would take forever wouldn’t it? What DHCP does it find it for you automatically when you connect to the internet!

Whenever a device is connected to the internet its assigned an IP address so that the internet knows who the device is and who to send data from and to.

Here is the breakdown of that process:

1. Discover: Your device yells out to find a DHCP server (normally in your router).
2. Offer: The server shouts back with an open IP address.
3. Request: Your device asks the DHCP server to use that IP address.
4. Acknowledgement: The server says yes and locks that IP address to that device.

Quite impressive stuff right?

<ins>Primary Components of DHCP</ins>

The primary components of DHCP consist of three parts, the DHCP server,DHCP client and DHCP relay.

The DHCP server is what the devices go to ask for a IP address. It holds the "pool" of unused IP addresses which gives it the ability to assign IP address automatically to each device requesting and IP address. It is able to provide temporary and dynamic IP addresses form the pool of available IP addresses.
In addition to that a DHCP server gives permenant IP addresses and DHCP configuration parameters, including subnet masks, default gateways and DNS servers.

The DHCP client is the device asking for the information from the DHCP server, it acts as a host for the IP address that the DHCP gives out.

The DHCP relay is any TCP/IP host that forwards DHCP messages between servers and clients. For instance when a network consists of multiple subnetworks the DHCP relay would enable the DHCP server to provide the necessary information to the clients both on the primary network and subnet.

<ins>Security considerations for using DHCP</ins>

