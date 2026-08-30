<ins>Firewalls</ins>

<img width="638" height="480" alt="image" src="https://github.com/user-attachments/assets/08c44095-494b-4e70-88fc-a9104b9d9611" />

A firewall is a security system that monitors and controls ingress and egress network traffic. We can control this by configuration security rules in the Firewall. Things we can alter are Whitelisting/Blacklisting IP addresses and Websites and packet filtering.

<ins>Types of firewalls</ins>

There are 4 different types of firewalls: 

  - Stateful Firewalls - These track active connections and decides on whether it should enter the network based on its contents. This firewall remembers previous connections and allows them in straight away thus being more efficient. They can also close Ports when they are unused and open them if needed. This firewall works in layer 3 and 4 of the OSI model.
  - Stateless Firewalls - This type of firewall does not track active connections and only inspect the packet as a whole. however its quicker than stateful firewalls but less insecure.
  - Proxy based firewalls (application gateway) - This type of firewall inspects outgoing packets from both client and Web server, it prevents direct connection to either web server or client.
  - Next generation firewalls (NGFW) - This type of firewall has all the features of the other firewalls however its more advanced and can do alot more like:

      - Deep packet inspection - This allows the NGFWs to inspect packets more closely and rigorously allows more granular filtering rules
      - Application awareness - This makes the firewall aware of which applications are running and which ports are open to allow it to prioritise in defending against certain malware types.
      - Identity awareness - Lets you set rules on identity (which user or computer being used to send the data).
      - Sandboxing - This feature allows the firewall to take pieces of code into an isolated space and interrogates the code and finds out if its malicious or not, if malicious it does not allow it into the network.
   
    Firewall-as-a-service (FWaaS) also has these capabilities just in cloud form meaning no hardware required!

  - Web Application Firewalls (WAF) - The other firewalls we have discussed help protect private networks, this firewall protects web application from attackers. it does this by focusing on HTTP traffic between the internet and the application, it defends against attack like SQL injections and cross-site scripting and more!



<ins>Where should i place my firewall on my network?</ins>

There are 3 main places we could put our firewalls however they will differ on what they do due to there placement and scope.

  - Perimeter firewalls - These firewalls are placed on the edge of the network to filter traffic between the internal network and the internet. These are normal the centre of the security environment as it can block external attacks.
  - Internal firewalls - These are used to separate departments in a network so one department cannot access another which means more control over the internal network
  - Distributed firewalls - These firewalls are on each individual device in the network. These have no single point of failure and consistent across all devices. More commonly known as host based firewalls as they are installed by the host device.
