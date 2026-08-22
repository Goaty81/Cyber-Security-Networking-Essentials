<ins>Domain name system</ins>

So first of all what is a Domain name system (DNS)?

Think of a phone book but for the internet, you know the book that holds all the phone numbers of people?
Domain name system (DNS) works exactly like that, However instead of phone numbers its IP addresses.

<ins>Types of DNS servers</ins>

DNS was designed with a hierarchical, distributed database structure to had a more dynamic approach to domain name resolution. After all it would need to keep up with the ever expanding internet.
The hierarchy starts at the root level denoted by a dot (.) for example: www.google.com the dot for the DNS would be the dot before for com and then branches out the the top level domains (TLDs),
Such as ".com", ".net" and ".org" or Country code top level domains (ccTLDs) such as ".uk", ".jp" and ".au".

</ins> DNS architectures<ins>

There are two types of DNS servers, Recursive and Authoritative. Recursive is the one doing the searching (asking), it searches for the information that connects the user to the website. Authoritative servers provide the "answers".

<ins>Recursive DNS servers</ins>

Recursive servers are typically managed by internet service providers (ISPs) or third party DNS service providers. however a organisation can also provide it own server.
Recursive servers act on behalf of the end user to resolve the domain name to the IP address it also stores a temporary cache of recent DNS lookups to improve the system efficiency.
When a user types a web address into a web browser, the browser will connect to a recursive DNS server to resolve the request. Then the recursive server will queries the DNS hierarchy until it finds the DNS records containing  the IP address for the given domain.

<ins>Authoritative servers</ins>

Authoritative servers hold the definitive records for a domain and respond to requests about domain names stored within their respective zones. There are different servers that are each responsible for a distinct part of the namespace these are root name servers, Top-level domains (TLDs) and other name servers.

  - Root name servers - Root name servers are at the top of the DNS hierarchy and are responsible for serving the root zone (Central database for the DNS). There are 13 root nameservers "identities" or "authorities" (logical groupings of root servers) identified by letters A through to M. They answer queries for records sorted within the root zone and refer requests to the appropriate TLD name server.

  - Top-level domain (TLD) name servers - TLD servers are responsible for managing the next level of the hierarchy, including generic top-level domains (gTLDs). TLD name servers direct queries to the authoritative name servers for the specific domains within their TLD. so, the TLD name serve ".com" would direct domains ending in ".com", the TLD name server for ".gov" would direct domains ending in ".gov" and so on.

  - Second level domain servers (SLD) - SLDs are directly below Top-level domains, for example in google.com, google is the second-level domain of the .com TLD. SLDs commonly refer to the organisation that is registered to the domain name registrar.

<ins>DNS zone files and resource records</ins>

So we have gone through the server types of the DNS servers, in addition to them the DNS uses zone files and several record types to help with the resolution process. Zone files are text-based that include mappings and information about specific domains within the DNS zone.

Each line of a zone file specifies a DNS resource record. The resource records help ensure that when a user submits a query, the DNS can quickly convert domain names into actionable information that directs queries to the correct server.

There are two mandatory records: name server (NS) records which indicates the authoritative name server for a domain and the start of authority (SOA) record which specifies the primary authoritative name server of the DNS server.

Zone files include several other record types other than the two primary records which are:

  - A and AAAA records - A records links the domain to IPv4 addresses while AAAA links the domain to IPv6 addresses.
  - Mail exchanger records (MX record) - Specifies a SMTP email server for a domain.
  - Canonical name records (CNAME records) - Redirect hostnames from an alias to another domain (the  "Canonical domain").
  - Pointer records (PTR records) - Specifies a reverse DNS lookup process, mapping IP addresses back to domain names.
  - Sender policy framework (SPF) records - Identifies the mail servers that have permission to send emails through a domain.
  - Text records (TXT records) - Used for human-readable notes and automated processing, such as sender policy frameworks for email authentication.

<ins>How DNS works</ins>

So say for instance i wanted to access www.google.co.uk what we normally do is type it into our browser search bar and it comes up, right?

However what we don’t see is DNS working,

What actually happens when you press enter is that our device will send a signal (DNS request) to the DNS recursive resolver asking for www.google.co.uk, the DNS recursive resolver will then query the Authoritative DNS servers to look up google in its phone book and see that google has an IP address, Then it would match the name of the service (google) to the IP address then it will direct you to googles website.

<img width="1200" height="675" alt="image" src="https://github.com/user-attachments/assets/3426b42a-8756-4d85-b667-80029102947b" />

Query resolution in the DNS involves several key processes and components.

  - Query initiation
  - Recursive resolver
  - Root name server
  - Top-level domain name servers
  - Domain name server
  - Query resolution
