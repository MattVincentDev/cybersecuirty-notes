# Day X – Connect and Protect: Networks and Network Security
📅 Date: 2025-09-01
🎯 Focus: Network Architecture

---

## 📘 Concepts Learned

- What is a network?
  - A group of connected devices.
  - Devices use unique addresses, or identifiers to locate each other. These addresses will ensure that communications happen with the right device. These are called IP and MAC addresses.

- Local Area Network (LAN)
  - A network that spans a small area like an office building, a school or a home.

- Wide Area Network (WAN)
  - A network that spans a large geographic area like a city, state, or country.

- Network Tools
  - HUB: A network device that broadcasts information to every device on the network.

  - SWITCH: A device that makes connections between specific devices on a network by sending and receiving data between them. A switch is more intelligent than a hub. It only passes data to the intended destination. This makes switches more secure than hubs, and enables them to control the flow of traffic and improve network performance.

  - Router: A network device that connects multiple networks together.

  - Modem: A device that connects your router to the internet and brings internet access to the LAN.

  - Virtualization Tools: Pieces of software that perform network operations.They carry out operations that would normally be completed by a hub, switch, router, or modem, and they are offered by Cloud service providers.

  - Firewall: a network security device that monitors traffic to or from your network.

  - Servers: provide information and services for devices like computers, smart home devices, and smartphones on the network. The devices that connect to a server are called clients.

- Cloud Computing
  - The practice of using remote servers, applications, and network services that are hosted on the internet instead of on local physical devices.

- Cloud Network
  - Is a collection of servers or computers that stores resources and data in remote date centers that can be accessed via the internet.

- Computing processes in the cloud
  - Cloud service providers provide three main categories of services:
    - Software as a service (Saas) refers to software suites operated by the CSP that a company can use remotely without hosting the software.
    - Infrastructure as a service (Iaas) refers to the use of virtual computer components offered by the CSP.
    - Platform as a service (Paas) refers to tools that application developers can use to design custom applications for their company.

- Benefits of cloud computing and software defined networks.
  - Reliability
  - Cost
  - Scalability

- Data Packet
  - A basic unit of information that travels from one device to another within a network.
  - A Data Packet contains:
    - Header: IP address / MAC address / Protocol Number
    - Body: contains the message
    - Footer: the footer signals to the receiving device that the packet is finished.

  - Bandwidth is the amount of data a device receives every second.
  - Speed is the rate at which data packets are received or downloaded.
  - Packet Sniffing is the practice of capturing and inspecting data packets across a network.

- The TCP/IP Model (Transmission Control Protocol and Internet Protocol)
  - TCP/IP is the standard model used for network communication.
  - TCP is an internet communication protocol that allows two devices to form a connection and stream data. It also establishes a connection between two devices and makes sure that packets reach their appropriate destination.
  - IP is a set of standards used for routing and addressing data packets as they travel between devices on a network.
  - Port is a software based location that organizes the sending and receiving of data between devices on a network. Ports divide network traffic into segments based on the services they will perform between two devices. The computers sending and receiving these data segments know how to prioritize and process these segments based on their port number.
    - Common Port Numbers
      - Port 25 - Email
      - Port 443 - Secure internet communication
      - Port 20 - Large file transfers.

- TCP/IP model is a framework used to visualize how date is organized and transmitted across the network. The TCP/IP model has 4 layers:
  - Network access layer. Deals with creation of data packets and their transmission across a network. This include hardware devices connected to physical cables and switches that direct data to its destination.

  - Internet layer. This is where IP addresses are attached to data packets to indicate the location of the sender and receiver. The internet layer also focuses on how networks connect to each other.
    - Internet Protocol. IP sends the data packets to the correct destination and relies on the Transmission Control Protocol/User Datagram Protocol (TCP/UDP) to deliver them to the corresponding service.
    - Internet Control Message Protocol (ICMP). The ICMP shares error information and status updates of data packets. This is useful for detecting and troubleshooting network errors.

  - Transport layer. This includes protocols to control the flow of traffic across a network. These protocols permit or deny communication with other devices and include information about the status of the connection.
    - Transmission Control Protocol is an internet communication protocol that allows two devices to form a connection and stream data. It ensures that data is reliably transmitted to the destination service. TCP contains the port number of the intended destination service, which resides in the TCP header of the TCP/IP packet.
    - User Datagram Protocol is a connectionless protocol that does not establish a connection between devices before transmissions. It is used by applications that are not concerned with the reliability of the transmission. Data sent over the UDP is not tracked as extensively as data sent using TCP. Because UDP does not establish network connections, it is used mostly for performance sensitive applications that operate in real time, such as video streaming.

  - Application layer. Protocols determine how the data packets will interact with receiving devices. This layer is responsible for making network requests or responding to requests. This layer defines which internet services and applications any user can access. Protocols in this application layer determine how the data packets will interact with receiving devices. Some common protocols used on this layer are:
    - Hypertext Transfer Protocol (HTTP)
    - Simple Mail Transfer Protocol (SMTP)
    - Secure Shell (SSH)
    - File Transfer Protocol (FTP)
    - Domain Name System (DNS)

- The OSI Model. This has 7 layers.
  - Physical
    - The physical layer corresponds to the physical hardware involved in network transmission.

  - Data Link
    - The data link layer organizes sending and receiving data packets within a single network.

  - Network
    - The network layer oversees receiving the frames from the data link layer (layer 2) and delivers them to the intended destination.

  - Transport
    - The transport layer is responsible for delivering data between devices.

  - Session
    - A session describes when a connection is established between two devices.

  - Presentation
    - Functions at the presentation layer involve data translation and encryption for the network.

  - Application
    - The application layer includes processes that directly involve the everyday user. This layer includes all of the networking protocols that software applications use to connect a user to the internet.

- IP address is a unique string of characters that identifies the location of a device on the internet.
  - IP Version 4 (IPv4)
  - IP Version 6 (IPv6)

- MAC address is a unique alphanumeric identifier that is assigned to each physical device on a network.


---

🧠 Reflection

Once you have that fundamental level of skills and fundamental level of background, there are so many different directions you can go, there is so much opportunity out there.

----------------------------------
