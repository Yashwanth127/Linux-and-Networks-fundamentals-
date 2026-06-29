# Week 4 - Advanced Process Management & Networking Fundamentals

## Overview

This week focused on Linux process management and core networking concepts. The goal was to understand how Linux manages running processes and how devices communicate over a network.

---

## Process Management

### Topics Covered

* Process Basics
* Process Priority
* nice
* renice
* Background Jobs
* Foreground Jobs
* jobs
* bg
* fg
* nohup

### Practical Commands

```bash
sleep 300 &
jobs
fg %1

sleep 300
# Press Ctrl + Z

bg

nice -n 10 sleep 300

ps aux | grep sleep

renice 10 -p PID

nohup sleep 300 &
```

### Key Learning

* A process is a running program.
* Linux assigns CPU time based on process priority.
* `nice` starts a process with a specified priority.
* `renice` changes the priority of an already running process.
* `jobs` displays background jobs in the current shell.
* `bg` resumes a stopped job in the background.
* `fg` brings a background job to the foreground.
* `nohup` keeps a process running after logging out.

---

## Networking Fundamentals

### Topics Covered

* Networking Basics
* IP Address
* IPv4 vs IPv6
* Public vs Private IP
* Subnet Mask
* Default Gateway
* DNS (Domain Name System)
* TCP vs UDP
* OSI Model
* Network Types
* Network Devices
* Network Topologies

### Practical Commands

```bash
ip a
hostname -I
ip route
cat /etc/resolv.conf
nslookup google.com
ping google.com
```

### Key Learning

* Every device on a network has an IP address.
* Public IP addresses are used on the Internet, while Private IP addresses are used within local networks.
* A Subnet Mask separates the network and host portions of an IP address.
* A Default Gateway forwards traffic to other networks.
* DNS converts domain names into IP addresses.
* TCP provides reliable communication, while UDP prioritizes speed.
* The OSI Model explains how data moves through seven layers during network communication.

---

## Repository Contents

* README.md
* Theory Notes
* Practical Command Screenshots
* Networking Notes
* Process Management Notes

---

## Outcome

After completing this week, I can:

* Manage Linux processes using nice, renice, jobs, bg, fg and nohup.
* Understand foreground and background processes.
* Identify IP addressing concepts.
* Explain Public and Private IP addresses.
* Understand Subnet Masks and Default Gateways.
* Explain how DNS works.
* Differentiate between TCP and UDP.
* Describe the seven layers of the OSI Model.

---

