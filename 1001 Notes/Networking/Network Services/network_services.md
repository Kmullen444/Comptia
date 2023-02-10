### DNS

#### Domain Name System (100% up time service)
- Convert names to IP addresses and vice versa

#### Distributed naming system
- The load is balanced across many different servers

#### Usually managed by the ISP or enterprise IT department
- A critical resource

### DHCP server

#### Dynamic Host Configuration Protocol
- Automatic IP address configuration

#### Very common service
- Available on most home routers

#### Enterprise DHCP will be redundant
- Multiple DHCP servers will be running to make sure this service is available
- Usually running on central servers

### File Server

#### Centralized storage of documents, spreadsheets, videos, pictures, and any other files
- A file share

#### Standard system of file management
- SMB (Server Message Block), Apple Filing Protocol (AFP), etc.

#### The front-end hides the protocol
- Allows a users to copy, delete, rename, etc.

### Print Server 

#### Connect a printer to the network
- Provide printing services for all network devices

#### May be software on a computer
- Computer is connected to the printer

#### May be built-in to the printer
- Network adapter and software

#### Uses standard printing protocols
- SMB (Server Message Block),
- IPP (Internet Printing Protocol),
- LPD (Line Printer Daemon)

### Mail Server (100% up-time service)

#### Store your incoming mail
- Send your outgoing mail

#### Usually managed by the ISP or the enterprise IT department
- A complex set of requirements

#### Usually one of the most important services
- Because of this it usually has 24hr a day 7 days a week support

### Syslog

#### Standard for message logging
- Diverse systems, consolidated log

##### Usually a central logging receiver
- Integrated into the SIEM (Security Information Event Manager)

#### You're going to need a lot of disk space
- No, more. More than that!

### Web Server

#### Respond to browser requests
- Using standard web browsing protocols - HTTP/HTTPS
- Pages are built with HTML, HTML5

#### Web pages are stored on the server
- Downloaded to the browser
- Static pages or built dynamically in real-time

### Authentication server (100% up-time)

#### Login authentication to resources
- Centralized management

#### Almost always an enterprise service
- Not required on a home network

#### Usually a set of redundant servers
- Always available
- Extremely important service

### Spam

#### Unsolicited messages
- Email, forums, etc.

#### Various content
- Commercial advertising
- Non-commercial proselytizing
- Phishing attempts

##### Significant technology issue
- Security concerns, resource utilization, storage costs, managing the spam

### Spam gateways

#### Unsolicited email
- Stop it at the gateway before it reaches the user
- On-site or cloud-based
- Email enters through the Internet, passes through the Firewall, then moves to the mail gateway where it is scanned and if it isn't spam is sent to the internal network

### All-in-one security appliance

#### Some times called
- Next-generation firewall, Unified Treat Management (UTM) / Web security gateway

#### URL Filter/Content Inspection

#### Malware Inspection

##### Spam Filter

#### CSU (Channel Service Unit)/DSU (Data Service Unit)

#### Router, Switch

#### Firewall

#### IDS (Intrusion Detection System)/IPS (Intrusion Prevention System) 

### Bandwidth sharper

#### VPN endpoint

### Load Balancers

#### Distribute the load
- Multiple servers
- Invisible to the end-user

#### Large-scale implementations
- Web server farms, database farms

#### Fault tolerance
- Server outages have no effect
-   If a server becomes unresponsive, that server is removed from the load while the rest of the data continues
- Very fast convergence

### Load Balancer features

#### Configurable load
- Manage across servers

#### TCP offload
- Protocol overhead
-   This is done so the load balancer has a constant connection to the servers

#### SSL offload
- Encryption/Decryption

#### Caching 
- Fast Response

#### Prioritization
- QoS (Quality of Service)

#### Content switching
- application-centric balancing
-   Best server for that a certain application

### Proxy Server

#### An intermediate server
- Client makes the request to the proxy
- The proxy performs the actual request
- The proxy then can scan the returned data for any malicious content 
- If there isn't any, the proxy provides results back to the client

#### Useful Features
- Access control (need a login to access the internet or network), caching, URL filtering, content scanning

### SCADA/ICS

#### Supervisory Control and Data Acquisition System
- Large-scale, multi-site Industrial Control Systems (ICS)

#### PC manages equipment
- Power generation, refining, manufacturing equipment
- Facilities, industrial, energy, logistics

#### Distributed control system
- Real-time Information
- System control

#### Requires extensive segmentation
- No access from the outside

### Legacy and embedded systems

#### Legacy systems
- Another expression for "really old"
- May also be "really important"
- Learning old things can be just as important as learning the new things

#### Embedded systems
- Purpose-built devices
- Not usual to have direct access to the operating system
- Examples: Alarm system, door security, time card system

### IoT (Internet of Things)

#### Appliances
- Refrigerators

#### Smart devices
- Smart speakers responds to voice commands

#### Air Control
- Thermostats, temperature control

#### Access
- Smart doorbells

#### May require a segmented network
- Limit any security breaches
