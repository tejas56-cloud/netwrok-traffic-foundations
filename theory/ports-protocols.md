# what is port -
The PORT is the logical gate (entry/exit point) on a device that decides which application sends or recieves data 

# TCP VS UDP 
core difference -

TRANSIMISSION CONTROL PROTOCOL (TCP)-

-Its reliable,connection-based

-Used when data must arrive correctly 

USER DATAGRAM PROTOCOL(UDP)

-Fast , connectionless

-Used when speed matters more than accuracy 

TCP IS USED FOR-

Websites(HTTP/HTTPS)

Login systems

File transfers


UDP IS USED FOR-

streaming

gaming

dns queires

# TCP = Reliability , UDP = Speed

# 20 Critical Ports -

| Port    | Protocol | Used For             | Security Relevance        |
| ------- | -------- | -------------------- | ------------------------- |
| 20/21   | FTP      | File transfer        | Unencrypted, vulnerable   |
| 22      | SSH      | Secure remote login  | Brute-force target        |
| 23      | Telnet   | Remote login         | Insecure (no encryption)  |
| 25      | SMTP     | Email sending        | Spam abuse                |
| 53      | DNS      | Domain resolution    | DNS attacks/amplification |
| 67/68   | DHCP     | IP assignment        | Network spoofing risk     |
| 69      | TFTP     | Simple file transfer | No security               |
| 80      | HTTP     | Web traffic          | No encryption             |
| 110     | POP3     | Email retrieval      | Credentials exposed       |
| 119     | NNTP     | News transfer        | Rare but exploitable      |
| 123     | NTP      | Time sync            | DDoS amplification        |
| 137-139 | NetBIOS  | Windows networking   | Enumeration risk          |
| 143     | IMAP     | Email retrieval      | Needs encryption          |
| 161     | SNMP     | Network management   | Info leakage              |
| 179     | BGP      | Routing protocol     | Internet-level attacks    |
| 389     | LDAP     | Directory services   | Sensitive data exposure   |
| 443     | HTTPS    | Secure web           | Main attack surface       |
| 445     | SMB      | File sharing         | WannaCry-type attacks     |
| 3389    | RDP      | Remote desktop       | Bruteforce, exploits      |
| 8080    | HTTP-alt | Web alternative      | Misconfigured services    |


# Ports define how services communicate on a system, while protocols like TCP and UDP determine how data is transmitted. Understanding common ports and their security risks is critical for network analysis and cybersecurity.

