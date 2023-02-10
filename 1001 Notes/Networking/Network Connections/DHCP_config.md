### Scope properties

#### Things you'll need to assign DHCP server connection

#### IP address range 
- And excluded addresses

#### Subnet Mask

#### Lease durations

#### Other scope options
- DNS server
- Default gateway
- VOIP servers

### DHCP pools 

#### Grouping of IP addresses
- Each subnet has it wn scope
- 192.168.1.0/24
- 192.168.2.0/24
- 192.168.3.0/24
- ...

#### A scope is generally a single contiguous pool of IP addresses
- DHCP exceptions can be made side of the scope

### DHCP address assignment 

#### Dynamic assignment
- DHCP server has a big pool of addresses to give out
- Addresses are reclaimed after a lease period

#### DHCP address allocation

#### Address reservation
- Administratively configured

#### Table of MAC addresses
- Each MAC address has a matching IP address

#### Other name
- Static DHCP Assignment
- Static DHCP
- Static Assignment
- IP Reservation

### DHCP leases

#### Leasing your address
- It's only temporary
- But it can seem permanent

#### Allocation
- Assigned a lease time by the DHCP server
- Administratively configured

#### Reallocation
- Reboot your computer
- Confirms the lease

#### Workstation can also manually release the IP address
- Moving to another subnet

### DHCP renewal

#### Other timers besides the set lease time

#### T1 timer
- Check in with the lending DHCP server to renew the IP address
- Happens at 50% of the lease time (by default)

#### T2 Timer
- If the original DHCP server is down, try rebinding with any DHCP server
- Happens at 87.5% of the lease time (7/8th)
