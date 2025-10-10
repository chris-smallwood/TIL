# Place to take notes daily

## End day by transcribing notes from here to specific documents. Goal of reinforcing learning and organization.

### EXP - Present

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
  - 


### Code Review
#### https://github.com/

Regex
- `^` means start of a string
- `[a-z]` matches any lowercase english letter
- `+` means one or more characters required
- `$` means end of string
- `/.../` JS/TS regex literal, wrap any regex in this when writing JS/TS
  - Optional flags go after second `/` e.g. adding `/.../i` would be case insensitive
- All together `/^[a-z]+$/` means lowercase alphabet only min 1


#### Pagination Utility

   
### Brandon Pairing

- checkout tsconfig.json
- parse vs safeParsej
- types vs interfaces

- TS Result ```ts-resuls-es``` for implementing step result functionality

- Usecase should never be importing anything from the repository, clean architecture
  - usecase should define the type of repo IT needs and then the repo type (defined in repo layer) should implimit that
  - define our repo interfaces in the usecase, do not import from repo to usecase
  - implement repo to meet the interface defined in the usecase
  - interface has advantage over type here when defining repo needed by usecase, look into it
 
Brandon's last minute DDD domain/use-case process meeting
- 45 max is not used anywhere in backend as of yet

### Wataru Pairing

- Module to module communication
  - only through service layer (use case)
  - type declarations are an exception
  - 



### Wataru Pairing

