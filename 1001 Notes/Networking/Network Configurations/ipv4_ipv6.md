### IP addressing

#### IPv4 is the primary protocol for everything we do
- Included in almost all configurations

#### IPv6 is now part of all major operating systems
- And the backbone of our Internet infrastructure

### IPv4 addresses

#### Internet Protocol version 4
- OSI Layer 3 address

#### Example:
- 192.168.1.131
  Each of those segments = 8 bits = 1 byte = 1 octet
  The address as a whole = 32 bits = 4 bytes
  Since one byte is 8 bit, the maximum decimal value for each byte is 255

### IPv6 addresses

#### Internet Protocol v6 - 128-bit address
- 340 undecillion
- 6.8 billion people could have 5,000,000,000,000,000,000,000,000,000 addresses each
- These IP addresses are usually broken down into hexadecimal number ie. 5d18

#### Your DNS is very important!

#### These addresses are assigned with a 64-bit subnet mask
- First 64 bits is generally the network prefix (/64)
- Last 64 bits is then the host network address

### Networking with IPv4

#### IP address, e.g., 192.168.1.165
- Every device needs a unique IP address
-   Last byte of the IP address is the host address i.e 165

#### Subnet mask, e.g., 255.255.255.0
- Used by the local device to determine what subnet it's on
-   The subnet mask isn't (usually) transmitted across the network
-   You'll ask for the subnet mask all the time
-     What's the subnet mask of this network?

#### Default gateway, e.g., 192.168.1.1
- The router that allows you to communicate outside of your local subnet
- The default gateway must be an IP address on the local subnet 

### DNS servers

#### We remember names
- professormesser.com, google.com, YouTube.com

#### Internet routers don't know names
- Routers only know IP addresses

#### Something has to translate between names and IP addresses
- Domain Name Services

#### You configure two DNS server in your IP configuration
- That's how important it is
