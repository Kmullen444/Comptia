### DHCP

#### IPv4 address configuration used to be manual
- IP address, subnet mask, gateway, DNS servers, NTP servers, etc.

#### October 1993 - The bootstrap protocol
- Sometimes called BOOTP

#### BOOTP didn't automatically define everything
- Some manual configurations were still required
- BOOTP also didn't know when an IP address might be available again

#### Dynamic Host Configuration Protocol (DHCP)
- Initially released in 1997, updated through the years
- Provides automatic address/IP configuration for almost all devices

### DHCP process

#### DORA (Discover, Offer, Request, Acknowledge)
- A four-step process

#### Discover
- Your machine will look for a DHCP server

#### Offer
- The DHCP server will then an IP address to your device

#### Request
- Your device will then look at the one/many DHCP offers and lock in the offer and request the IP address from that DHCP server

#### Acknowledge
- Your device will then acknowledge that offer and the DHCP server will provide the device with all the IP configurations it needs

### Turning dynamic into static

#### DHCP assigns an IP address form the first available from a large pool of addresses
- Your IP address will occasionally change

#### You may not want your IP address to change
- Server, printer, or personal preference

#### Disable DHCP on the device
- Configure the IP address information manually
- Requires additional administration

#### **Better Option:** Configure an IP reservation on the DHCP server
- Associate a specific MAC address with an IP address

### Avoid manual configurations

#### No DHCP server reservation
- You configure the OP address manually

#### Difficult to change later
- You must visit the device again

#### A DHCP reservation is preferable
- Change the IP address from he DHCP server

### Automatic Private IP Addressing (APIPA)

#### A link-local address
- No forwarding by routers

#### IETF has reserved 169.254.0.0 through 169.254.255.255
- First and last 256 addresses are reserved
- Functional block of 169.254.1.0 through 169.254.254.255

#### Automatically assigned
- Uses ARP (Address Resolution Protocol) to confirm the address isn't currently in use

#### If a device on the network has a APIPA address, there wasn't a DHCP server available when it tried to connect 
