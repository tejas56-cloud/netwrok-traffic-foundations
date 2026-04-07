The TCP/IP Model is the real-world networking model used on the internet, while the OSI Model is a conceptual framework used for understanding.

the osi model has 7 layers (theorotical)

the tcp/ip mdoel has 4 layers(real practical world internet)

# 1. mapping tcp/ip vs osi 

|   TCP/IP Layer     |   OSI Layers Covered     |         What It Does                        |
|--------------------|--------------------------|---------------------------------------------|
| Application        | 7, 6, 5                  | User interaction, data formatting, sessions |
| Transport          | 4                        | End-to-end communication (TCP/UDP)          |
| Internet           | 3                        | Routing using IP addresses                  |
| Network Access     | 2, 1                     | Local delivery + physical transmission      |


## 2. key protocols in each layer

|     Layer        |     Protocols         |
|------------------|-----------------------|
| Application      | HTTP, HTTPS, DNS, FTP |
| Transport        | TCP, UDP              |
| Internet         | IP                    |
| Network Access   | Ethernet, WiFi        |

### 3. client to server flow

# step 1- application layer
user(client) types (eg- google.com) in the browser,

then-
Browser creates an HTTP request,

DNS resolves domain → IP address

# step 2 - transport layer(tcp)
the tcp establishes conenction using tcp handshake-
1. Client → SYN (request to connect)
2. Server → SYN-ACK (acknowledge)
3. Client → ACK (connection established)
now connection is eastblished and communication becomes reliable

# step 3 - internet layer (ip)
data is wrapped into packet

with attached source ip = users ip

and destination ip=servers ip

Routers use this to decide path across networks.

# step 4 - Network Access Layer
here packet is wrapped into frmae 

and it Uses MAC addresses for local delivery

Example:
Laptop -> Router -> ISP

Each hop changes MAC address, but IP stays same.

# step 5 - physical transmission 

data converted into bits(0s and 1s)

then send via-

ethernet

wifi cable

fiber optics

# 4 - at server side  descpasulation happens teh reverse process of sender 
1. Physical - receives bits  
2. Data Link - checks MAC  
3. Internet - checks IP  
4. Transport - reassembles data  
5. Application - processes request

Server then sends response back using same process.





