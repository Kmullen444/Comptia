### Networking is like a series of moving vans

#### Efficiently move large amounts of data
- If we need to move large amounts of things we would get a moving truck

#### The network topology is the road that moving truck travels on
- These network topology include
-   Ethernet
-   DSL
-   Cable system

#### The truck is the Internet Protocol (IP)
- We've designed the roads (network topology) for this truck

#### The boxes inside the truck hold your data
- These boxes hold TCP and UDP
-   The truck doesn't know what's in the boxes, it just carries them

#### Inside the boxes are more things
- Once the truck has reached its destination, we open up the boxes
- A box may belong to some room in your house
-   When the box is delivered it needs to be moved to that room
- Inside the boxes could be things like Application information

### IP - Internet Protocol

- On one side is the client (your laptop, a workstation)
- On the other is the server
- The client will send info to the server
-   In the case of ethernet it will be called an Ethernet payload
-     In Ethernet you will also have an Ethernet header (on the client side) <br> and an Ethernet Trailer on the server side
-   Since the most popluar protocol we use on our networks is IP the Ethernet header will have an IP header and there will <br> an IP payload within that part of the frame
-     The data inside the IP payload can also have data inside of it like TCP, <br> giving this a TCP header
-       The TCP may also have data within with an include TCP header

### TCP and UDP

#### Transported inside of IP 
- This is sometime called Encapsulation in the IP protocol

#### These are two ways to move data from place to place
- Differeent features for different applications

#### Sometimes refered to as being on the OSI Layer 4 of the IP protocol
- The transport layer

#### Multiplexing
- Unlike HTTP this allows for the use of many different applications at the same time
- Both TCP and UDP have this

### TCP - Transmission Control Protocol

#### Sometimes refered to as "Connection-oriented"
- This mean a formal process to create a connection and one when the conversation is over

#### "Reliable" delivery
- TCP has varification that the data sent has been received
- TCP has a bulit-in system to recover from errors
- It can also manage out-of-order messages or retransmissions

#### Flow control
- This allows receiver(the server) to control the speed and amount at which the data is sent

### UDP 

#### Connectionless
- Unlike TCP there is no formal process to open or close the connection

#### "Unreliable" Delivery
- No verifaction system to assuse the data that was sent has been received
- No reordering of data or retransmissions

#### No flow control
- The sender determnes the amount and speed of the data that is transmitted

### Why would you ever use UDP?

#### UDP is real-time communication
- There's no way to stop and resend the data when you talking 
- Time doesn't stop for your network
- ex. VoIP (Voice over IP) uses UDP

#### Connectionless protocols
- DHCP (Dynamic Host Configuration Protocol)
-   Automatically assing IP addresses to our devices
- TFTP (Trivial File Transfer Protocol)

#### The data might not get through
- The application keeps track and decides what to do 
- It might not do anything
- ex. If DHCP sends data and doesn't receive a response from the server DHCP is responsible for resending that data

### Communincation using TCP

#### Connection-oriented protocols prefer a "return receipt"
- HTTPS (Hypertext Transfer Protocol Secure)
-   Commonly used in web browswer
- SSH (Secure Shell)
-   Allows for encrypted connection to another device

#### The application doesn't worry about out of order frames or missing data
- TCP handles all of the communication overhead
- The application has one job
- ex. If packets are missing from an HTTPS connection TCP manages the resending of those packets and HTTPS doesn't have to worry

### Speedy delivery (Using the shipping truck from earlier)

#### The IP delivery truck delivers from on (IP) address to another (IP) address
- Every house has an address, every computer has an IP address

#### Boxes arrive at the house (IP address)
- Where do the boxes go?
- Each box has a room name (Port)

#### Port is written on the outside of the box
- Drop the box into the right room
- ex. House (IP address) recieves a box (data) with the room name on the outside (Port) <br> the box can then be taken to that room and unpacked

### Lots of ports

#### IPv4 sockets
- Server IP address, protocol, server application port number
- Client IP address, protocol, client port number

#### Non-ephemeral ports - (permanent port numbers)
- Can be any port between 0 - 1023 aslong as they are commonly known and well known across multiple devices
- Usually on a server or service
- ex. HTTP use Port 80, HTTPS uses Port 443

#### Ephermeral ports - (temporary port numbers)
- Between Ports 1024 - 65535
- These are determined in real-time by the client (OS)

### Port Numbers

#### TCP and UDP ports can be any number between 0 and 65535

#### Most servers (services) use non-ephemeral (not-temporary) port numbers
- This isn't always the case
-   It's just a number
-   As long as the server knows where that data is supposed to go everything runs smoothly

#### Port numbers are for communication, not security
- Even if you use a random port, it's very easy to run a port-scaner and find what services are using what port
- You would also need another service in place to make sure that the right data is going to the right port if everything were random
- That's why service port numbers need to be "well known"

#### TCP port numbers aren't the same as UDP port numbers 
- Port 80 on TCP isn't the same as Port 80 on UDP
- Isn't usually done in normal operation
