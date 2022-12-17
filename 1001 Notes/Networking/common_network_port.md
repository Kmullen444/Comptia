### Port numbers

#### Well-known port numbers
- Client and server need to match

#### Important for firewall rules
- This is Port-based security

#### A bit of rote memorization
- Becomes second nature after a while

#### Make sure you know port number, protoco, and hot the protocol is used
- ex. Test might ask "What port number is used by an application that transfers data <br> in a particular way across the network

### FTP - File Transfer Protocol

#### tcp/20 (active mode data), tcp/21 (control)
- Allows transfer of files between systems

#### Authenticates with a username and password
- Some systems use a generic/anonymous login

#### Full-featured functionality
- Allows things like List, add, delete, etc.

### SSH - Secure Shell

#### Encryted communication link - tcp/22
- Usually through a terminal and uses a text based interface

#### Looks and acts the same as Telnet (see below)

### Telnet

#### Telnet - Telecommunication Network - tcp/23

#### Login to devices romotely
- Allows console access

#### In-the-clear communication
- Telnet doesn't encrypt the data being sent
-   Anyone watching the communication has access to username and passwords
- Not the best choice for production systems, better to use SSH in those situations

### SMTP - Simple Mail Transfer Protocol

#### SMTP - Simple Mail Transfer Protocol - tcp/25
- Server to server transfer

#### Also used to send mail from a device to a mail server
- Commonly configured on mobile devices and email

#### While the email is sent through SMTP, other protocols are used for clients to receive email
- Theses are either IMAP, POP3

### DNS - Domain Name System

#### Converts names to IP addressess - upd/53 (doesn't need conformation the data sent was received) 
- www.professmesser.com = 162.159.246.164

#### These are very critical resources
- Usually multiple DNS servers are in production

### DHCP - Dynamic Host Configuration Protocol

#### Automated configuration of IP addressess, subnet mask and other options - upd/67, upd/68
- Requires a DHCP server
-   Server, applicance, integrated into a SOHO router, etc.

#### Dynamic/pooled
- IP addressess are assigned in real-time from a pool
-  Each system is given a leased IP address and must renew at set intervals

#### DHCP reservation
- Addessess are assigne by MAC address in the DHCP server
- An admin is able to assign IP to specific devices from the server and the <br> next time the system contects and changes to the configurations will be doene
- Manage addressess from one location

### HTTP and HTTPS

#### Hypertext Transfer Protocol (HTTP)
- Commmunication in the browser
- And by other applications

#### Hyper Transfer Protocol Secure (HTTPS)
- Same as HTTP but connection is encrypted 

#### In the clear (no encryption)
- HTTP - tcp/80

#### Encrypted 
- HTTPS - tcp/443

### POP3/IMAP

#### Receive emails from an email server
- Authenticate and transfer

#### POP3 - Post Office Protocol verison 3 - tcp/110
- Basic mail transfer functionality

#### IMAP4 - Internet Message Access Protocol v4 - tcp/143
- Includes management of email inbox from multiple clients

### SMB - Server Message Block

#### Protocol used by Microsoft Windows
- File sharing, printer sharing
- Also called CIFS (Common Internet File System)

#### Older Windows systems will use NetBIOS over TCP/IP (Network Basic Input/Output System)
- udp/137 - NetBIOS name services (nbname) - find devices on your network by the name
- tcp/139 - NetBIOS session services (nbsession)

#### Newer Windows systems will connect direct over tcp/445 (NetBIOS-less)
- Direct SMB Commmunication over TCP with the NetBIOS transport

### SNMP - Simple Network Management Protocol

#### Gather statistics from network devices
- Queries: upd/161
- Traps: upd/162 
-   Traps allow

#### When you use SNMP it will ask you what version you're running

##### v1 - The original
- Structured tables
- Data sent in-the-clear (non-encrypted)

##### v2 - A good step ahead 
- Data type enhancements 
- Bulk transfer
- Still in-the-clear

##### v3 - a sercure standard
- Message intergrity 
- Authentication
- Encryption of all the SNMP data

### LDAP (Lightweight Directory Access Protocol) - tcp/389

#### Store and retrieve information in a network directory
- Commonly used in Microsoft Active Directory

### RDP - Remote Desktop Protocol - tcp/3389

#### Share a desktop from remote location over tcp/3389

#### Remote Desktop Servieces on many Windows verisons

#### Can connect to an entire desktop or just an application

#### There are RDP clients for Windows, macOS, Linux, Unix, iPhone, Andriod and others

