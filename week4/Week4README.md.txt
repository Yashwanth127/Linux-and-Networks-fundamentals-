# Week 4 - Advanced Process Management & Networking Basics

## Process Management

### nice
- Start a process with lower priority

```bash
nice -n 10 sleep 300
```

### renice
- Change priority of a running process

```bash
sleep 300 &
ps aux | grep sleep
renice 10 -p PID
```

### Background Jobs

```bash
sleep 300 &
jobs
```

### Foreground Jobs

```bash
fg %1
```

### Background a Stopped Job

```bash
sleep 300
```

Press:

```text
Ctrl + Z
```

Then:

```bash
bg
```

### nohup

```bash
nohup sleep 300 &
```

- Process continues even after logout

---

## Networking Basics

### IP Address

Commands:

```bash
ip a
hostname -I
```

Learn:
- What is an IP Address
- IPv4 vs IPv6

---

### Public vs Private IP

Private IP Ranges:

```text
10.0.0.0 - 10.255.255.255

172.16.0.0 - 172.31.255.255

192.168.0.0 - 192.168.255.255
```

Find Public IP:

```bash
curl ifconfig.me
```

---

### Subnet Mask

Examples:

```text
255.255.255.0
/24
```

Learn:
- Network Portion
- Host Portion

---

### Default Gateway

Command:

```bash
ip route
```

Learn:
- How devices communicate outside the local network

---

### DNS

Commands:

```bash
cat /etc/resolv.conf
nslookup google.com
```

Learn:
- DNS converts domain names into IP addresses

---

### TCP vs UDP

TCP:
- Reliable
- Connection Oriented
- Error Checking

Examples:
- SSH
- HTTP
- HTTPS

UDP:
- Faster
- Connectionless
- No Delivery Guarantee

Examples:
- DNS
- Streaming
- Video Calls

---

### OSI Model

```text
7 - Application
6 - Presentation
5 - Session
4 - Transport
3 - Network
2 - Data Link
1 - Physical
```

Mnemonic:

```text
All People Seem To Need Data Processing
```

---

## Week 4 Outcome

By the end of Week 4 I should be able to:

- Manage process priorities using nice and renice
- Run and manage background jobs
- Use fg, bg and jobs commands
- Understand nohup usage
- Explain IP Address concepts
- Differentiate Public and Private IPs
- Understand Subnet Masks
- Explain Default Gateway
- Understand DNS basics
- Explain TCP vs UDP
- Explain the OSI Model in interviews

## Git Commit

```bash
git add .
git commit -m "Week 4 - Process Management and Networking Basics"
git push
```