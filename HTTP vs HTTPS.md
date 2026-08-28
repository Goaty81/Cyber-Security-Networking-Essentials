<ins>What is HTTP</ins>

HTTP (HyperText Transfer Protocol) is the foundation of data communication of the world wide web. After all everything had to start from something, This is where HTTPS started.

<ins>HTTP in Application layer</ins>

HTTP is in the Application layer of the OSI model, HTTP and its versions (HTTP/0.9, HTTP/1,0 HTTP/1.1, HTTP/2, HTTP/3) <ins>were</ins> the fore front of data transportation due to its reliability. It is a request-response protocol in the client server model. For example, a client would click enter to search for a website and HTTP would send a GET request to the server, Then the server would respond with a PUT, which then the information would be provided, However this would be invisible to the users. In HTTP/1.0 a TCP connection to the same sever is made with every resource, In HTTP/1.1 the TCP connection can be reused to make multiple requests, In HTTP/2 a TCP/IP connection are used, HTTP/3 used QUIC which provided reliability for the unreliable UDP.

<ins>HTTP vs HTTPS</ins>

So we know what HTTP is and what it was used in. However, this protocol wasn't as secure as we wanted it to be. It wasn't encrypted, So attackers could quite use this vulnerability to do damage to assets connected to the internet.

HTTPS (HyperText Transfer Protocol Secure) on the other hand is what we still use today. This works in the Transport layer. Its a secure extension of HTTP as it uses encryption for secure communication over a computer network. It can use SSL (Secure Socket Layer) for this or TLS (Transport Layer Security), Commonly known as HTTP over SSL or HTTP over TLS.

The two main reasons why HTTPS was created was for authentication, privacy and integrity of the exchanged data over transit through the internet. This protects from attacks like MITM (Man-In-The-Middle), eavesdropping and tampering data.

The authentication side of HTTPS requires a trusted third party to sign server-side digital certificates, with HTTP the digital certificates were expensive which only made then viable to payment transactions, however now that HTTPS is built in with this it means that most sites with HTTPS:// next to it are in fact trusted and encrypted over TLS.

| | HTTP | HTTPS |
|-----|-----|-----|
| URL | http:// | https:// |
| Security | Unsecure | Secure |
| Port | 80 | 443 |
| OSI Layer | Application | Transport |
| TLS Certificates | NO | Yes|
| Domain Validation | Not Required | Required |
| Encryption | No | Yes |

<img width="738" height="345" alt="image" src="https://github.com/user-attachments/assets/a530f547-e592-455e-84c9-1572198b8807" />
