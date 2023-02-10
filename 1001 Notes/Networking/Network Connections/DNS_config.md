### Domain Name System

#### Translates human-readable names into computer-readable IP addresses
- You only need to remember www.ProfessorMesser.com

#### Hierarchical
- They follow the path

#### Distributed database
- Many DNS servers
- 13 root server clusters (Over 1,000 actual servers)
- Hundreds of generic top-level domains (gTLDs) - .com, .org, .net, etc.
- Over 275 country code top-level domains (ccTLDs) - .us, .ca, .uk, etc.

### DNS lookup

#### `dig [website address]`
- Will show you the IP address to that site and any other IP addresses associated with it

#### `nslookup [website address]` 
- If your system doesn't support `dig` then you can use nslookup
- This goes to you locally configured DNS server and provides answer for the IP addresses

### DNS records

#### Resource Records (RR)
- The database records of domain name services 

#### Over 30 record types
- IP addresses, certificates, host alias names, etc.

#### **These are important and critical configurations**
- Make sure to check your settings, backup, and test!

### DNS configuration

### Address records (A - IPv4) (AAAA - IPv6)

#### Defines the IP address of a host
- This is the most popular query

#### **A** records are for IPv4 addresses
- Modify the A record to change the host name to IP address resolution

#### **AAAA** records are for IPv6 addresses
- The same DNS server, different records

#### Example:

`www.professmessor.com. IN A 162.159.246.164 ; Professor Messer`

- `www.professmessor.com.` shows the domain name of the site ending in `.`
- `IN` show that it is an internet address
- `A` shows it's using a **A** record
- `162.159.246.164` is the IP address for that domain
- ` ; Professor Messer` is an additional comment for the record

#### **A** records
- Web front-ends for A records can also give you a Time to Live (TTL) for that record 
-   After the set time the record will be removed and if another request needs to be made to the site a new request will need to be made

### Mail exchanger record (MX)

#### Determines that host name for the mail server
- This isn't an IP address; it's a name
- Example:
-   `IN MX mail.mydomain.name`
-   This will still need an A record for the mail domain

### Text records (TXT)

#### Human-readable text information 
- Useful public information
- Was originally designed for informal information

#### Can be used for verification purposes
- If you have access to the DNS, then you must be the administrator of the domain name

#### Commonly used for email security
- External email servers validate information from you DNS

### Viewing TXT records with dig

`dig [website domain] txt`

### Viewing TXT records with nslookup

`nslookup -type=txt [website domain]`

### Sender Policy Framework (SPF)

#### SPF protocol
- A list of all servers authorized to send emails for this domain 
- Prevent mail spoofing
- Mail servers perform a check to see if incoming mail really did come from an authorized host
- Also has a TTL setting when adding to the DNS server

### Domain Keys Identified Mail (DKIM)

#### Digitally sign a domain's outgoing mail
- Validated by mail servers, not usually seen by the end user
- The public key is in the DKIM TXT record

### DMARC

#### Domain-based Message Authentication, Reporting, and Conformance (DMARC)
- Prevents unauthorized email use (spoofing)
- An extension of SPF and DKIM

#### You decide what external email servers should do with emails that don't validate through SPF or DKIM
- That policy is written into a DMARC TXT record
- Accept all, send to spam, or reject the email
- Compliance reports can be sent to the email administrator
