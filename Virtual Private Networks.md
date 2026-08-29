<ins>Virtual Private Networks</ins>

A VPN (Virtual Private Network) is a network that uses virtualisation as a security mechanism to extend private networks, It does this by using encryption and tunnelling protocols to send data from one host to another.

There are there main uses of VPN, these being Host - Host, Host - Network and Network to Network. Host to Host is where there is two individual devices connected to each other via the tunnelling protocol, For example you are sending private data to a client. The Host to network is where a host is connected to a network via a VPN, For example is you was to work from home you would use a VPN to connect to your works servers to prevent attacks. Network to Network is where two networks are connected to each other, this is commonly used within organisations for site - site connections which connect the two business networks together.

<ins>VPN Security</ins>

When VPN is in use it creates a encrypted tunnel so that data inside that tunnel cannot be seen, this enhances confidentiality and reduces the risk of data sniffing. VPNs also use tamper proofing via a message authentication code to prevent data packets from being altered which increases integrity.

<img width="740" height="493" alt="image" src="https://github.com/user-attachments/assets/199da368-47d9-4f10-9933-d95cbb16aefd" />

So we have talked about the tunnel itself, but what about the two endpoints? These can be authenticated in a couple of ways. These being that a IP address could be whitelisted which puts that specific IP in the trusted section as the network or system already knows who you are connecting to. The other authentication method might be when the tunnel is already active and that is through Password, MFA, biometrics and cryptography methods (Digital certificates and Hardware security keys and passkeys).
