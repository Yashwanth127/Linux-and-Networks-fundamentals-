# Networking Commands and Troubleshooting

Networking commands are used to inspect network configuration, test connectivity, troubleshoot network problems, and monitor network activity.

---

## 1. Check IP Address

### `ip addr`

Displays the IP addresses assigned to network interfaces.

```bash
ip addr
```

Short form:

```bash
ip a
```

Example:

```text
inet 192.168.1.10/24
```

Here:

* `192.168.1.10` → IP address
* `/24` → CIDR notation
* `eth0` or `ens33` → Network interface

---

## 2. Check Network Interfaces

### `ip link`

Displays available network interfaces and their status.

```bash
ip link
```

Common interface states:

* `UP` → Interface is active
* `DOWN` → Interface is inactive

---

## 3. Check Routing Table

### `ip route`

Displays how packets are routed.

```bash
ip route
```

Example:

```text
default via 192.168.1.1 dev eth0
192.168.1.0/24 dev eth0
```

### Important Terms

* `default` → Default route for external networks
* `via` → Gateway
* `dev` → Network interface

---

## 4. Ping

The `ping` command tests whether a device is reachable over a network.

```bash
ping google.com
```

Or:

```bash
ping 8.8.8.8
```

Example:

```text
64 bytes from 8.8.8.8: icmp_seq=1 ttl=117 time=20 ms
```

### Important Information

* `time` → Response time
* `ttl` → Time To Live
* `icmp_seq` → Sequence number

Stop the command using:

```text
Ctrl + C
```

---

## 5. DNS Lookup

### `nslookup`

Used to find the IP address of a domain name.

```bash
nslookup google.com
```

### `dig`

Provides detailed DNS information.

```bash
dig google.com
```

To display only the IP address:

```bash
dig google.com +short
```

---

## 6. Trace Network Path

### `traceroute`

Shows the path packets take from your system to a destination.

```bash
traceroute google.com
```

On some systems:

```bash
tracepath google.com
```

This helps identify where network delays or failures occur.

---

## 7. Check Open Ports

### `ss`

Displays network connections and listening ports.

```bash
ss -tuln
```

Options:

* `t` → TCP
* `u` → UDP
* `l` → Listening ports
* `n` → Show numerical addresses

Example:

```text
LISTEN 0 128 0.0.0.0:22
```

This means SSH is listening on port `22`.

---

## 8. Check Active Connections

```bash
ss -tunap
```

This displays:

* TCP connections
* UDP connections
* Listening ports
* Process information

---

## 9. Test a Specific Port

### `nc` (Netcat)

Used to test whether a port is open.

```bash
nc -zv 192.168.1.1 22
```

Example output:

```text
Connection to 192.168.1.1 22 port [tcp/ssh] succeeded!
```

---

## 10. Check DNS Configuration

```bash
cat /etc/resolv.conf
```

This file contains DNS server information.

Example:

```text
nameserver 8.8.8.8
```

DNS servers convert domain names into IP addresses.

---

## 11. Hostname

### Check hostname

```bash
hostname
```

### Display detailed system information

```bash
hostnamectl
```

---

## 12. MAC Address

A MAC address is the physical address of a network interface.

```bash
ip link
```

Example:

```text
link/ether 00:0c:29:ab:cd:ef
```

---

# Basic Network Troubleshooting Process

When a network connection is not working, troubleshoot step by step.

## Step 1: Check the Network Interface

```bash
ip link
```

Check whether the interface is `UP`.

---

## Step 2: Check the IP Address

```bash
ip addr
```

Check whether the system has a valid IP address.

---

## Step 3: Test the Local Gateway

```bash
ping 192.168.1.1
```

If this fails, there may be a local network problem.

---

## Step 4: Test Internet Connectivity Using an IP

```bash
ping 8.8.8.8
```

If this works, internet connectivity is available.

---

## Step 5: Test DNS

```bash
ping google.com
```

If `8.8.8.8` works but `google.com` does not work, the problem may be DNS.

---

## Step 6: Check the Routing Table

```bash
ip route
```

Verify that a default gateway exists.

---

# Example Troubleshooting Flow

```text
Network Problem
      ↓
Check Interface
      ↓
Check IP Address
      ↓
Ping Gateway
      ↓
Ping Public IP
      ↓
Test DNS
      ↓
Check Open Ports
```

---

# Important Networking Terms

## Latency

The time taken for data to travel from one point to another.

Measured in:

```text
Milliseconds (ms)
```

Lower latency means faster communication.

---

## Bandwidth

The maximum amount of data that can be transferred over a network in a given time.

Example:

```text
100 Mbps
```

---

## Throughput

The actual amount of data successfully transferred.

Bandwidth is the maximum capacity, while throughput is the actual performance.

---

## Packet Loss

Occurs when network packets fail to reach their destination.

Packet loss can cause:

* Slow connections
* Video buffering
* Disconnections
* Poor online gaming performance

---

## Jitter

Variation in packet arrival time.

High jitter can affect:

* Voice calls
* Video calls
* Online gaming
* Real-time applications

---

# Useful Networking Commands Summary

| Command       | Purpose                      |
| ------------- | ---------------------------- |
| `ip addr`     | Display IP addresses         |
| `ip link`     | Display network interfaces   |
| `ip route`    | Display routing table        |
| `ping`        | Test connectivity            |
| `traceroute`  | Trace packet path            |
| `nslookup`    | Perform DNS lookup           |
| `dig`         | Detailed DNS information     |
| `ss`          | Display network connections  |
| `nc`          | Test ports and connections   |
| `hostname`    | Display system hostname      |
| `hostnamectl` | Display hostname information |

---

# Practical Lab

Run the following commands on Linux:

```bash
ip addr
ip link
ip route
ping -c 4 8.8.8.8
ping -c 4 google.com
nslookup google.com
dig google.com +short
ss -tuln
hostnamectl
```

## Questions to Answer

1. What is your system's IP address?
2. What is your network interface name?
3. What is your default gateway?
4. Which DNS server is being used?
5. Which ports are currently listening?
6. What is the latency to `8.8.8.8`?
7. Is there any packet loss?

---

# Key Takeaway

Understanding networking commands is essential for Linux administration, cloud computing, DevOps, and cybersecurity.

The basic troubleshooting process is:

```text
Interface → IP Address → Gateway → Internet → DNS → Ports
```
