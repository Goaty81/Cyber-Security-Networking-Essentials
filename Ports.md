<ins>Ports</ins>

Ports are like doors that open and shut to let information in and out, They are virtual endpoints that allows devices to communicate efficiently and effectively with websites,applications and over a network. Well, with 65535 of them you would think that would be enough!

<ins>Well-known Ports, Registered Ports and Dynamic/private ports</ins>

Yes, there is 65535 ports available to use however these are split down into three categories. One being Well-known ports, registered ports and Dynamic private ports.

Well-known ports range from 0 - 1023. These are ports are the ports that make up the core internet protocols because they’re known for standardisation and security. These well known port include ports like 80(HTTP),22(SSH),69(TFTP),443(HTTPS) and 21 (FTP).

Registered ports range from ports 1024 - 49151. These ports are used by applications and user programs and are given these so that they do not conflict with the well known Ports. These include Ports like: 1119 (Battle.net), 1220 (Quicktime streaming server) and 1433/1434 (MSSQL)

Dynamic private Ports range from 49152 - 65535. These ports are used for temporary (ephemeral) use only, meaning these are never permanently used by a specific application or service.

<ins>Common ports and the cyber risks that are associated with them</ins>

Having common ports that alot of services/applications use is very convenient however it not only becomes convenient for the normal internet user it also comes convenient for the attackers themselves. stated below are some common ports and there cyber risks that that attackers could exploit:

1. 443 (HTTPS) - Vulnerable to phishing and malicious fake SSL certificates.
2. 21 (FTP) - Vulnerable to spoofing, sniffing and brute force attacks.
3. 67/68 (DHCP) - Vulnerable to MITM attacks and IP address conflicts.
4. 22 (SSH) - Vulnerable to Brute force attacks if the credentials are not up to secure standard.
5. 23 (Telnet) - Vulnerable to eavesdropping and credentials being stolen.
6. 3389 (RDP) - Vulnerable Unauthorised access and brute force attacks.
7. 1433/1434 (MSSQL) - Vulnerable to SQL injection attacks and unauthorised access.
8. 123 (NTP) - Vulnerable to DDoS attacks.
9. 389 (LDAP) - Vulnerable to SQL injections, directory traversal and unauthorised access.
10. 161/162 (SNMP) - Vulnerable to unauthorised access and information disclosure.

Many ports are frequently left open without the need for them t be, this in itself is a security risk as it makes the networks attack surface bigger than it needs to be. If they are unused close them.!
