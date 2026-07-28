# Networking Revision Notes

## Overview

Today I revised the fundamentals of networking by practicing packet analysis using Wireshark on Kali Linux. The goal was to understand how devices communicate over a network and how different protocols appear in live traffic.

---

# Tools Used

* Kali Linux
* VMware Workstation 17 Player
* Wireshark

---

# Topics Revised

## 1. Packet Capture

* Started a live capture on the `eth0` interface.
* Observed incoming and outgoing network traffic.
* Learned how packet capture works in real time.

---

## 2. Display Filters

Used the following filter:

```text
ip.dst == 151.101.129.91
```

This filter displays only packets whose destination IP address matches the specified IP.

---

## 3. Protocols Observed

### TCP (Transmission Control Protocol)

* Connection-oriented protocol
* Reliable data delivery
* Uses Sequence Numbers and ACKs
* Commonly used for HTTP, HTTPS, SSH, FTP

---

### TLS (Transport Layer Security)

* Encrypts communication between client and server.
* Protects sensitive information.
* Commonly runs over TCP port 443.

---

### ARP (Address Resolution Protocol)

* Maps IP addresses to MAC addresses.
* Used inside the local network.
* Required before devices communicate over Ethernet.

---

### ICMPv6

* Used in IPv6 networks.
* Helps with network discovery.
* Router Solicitation packets help devices locate routers.

---

# Wireshark Fields Reviewed

* Source IP
* Destination IP
* Source Port
* Destination Port
* Protocol
* Packet Length
* Sequence Number
* Acknowledgement Number
* Packet Information

---

# What I Learned

* How to capture live network traffic.
* How to apply display filters.
* Difference between TCP and TLS.
* Purpose of ARP.
* Basic understanding of ICMPv6.
* How to inspect packet details.

---

# Key Networking Concepts

### IP Address

Identifies a device on a network.

### MAC Address

Unique hardware address of a network interface.

### Port

Logical communication endpoint.

Examples:

* 22 → SSH
* 53 → DNS
* 80 → HTTP
* 443 → HTTPS

---

# Commands Worth Remembering

```bash
ip a
```

Shows network interfaces.

```bash
ping google.com
```

Checks network connectivity.

```bash
traceroute google.com
```

Shows the path packets take.

```bash
netstat -tulnp
```

Displays listening ports.

```bash
ss -tulnp
```

Modern replacement for netstat.

---

# Today's Practice

✔ Installed and used Wireshark

✔ Captured live packets

✔ Applied display filters

✔ Observed TCP, TLS, ARP and ICMPv6 traffic

✔ Reviewed packet details

---

# Next Topics to Practice

* DNS Packet Analysis
* TCP Three-Way Handshake
* UDP vs TCP
* HTTP vs HTTPS
* DHCP
* NAT
* VLAN Basics
* Linux Networking Commands
* SSH Packet Capture
* ICMP Analysis
* Firewall Basics (iptables / ufw)
* Cloud Networking Basics (AWS VPC)

---

## Revision Summary

Today's practice improved my understanding of packet capture, protocol analysis, and Wireshark filtering. This revision strengthened my networking fundamentals and prepared me for more advanced topics such as DNS, routing, cloud networking, and network security.
