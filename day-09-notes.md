# Day 9 – Connect and Protect: Networks and Network Security
📅 Date: 2025-09-08
🎯 Focus: Network Operations

---

## 📘 Concepts Learned

- Network Protocols. A set of rules used by two or more devices on a network to describe the order of delivery and the structure of the data.

- Transmission Control Protocol (TCP). An internet communications protocol that allows devices to form a connection and stream data.

- Address Resolution Protocol. A network protocol used to determine the MAC address of the next router or device on the path.

- HyperText Transfer Protocol Secure (HTTPS). A network protocol that provides a secure method of communication between clients and website servers.

- Domain Name System (DNS). A network protocol that translates internet domain names into IP addresses.

- User Datagram Protocol (UDP). A connectionless protocol that does not establish a connection between devices before a transmission. This makes it less reliable that TCP. But that also means that it works well for transmissions that need to get to their destination quickly.

- Three types of network protocols (3 main there are many more)
  - Communication Protocols
    - Transmission Control Protocol (TCP) is an internet communication protocol that allows two devices to form a connection and stream data. TCP uses a three-way handshake process. First, the device sends a synchronize (SYN) request to a server. Then the servers responds with a SYN/ACK packet to acknowledge receipt of the device's request. Once the server receives the final ACK packet from the device, A TCP connection is established. In teh TCP/IP model, TCP occurs at the transport layer.

    - User Datagram Protocol (UDP) is a connectionless protocol that does not establish a connection between devices before a transmission. This makes it less reliable than TCP. But it also means that it works well for transmissions that need to get to their destinations quickly. For example, one use for UDP is for sending DNS requests to local DNS servers. In the TCP/IP model, UDP occurs at the transport layer.

    - Hypertext Transfer Protocol (HTTP) is an application layer protocol that provides a method of communication between clients and website servers. HTTP uses port 80. HTTP is considered insecure, so it is being replaced on most websites by a secure version, called HTTPS that uses encryption from SSL/TLS for communication. However, there are still many websites that use the insecure HTTP protocol. In the TCP/IP model, HTTP occurs at the application layer.

    - Domain Name System (DNS) is a protocol that translates internet domain names into IP addresses. When a client computer wishes to access a website domain using their internet browser, a query is sent to a dedicated DNS server. The DNS server then looks up the IP address that corresponds to the website domain. DNS normally uses UDP on port 53. However, if the DNS reply to a request is large, it will switch to using the TCP protocol. In the TCP/IP model, DNS occurs at the application layer.

  - Management Protocols
    - Simple Network Management Protocol (SNMP) is a network protocol used for monitoring and managing devices on a network. SNMP can reset a password on a network device or change its baseline configuration. It can also send requests to network devices for a report on how much of the network's bandwidth is being used up. In the TCP/IP model, SNMP occurs at the application layer.

    - Internet Control Message Protocol (ICMP) is an internet protocol used by devices to tell each other about data transmission errors across the network. ICMP is used by a receiving device to send a report to the sending device about the data transmission. ICMP is commonly used as a quick way to troubleshoot network connectivity and latency bu issuing the "ping" command on a Linux operating system. In the TCP/IP model, ICMP occurs at the internet layer.

  - Security Protocols
    - Hypertext Transfer Protocol Secure (HTTPS) is a network protocol that provides a secure method of communication between clients and website servers. HTTPS is a secure version of HTTP that uses secure sockets layer/transport layer security (SSL/TLS) encryption on all transmissions so that malicious actors cannot read the information contained. HTTPS uses port 443. In the TCP/IP model, HTTPS occurs at the application layer.

    - Secure File Transfer Protocol (SFTP) is a secure protocol used to transfer files from one device to another over a network. SFTP uses secure shell (SSH), typically through TCP port 22. SSH uses Advanced Encryption Standard (AES) and other types of encryption to ensure that unintended recipients cannot intercept the transmissions. In the TCP/IP model, SFTP occurs at the application layer. SFTP is often used with cloud storage. Every time a user uploads or downloads a file from cloud storage, the file is transferred using the SFTP protocol.

  - Network Address Translation. Devices on your local home or office networks each have a private IP address that they use to communicate directly with each other. However, in order for the devices with private IP address to communicate with the public internet, they need to have a single public IP address that represents all devices on the LAN to the public. For outgoing messages, the router can replace a private source IP address with its public IP address and perform the reserve operation for responses. This process is known as Network Address Translation (NAT) and it generally requires a router or firewall to be specifically configured to perform NAT. NAT is part of layer 2 (internet layer) and layer 3 (transport layer) of the TCP/IP model.

  - Dynamic Host Configuration Protocol. is in the management family of network protocols. DHCP is an application protocol used on a network to configure devices. It works with the router to assign a unique IP address to each device and provide the addresses of the appropriate DNS server and default gateway for each device. DHCP servers operate on UDP port 67 while DHCP client operate on UDP port 68.

  - Address Resolution Protocol. ARP is mainly a network access layer protocol in the TCP/IP model used to translate the IP addresses that are found in data packets into the MAC address of the hardware device.

  - Telnet is an application layer protocol that is used to connect with a remote system. Telnet sends all information in clear text. It uses command line prompts to control another device similar to secure shell (SSH), but Telnet ius not as secure as SSH. Telnet can be used to connect to local or remote devices and uses TCP port 23.

  - Secure Shell protocol (SSH) is used to create a secure connection with a remote system. This application layer protocol provides an alternative for secure authentication and encrypted communication. SSH operates over the TCP port 22 and is a replacement for less secure protocols, such as Telnet.

  - Post office Protocol (PO) is an application layer (layer 4 of the TCP/IP model) protocol used to manage and retrieve email from a mail server. POP3 is the most commonly used version of POP.

  - Internet Message Access Protocol (IMAP) is used for incoming email. It downloads the headers of emails and the message content. The content also remains on the email server, which allowed users to access their email from multiple devices. IMAP uses TCP port 143 for unencrypted email and TCP port 993 over the TLS protocol.

  - Simple Mail Transfer Protocol is used to transmit and route email from the sender to the recipient's address. SMTP works with Message Transfer Agent (MTA) software, which searches DNS servers to resolve email addresses to IP addresses, to ensure emails reach their intended destination. SMTP uses TCP/UDP port 25 for unencrypted emails and TCP/UDP port 587 using TLS for encrypted emails. The TCP port 25 is often used by high-volume spam. SMTP helps to filter out spam by regulating how many emails a source can send at a time.

  - Protocols and Port numbers. Port numbers are used by network devices to determine what should be done with the information contained in each data packet once they reach their destination. Firewalls can filter out unwanted traffic based on port numbers.

