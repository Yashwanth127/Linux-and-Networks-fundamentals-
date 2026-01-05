Network Fundamentals

Networking is the practice of connecting computers and devices so they can communicate and share data. It is the foundation of cloud computing, DevOps, cybersecurity, and modern applications.

Network Types

PAN (Personal Area Network)
A small network used for personal devices. Example: Bluetooth connection between a mobile phone and headset.

LAN (Local Area Network)
A network within a small area such as a home, office, or school. Ethernet and Wi-Fi are commonly used.

MAN (Metropolitan Area Network)
A network that covers a city or large campus. It connects multiple LANs together.

WAN (Wide Area Network)
A network that spans a large geographical area. The Internet is the best example of a WAN.

VLAN (Virtual LAN)
A logical network created inside a physical network. Used to improve security and network management.

SAN (Storage Area Network)
A high-speed network that connects servers to storage devices and provides block-level data access.

Network Topologies

Bus Topology
All devices are connected to a single cable. Easy to set up but a cable failure breaks the entire network.

Star Topology
All devices are connected to a central switch or hub. Easy to manage, but the central device is a single point of failure.

Ring Topology
Devices are connected in a circular manner. Data travels in one direction. Failure of one device can disrupt the network.

Mesh Topology
Each device is connected to multiple devices. Very reliable but expensive to implement.

Tree Topology
A hierarchical structure that combines bus and star topology.

Hybrid Topology
A combination of two or more network topologies.

Key Networking Devices

Hub
A basic device that sends data to all connected devices. Works at the Physical Layer.

Switch
Forwards data only to the intended device using MAC addresses. Works at the Data Link Layer.

Router
Connects different networks and forwards data using IP addresses. Works at the Network Layer.

Firewall
A security device that allows or blocks network traffic based on rules. Can work at multiple layers.

Wireless Access Point
Allows wireless devices to connect to a wired network.

Load Balancer
Distributes network traffic across multiple servers to improve performance and availability.

OSI Model Layers

Layer 7 – Application
Provides services to applications like HTTP, FTP, SMTP.

Layer 6 – Presentation
Handles data formatting, encryption, and decryption.

Layer 5 – Session
Manages communication sessions between systems.

Layer 4 – Transport
Ensures data delivery using TCP or UDP.

Layer 3 – Network
Handles routing and logical addressing using IP.

Layer 2 – Data Link
Handles MAC addressing and error-free data transfer.

Layer 1 – Physical
Defines physical components like cables and signals.

TCP/IP Model Layers

Application Layer
Handles protocols like HTTP, HTTPS, DNS, SMTP.

Transport Layer
Uses TCP or UDP for data delivery.

Internet Layer
Handles IP addressing and routing.

Network Access Layer
Handles physical data transmission such as Ethernet and Wi-Fi.

IP Addressing

An IP address is a unique identifier assigned to a device on a network.

IP Classes
Class A: 1.0.0.0 – 126.0.0.0
Class B: 128.0.0.0 – 191.255.0.0
Class C: 192.0.0.0 – 223.255.255.0
Class D: Used for multicast
Class E: Reserved for experimental use

Private IP Ranges
10.0.0.0 – 10.255.255.255
172.16.0.0 – 172.31.255.255
192.168.0.0 – 192.168.255.255

Private IPs are not accessible on the public internet.

Subnetting Basics

Subnet Mask
A value that separates the network and host portion of an IP address.

CIDR Notation
Represents subnet mask using /n format. Example: /24 means 255.255.255.0.

Subnetting
The process of dividing a network into smaller networks for better management and security.

Transport Layer Protocols

TCP (Transmission Control Protocol)
Connection-oriented, reliable, and ordered data transfer. Used by HTTP, FTP, SMTP.

UDP (User Datagram Protocol)
Connectionless, faster, but unreliable. Used by DNS, VoIP, streaming services.

Application Layer Protocols

HTTP
Transfers web data. Uses port 80.

HTTPS
Secure version of HTTP using encryption. Uses port 443.

DNS
Resolves domain names to IP addresses. Uses port 53.

SMTP
Used for sending emails. Uses port 25.

POP3
Used for receiving emails. Uses port 110.

IMAP
Used for managing emails on the server. Uses port 143.

FTP
Transfers files between systems. Uses ports 20 and 21.

SSH
Provides secure remote access to systems. Uses port 22.
