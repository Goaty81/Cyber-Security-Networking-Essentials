</ins>Domain name system<ins>

So first of all what is a Domain name system (DNS)?

Think of a phone book but for the internet, you know the book that holds all the phone numbers of people?
Domain name system (DNS) works exactly like that, However instead of phone numbers its IP addresses.

What the DNS will do is match the Website address to the IP address!
So say for instance i wanted to access www.google.co.uk what we normally do is type it into our search bar and it comes up, right?

However what we don’t see is DNS working,

What actually happen when you press enter is that our device will send a signal to the DNS asking for www.google.co.uk, it will look up google in its massive phone book and see that google has an IP address,
Then it would match the name of the service (google) to the IP address then it will direct you to googles website.

</ins>Types of DNS servers<ins>

DNS was designed with a hierarchical, distributed database structure to had a more dynamic approach to domain name resolution. After all it would need to keep up with the ever expanding internet.
The hierarchy starts at the root level denoted by a dot (.) for example: www.google.com the dot for the DNS would be the dot before for com and then branches out the the top level domains (TLDs),
Such as ".com", ".net" and ".org" or Country code top level domains (ccTLDs) such as ".uk", ".jp" and ".au".

</ins> DNS architectures<ins>

There are two types of DNS servers, Recursive and Authoritative. Recursive is the one doing the searching (asking), it searches for the information that connects the user to the website. Authoritative servers provide the "answers".

</ins>Recursive DNS servers<ins>

Recursive servers are typically managed by internet service providers ( ISPs) or third party DNS service providers. however a organisation can also provide it own server.
Recursive servers act on behalf of the end user to resolve the domain name to the IP address it also stores a temporary cache of recent DNS lookups to improve the system efficiency.
When a user types a web address into a web browser, the browser will connect to a recursive DNS server to resolve the request. Then the recursive server will queries the DNS hierarchy until it finds the DNS records containing  the IP address for the given domain.
