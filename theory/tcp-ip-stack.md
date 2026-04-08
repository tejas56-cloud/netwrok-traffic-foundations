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


### 3. CLIENT TO SERVER FLOW.

# Step 1- Application layer
user(client) types (eg- google.com) in the browser,

then-
Browser creates an HTTP request,

DNS resolves domain → IP address

# Step 2 - Transport layer(tcp)
the tcp establishes conenction using tcp handshake-
1. Client → SYN (request to connect)
2. Server → SYN-ACK (acknowledge)
3. Client → ACK (connection established)
now connection is eastblished and communication becomes reliable

# Step 3 - Internet layer (ip)
data is wrapped into packet

with attached source ip = users ip

and destination ip=servers ip

Routers use this to decide path across networks.

# Step 4 - Network Access Layer
here packet is wrapped into frmae 

and it Uses MAC addresses for local delivery

Example:
Laptop -> Router -> ISP

Each hop changes MAC address, but IP stays same.

# Step 5 - Physical transmission 

data converted into bits(0s and 1s)

then send via-

ethernet

wifi cable

fiber optics

# 4 - At server side  decapsulation happens the reverse process of sender 
1. Physical - receives bits  
2. Data Link - checks MAC  
3. Internet - checks IP  
4. Transport - reassembles data  
5. Application - processes request

Server then sends response back using same process.

# 5. TCP VS UDP

|   Feature   |    TCP     |      UDP            |
|-------------|------------|---------------------|
| Connection  | Yes        | No                  |
| Reliability | Guaranteed | Not guaranteed      |
| Speed       | Slower     | Faster              |
| Use Case    | HTTPS, login | Streaming, gaming |


# 6. Key concepts to remeber 

1.ENCAPSULATION - Each layer adds its own header

2.Packet - Data + IP (layer 3)

3.Frame - Packet + MAC (layer 2)

4.TCP - Reliable copmmunication

5.UDP - Fast, no guarantee

6.IP - Handles routing across network 

# TCP/IP stack defines how data is created, transmitted, routed, delivered, and understood across networks.







