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

<img width="338" height="276" alt="image" src="https://github.com/user-attachments/assets/4919142a-037d-430b-9228-aa759bce8776" />


Quite impressive stuff right?

<ins>Primary Components of DHCP</ins>

The primary components of DHCP consist of three parts, the DHCP server,DHCP client and DHCP relay.

The DHCP server is what the devices go to ask for a IP address. It holds the "pool" of unused IP addresses which gives it the ability to assign IP address automatically to each device requesting and IP address. It is able to provide temporary and dynamic IP addresses form the pool of available IP addresses.
In addition to that a DHCP server gives permanent IP addresses and DHCP configuration parameters, including subnet masks, default gateways and DNS servers.

The DHCP client is the device asking for the information from the DHCP server, it acts as a host for the IP address that the DHCP gives out.

The DHCP relay is any TCP/IP host that forwards DHCP messages between servers and clients. For instance when a network consists of multiple subnetworks the DHCP relay would enable the DHCP server to provide the necessary information to the clients both on the primary network and subnet.

<ins>Security considerations for using DHCP</ins>

In the eyes of cyber security we like to try and keep everything secure, DHCP poses its own considerations to keep it secure:

  - A DHCP server can only provide a limited number of IP addresses, This means an attacker may try to DDoS (Distributed Denial of Service) the service by sending it loads of IP requests which may cause disruption in the service.
  - It is also possible for the attacker to make a false DHCP server to send fraudulent IP addresses to the clients on the network.
  - Users that get an IP address also get a DNS address meaning it is possible they can obtain more data than they should from those servers.

One other security consideration is what is called a DHCP starvation attack. This is where an attacker sends fake IP requests to the server to exhaust it al all IP addresses, therefore giving the attacker a chance to deny authorised users to the network as well as making a fraudulent DHCP to pave the way for a Man In The Middle (MiTM) attack.

<ins>Best practices for DHCP deployment</ins>

To enable effective deployment of DHCP a few best practices are to be considered

  - Avoid putting DHCP on your domain controller - This will prevent your Domain controller from being overwhelmed with requests and prevents those connecting to your Wi-Fi as guests from having access to your domain controller which will keep your attack surface small, especially is those that wish to cause harm to you network access your guest Wi-Fi then at least there is still barriers to get passed after the to reach the domain controller.
  - Use DHCP failover - If one server goes down, to make sure the network is still available it is best to have a secondary server (failover server).
  - Avoid using static IP addresses where possible - using static IP make it easier for the attacker to scan the IP because it never changes, using DHCP will allow the IP address to be continuously changed making it harder for the attacker to scan it.

<img width="921" height="472" alt="image" src="https://github.com/user-attachments/assets/b46401b3-70bb-4f18-bd79-f0ad4bd6994d" />