- Wireless Protocols

  - IEEE 802.11 (WiFi) is a set of standards that define communication for wireless LANs.
  - IEEE stands for the Institute of Electrical and Electronics Engineers, which is an organization that maintains WiFi standards, and 802.11 is a suite of protocols used in wireless communications.
  - WiFi Protected Access (WPA) is a wireless security protocol for devices to connect to the internet.

  - Wired Equivalent Privacy (WEP)is a wireless security protocol designed to provide users with the same level of privacy on wireless network communications as they have on wired network connections. WEP is largely out os use today. This is considered a high risk security protocol.

  - Wi-Fi Protected Access (WPA) was developed in 2003 to improve upon WEP, address the security issues that it presented, and replace it. Despite the security improvement of WPA, it still have vulnerabilities.

  - WPA2 & WPA3. Because of the strength of WPA2, it is considered the security standard for all Wi-Fi transmissions today. It is best used for personal home networks. WPA2 enterprise mode works best for business applications. WPA3 is a secure Wi-Fi protocol and is growing in usage as more WPA3 compatible devices are released.

- Firewall is a network security device that monitors traffic to and from your network.
  - Port Filtering. A firewall can use port filtering, which blocks or allows certain port numbers to limited unwanted communication.
  - Stateful is a class of firewall that keeps track of information passing through it and proactively filters out threats.
  - Stateless is a class of firewall that operates based on predefined rules and does not keep track of information from data packets.
  - Next Generation Firewall (NGFW) provides even more security than a stateful firewall. It performs more in depth security functions like deep packet inspection and intrusion protection.

- Virtual Private Networks (VPN) is a network security service that changes your public IP address and hides your virtual location so that you can keep your data private when you are using a public network like the internet.
  - Encapsulation is a process performed by a VPN service that protects your data by wrapping sensitive data in other data packets.

- Security Zone is a segment of a network that protects the internal network from the internet.
- Network Segmentation is a security technique that divides the network into segments.
- Uncontrolled Zones is any network outside of the organization's control.
- Controlled Zone is a subnet that protects the internal network from the uncontrolled zone.
  - Demilitarized zone (DMZ).
  - Internal network
  - Restricted zone

- Subnetting is the subdivision of a network into logical groups called subnets. It works like a network inside a network. Subnetting divides up a network address range into smaller subnets within the network. These smaller subnets form based on the IP addresses and network mask of the devices on the network. Subnetting creates a network of devices to function as their own network. This makes the network more efficient and can also be used to create security zones. If devices on the same subnet communicate with each other, the switch changes the transmissions to stay on the same subnet, improving speed and efficiency of the communications.

  - Classless Inter-Domain Routing notation for subnetting
    - CIDR is a method of assigning subnet masks to IP addresses to create a subnet. Classless addressing replaces classful addressing. CIDR allows cybersecurity professionals to segment classful networks into smaller chunks.

- Proxy Server is a server that fulfills the requests of a client by forwarding them on to other servers. The proxy server is a dedicated server that sits between the internet and the rest of the network. When a request to connect to the network comes in from the internet, the proxy server will determine if the connection request is safe.

  - Forward Proxy Server regulates and restricts a person's access to the internet.
  - Reverse Proxy Server regulates and restricts the internet's access to an internal server.
  - Email Proxy Server it filers spam email by verifying whether a sender's address was forged. This reduces the risk of phishing attacks that impersonate people known to the organization.


---

## 🛠 Commands / Tools Practiced

----------------------------------

🧠 Reflection

The protocols learned in this reading are basic networking protocols that entry-level cybersecurity analysts should know. Understanding how protocols function on a network is essential.

There is a lot to network security. It is a bit overwhelming but fun, something I want to make sure I do a deep dive into and continuously learn.

----------------------------------
