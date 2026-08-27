<ins>TCP and UDP</ins>

<img width="738" height="360" alt="image" src="https://github.com/user-attachments/assets/ac0c1605-4cbb-47ce-aa46-65b60347e4c3" />

First of all what is TCP (Transmission Control Protocol) and UDP (User Datagram Protocol)? 

These two protocols are the core protocols of the transport layer of the OSI and TCP/IP models, both of these protocols have there use-cases uses for each activity on the internet. Each are responsible for the end-to-end communication between applications/devices, They are both needed for the efficiency and reliability of our networks. The way i remember these protocols are they're like brothers, one prioritises accuracy over speed, the other prioritises speed over accuracy.

<ins>TCP (Transmission Control Protocol)</ins>

TCP is the more reliable one of the two, however its slower and more critical of its job. It likes to do things in order and likes things to be organised and in the right place. So as for its Data, anything sent over TCP will be at the correct address, in the right order and will guarantee data correctness. We call this a connection-orientated protocol.
This Protocols Use cases examples are:

  - Emails
  - Downloads
  - Transactions
  - Web browsing

TCP also has common ports it will work on such as:

  - 22 Secure Shell (SHH)
  - 443 HTTPs
  - 23 Telnet
  - 110 POP3
  - 3389 Remote Desktop Protocol (RDP)

Think is TCP as the older more responsible one!

<ins>User Datagram Protocol</ins>

UDP is more the younger, more skittish brother of the two. It likes to go fast and doesn’t really care about which order it gives it to you in or if it gives it to you at all. This is called a connectionless protocol. 
This protocols use cases examples are:

  - Streaming
  - Online gaming
  - VoIP (Voice over IP)
  - DNS lookups

UDP has also common ports it works on such as:

  - 53 Domain Name System (DNS)
  - 127/138 NetBIOS
  - 123 Network Time Protocol (NTP)
  - 69 Trivial File Transfer Protocol (TFTP)
  - 67/68 Dynamic Host Configuration Protocol (DHCP)

<ins>TCP vs UDP</ins>

In the table below it will show the differences in TCP compared to UDP.

| TCP | UDP |
|-----|-----|
|Connection-orientated | Connectionless|
|treats data as a continuous bit stream | Treats data as independent packets|
|Guarantees reliability of data | Doesn’t guarantee delivery|
|Slower due to high overhead | Fast due to low overhead|
|Uses acknowledgements (ACKS) | No Acknowledgements|
|Uses a variable header between sizes 10 - 60 bytes | Fixed header size to 8 bytes|

