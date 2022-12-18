### Network Devices

#### Many different devices and components
- All have different roles

#### Some of these functions are combined together
- Wireless router/switch/firewall

#### Compare different devices
- Understand when they should be used

### Router
- Connects multiple switches and their respective networks to form an even larger networks
-   Allow networked devices and mulitple users to access the Internet

#### Routers traffic between IP subnets
- Making forwarding decisions based on the IP address within the packet
- Routers work on OSI layer 3 so they are sometimes called "layer 3 devices"
- Routers can also be found inside of switches, these are called "layer 3 switches"

#### Often connects diverse network types
- LAN (Local Access Network), WAN (Wide Area Network), copper, fiber
- Chooses the most efficient roue for data, in the form of sata packets to travel across the network

### Switches
- Allow devices to share information and talk to each other regardless of there are in a building or campus

#### If you're using a copper cable to plug directly into something, you're probably plugging into a switch

#### Makes forwarding decisions based on the MAC address inside of that frame 
- Switches use "frames" vs Routers which use packets
- Can forward traffic very quickly because bridging is done in the hardware
-   Many switches use Application-specific integrated circuit (ASIC)

#### Many ports and features
- Switches are the core of an enterprise network
- These switches provide many features with some providing Power over Ethernet (PoE)

#### If a switch contains a router there are called Multilayer switches or "layer 3 switches"
- Incluedes routing funcitonality

### Unmanaged switches

#### These can be bought for home use/small business and usually have very few configuration options
- They work through plug and play

#### Fixed configuration
- no VLANs
- Not much you can change on them

#### Very little integration with other devices
- Since they are very simple there are no management protocols 
-   Can't use SNMP to quere the switch for errors or for proformance

#### Low price point
- Since they are simple they are less expensive than something with more features

### Managed switches

#### Come with VLAN support (Virtual Local Area Network)
- Interconnect with other switches via 802.1Q

#### Traffic priortization
- Allow for certain traffic to have priority on the network
-   Voice traffic gets a higher priority

#### Redundancy support 
- Stop loops from happening
- Using Spanning Tree Protocol (STP)

#### Allows for Port mirroring
- One port can be mirrored to another
- This allows for the capture of packets to monitor the network and troubleshooting

#### External Management
- Can use SImple Network Management Protocol (SNMP)

### Access point

#### Not a wireless router
- A wireless router is a router and an access point in a single device
- Access point simple takes a wired connection and makes it wireless

#### An access point is a bridge
- Extends the wired Network onto the wireless network
- Similar to switches Access points make forwarding decisions based on MAC addresses

### Cable infurstructor

#### Every desk has a cable
- These cables are usually permanent and connect to a patch panel

### Patch panels

#### Combination of punch-down blocks and RJ-45 connectors

#### Runs from desks are made once
- Permanently punched down to patch panel

#### Patch panel to switch can be easily changed
- No special tools
- Use exisiting cables

### Firewalls

#### Filters traffic by port number
- OSI layer 4 (TCP/UDP)
-   Some firewalls can filter based on the application making them OSI layer 7 devices

#### Can encrypt traffic into/out of the network
- Protect our traffic between sites

#### Can proxy traffic 
- A common secuirty technique

#### Most firewalls can be layer 3 devices (routers)
- Usually sits on the ingress (incoming)/egress (out going) of the network

### Power over Ethernet (PoE)

#### Power is provided on an Ethernet cable
- One wire for both network and electricity
- Phones, cameras, wireless access points
- Useful in difficult-to-power areas

#### Power provided at the switch
- Some switches have built-in power called Endspans
- If switch doesn't provide power you'll need something in the middle that can provide it
-   In-line power injector provide this power and are called Midspans

### PoE switch

#### Power over Ethernet
- Commonly marked on the switch or interfaces with ports provide PoE

### PoE, PoE+, PoE++

#### PoE: IEEE 802.3af-2003
- The original PoE specification
- Now part of the 802.3 standard
- Provides 15.4 watts DC pwer, 350 mA max current

#### PoE+: IEEE 802.3at-2009
- Now also part of the 802.3 standard
- Provides 25.5 watts DC power, 600 mA max current

#### PoE++: IEEE 802.3bt-2018
- If it provides 51 W its a type 3, 600 mA max current
- If it provides 71.3 W its a type 4, 960 mA max current (designed for 10 gig Ethernet and provide power to 10 gig devices)
- PoE with 10GBASE-T

### Hub

#### "Multi-port repeater"
- Traffic going in one port is repeated (copied) to every other port

#### Everything is half-duplex (can either send **or** recieve)

#### Becomes less efficient as network traffic increases

#### Only available in 10 magebit/ 100 megabit

#### Difficult to find today

### Cable Modem

#### Uses what's called Broadband
- Transmission across multiple frequencies
- Different traffic types (Phone, data, T.V)

#### Data on the "cable" network
- Uses DOCSIS standard
-   Data Over Cable Service Interface Specification)

#### High-speed networking
- Speeds up to 1 Gigabit/s are available

#### Provides Multiple services
- Data, voice, video

### DSL modem 

#### Really ADSL (Asymmetric Digital Subscriber Line)
- Uses telephone lines

#### Download speed is faster than the upload speed (asymmetric)
- Usually have about 10,000 foot limitation from the central office (CO)
- 52 Mbit/s downsteam to 15Mbit/s upsteam are common speeds
- Faster speeds may be possible if closer ot the CO

### ONT 

#### Optical network terminal
- Fiber to the premises

#### Connect the ISP fiber network to the copper network
- The point at this connection is called the Demarcation point (demarc)
-   Can be located in the data center or in homes on the outside of the house
-     This point shows where the ISP is responsible for the connection and where you <br> are responsible
- The terminal box might be on the side of the building 

#### Line of responsibility
- Anything on one sie for the box the ISP is responsible for
- On the other side you are (your network)

### Network Interface Card (NIC)

#### The fundamental network device
- Every device on the network has a NIC
- Computers, servers, printers, routers, switches, phones, tablets, cameras, etc.

#### Need a card specific to the network type
- Ethernet, WAN, wireless, etc.

#### Often built-in to the motherboard
- Or added as an expansion card

#### Many options for cards
- Single port, multi-port, copper, fiber
