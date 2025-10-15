#### Roadmap.sh/backend
##### Internet - How does the internet work - How does the Internet Work article

- Network - a group of computer or other devices that are connected to eachother e.g. network in your home
- Internet is a network of networks
- High level: works by connectin devises and computer systems togther using standardized protocols
- Core of internet: global network of interconnected routers
- Protocols: IP, TCP, DNS, HTTP, SSL/TLS
- Packet: A small unit of data that is transmitted over the internet.
- Router: A device that directs packets of data between different networks.
- IP Address: A unique identifier assigned to each device on a network, used to route data to the correct destination.
- Domain Name: A human-readable name that is used to identify a website, such as google.com.
- DNS: The Domain Name System is responsible for translating domain names into IP addresses.
- HTTP: The Hypertext Transfer Protocol is used to transfer data between a client (such as a web browser) and a server (such as a website).
- HTTPS: An encrypted version of HTTP that is used to provide secure communication between a client and server.
- SSL/TLS: The Secure Sockets Layer and Transport Layer Security protocols are used to provide secure communication over the internet.
- 

##### Internet - How does the internet work - How does the Internet Work short youtube
- IP Address: every website is stored on a server in a datacenter which also has an ip address. You could access that server by the ip address but obviously difficult for humans to remember so we use domain names.
- DNS server provides a directory which links ip addresses to domain names
- ICANN corporation that regulates
- Data is transferred in small data packets that include a sequence number which is used to reassemble the packets in order at the destination device
- Protocols

#### Internet - How does the internet work? - How does the internet work? whitepaper
- ping <domain name> command in terminal
- each message sent across internet broken into packets
- traceroute <domain name> command in terminal

- When you type a URL into a web browser, this is what happens:
1. If the URL contains a domain name, the browser first connects to a domain name server and retrieves the corresponding IP address for the web server.
2. The web browser connects to the web server and sends an HTTP request (via the protocol stack) for the desired web page.
3. The web server receives the request and checks for the desired page. If the page exists, the web server sends it. If the server cannot find the requested page, it will send an HTTP 404 error message. (404 means 'Page Not Found' as anyone who has surfed the web probably knows.)
4. The web browser receives the page back and the connection is closed.
5. The browser then parses through the page and looks for other page elements it needs to complete the web page. These usually include images, applets, etc.
6. For each element needed, the browser makes additional connections and HTTP requests to the server for each element.
7. When the browser has finished loading all images, applets, etc. the page will be completely loaded in the browser window.

TCP is responsible for routing application protocols to the correct application on the destination computer.
TCP is not a textual protocol. TCP is a connection-oriented, reliable, byte stream service. Connection-oriented means that two applications using TCP must first establish a connection before exchanging data. TCP is reliable because for each packet received, an acknowledgement is sent to the sender to confirm the delivery. TCP also includes a checksum in it's header for error-checking the received data
- When the TCP layer receives the application layer protocol data from above, it segments it into manageable 'chunks' and then adds a TCP header with specific TCP information to each 'chunk'. The information contained in the TCP header includes the port number of the application the data needs to be sent to
- When the TCP layer receives a packet from the IP layer below it, the TCP layer strips the TCP header data from the packet, does some data reconstruction if necessary, and then sends the data to the correct application using the port number taken from the TCP header.

#### Internet - How does the internet work? - How does the internet work? freeCodeCamp youtube 
- What is the switch and why do we need it?
   - Access point device or switch device connects internet devices in a single network (home or office)
   - LAN = local area netowrk - series of devices connected via switch or access pont device
   - Etherenet outlets are LAN ports that allow computers to connect to Switches
- What is the router?
  - enable computers to connect to the internet
  - LAN (switch) connects to router, router connects to ISP via cable
- What does the interent represent?
  - Structure that connect all LAN's all over the world
  - home router is a combo device that combines a router and a switch
    - Most home routers also have an access point which allows LAN devices to use WiFi
  - Distributed router structure
  - Routing table: created by a processor inside the router. Used to determine which path (port) to forward the packet to
- The internet is the 'Netowrk of Networks'
- Connecting to the internet from the computer's perspective
  - Need to use the router feature of a Home-Router (don't need the switch part for this)
  - Servers, computers with more powerful hardware for handling packet transmission from much more traffic than your personal PC
