# Linux Learning Roadmap 🚀

This repository contains my complete Linux learning journey from fundamentals to scripting, automation, and real-world Linux administration.

The goal of this roadmap is not just to memorize commands, but to actually understand how Linux works internally through daily practice, troubleshooting, and hands-on usage.

---

# 📅 Week 1 — Linux Fundamentals

Goal:
Build strong basics and become comfortable using the Linux terminal.

---

## Day 1 — Navigation & File System Basics

Learned:

* Linux filesystem structure
* directories and paths
* basic navigation commands

Commands:

```bash
pwd
ls
cd
mkdir
rmdir
clear
tree
```

Concepts:

* absolute vs relative paths
* important Linux directories:

  * `/home`
  * `/etc`
  * `/var`
  * `/bin`
  * `/root`

Practice:

* creating folders
* navigating directories
* understanding filesystem hierarchy

---

## Day 2 — File Operations

Learned:

* creating, editing, copying, moving, and deleting files

Commands:

```bash
touch
cp
mv
rm
cat
nano
```

Practice:

* creating notes
* editing files
* renaming files
* copying directories

Important Understanding:
In Linux, almost everything is treated as a file.

---

## Day 3 — Networking Fundamentals

Learned:

* basic networking concepts
* IP addresses
* local and remote communication

Commands:

```bash
ip a
ping
ifconfig
netstat
ss
curl
wget
```

Practice:

* checking IP address
* testing internet connectivity
* downloading files from terminal

Concepts:

* localhost
* packets
* ports
* interfaces

---

## Day 4 — Users, Permissions & Processes

Learned:

* Linux users and permissions
* process management basics

Commands:

```bash
whoami
sudo
chmod
chown
ps
top
kill
```

Concepts:

* root user
* permissions (`rwx`)
* ownership
* PID (Process ID)

Practice:

* modifying permissions
* checking running processes
* stopping processes

---

## Day 5 — Text Processing

Learned:

* filtering and manipulating text in terminal

Commands:

```bash
grep
awk
sed
sort
cut
head
tail
```

Practice:

* searching logs
* filtering output
* extracting specific text

---

# 📅 Week 2 — Bash Scripting Basics

Goal:
Understand shell scripting and basic automation.

---

## Topics Covered

### Variables

```bash
name="Linux"
echo $name
```

### Conditions

```bash
if [ condition ]
then
  echo "True"
fi
```

### Loops

```bash
for i in 1 2 3
do
  echo $i
done
```

### User Input

```bash
read name
echo $name
```

### Bash Script Basics

```bash
#!/bin/bash
```

Practice:

* greeting scripts
* simple calculator
* loops and conditions
* file checking scripts

Goal:
Write small automation scripts confidently.

---

# 📅 Week 3 — Linux Administration & Automation

Goal:
Learn practical Linux administration and monitoring.

---

## 1. Processes & Process Management

Learned:

* what a process is
* process monitoring
* stopping processes

Commands:

```bash
ps aux
top
htop
kill
kill -9
```

Concepts:

* PID (Process ID)
* CPU usage
* memory usage
* foreground vs background processes

Practice:

* monitoring processes
* killing frozen applications
* understanding system resource usage

---

## 2. systemctl & Linux Services

Learned:

* Linux services and daemons
* managing background services

Commands:

```bash
systemctl status ssh
sudo systemctl start ssh
sudo systemctl stop ssh
sudo systemctl restart ssh
sudo systemctl enable ssh
```

Concepts:

* services
* daemons
* background processes
* startup services

---

## 3. SSH Basics

Learned:

* secure remote login
* SSH authentication basics

Commands:

```bash
ssh user@ip-address
ssh localhost
```

Practice:

* local SSH connection
* understanding remote access

---

## 4. Cron Jobs

Learned:

* task scheduling
* automation using cron

Commands:

```bash
crontab -e
crontab -l
```

Example:

```bash
* * * * * echo "Hello" >> test.txt
```

Concepts:

* minute
* hour
* day
* scheduled automation

---

## 5. Logs & Monitoring

Learned:

* system logs
* live monitoring

Commands:

```bash
journalctl
dmesg
tail -f file.txt
```

Practice:

* monitoring logs in real time
* troubleshooting errors

---

## 6. Environment Variables

Learned:

* shell variables
* environment variables

Commands:

```bash
echo $HOME
echo $PATH
env
```

Variables:

```bash
name="Linux"
echo $name
```

---

## 7. Disk Usage & Memory Monitoring

Learned:

* storage monitoring
* memory usage checking

Commands:

```bash
df -h
du -sh *
free -h
```

Concepts:

* disk space
* RAM usage
* filesystem storage

---

## 8. More Bash Practice

Practice:

* loops
* variables
* conditions
* executable scripts

Example:

```bash
#!/bin/bash

name="Linux"

if [ $name = "Linux" ]
then
 echo "Correct"
fi
```

---

# 📅 Week 4 — Projects & Interview Preparation

Goal:
Apply Linux knowledge through mini-projects and interview practice.

---

## Projects

### 1. System Monitoring Script

Monitor:

* CPU usage
* RAM usage
* disk space

### 2. Backup Automation Script

Automatically:

* create backups
* organize files
* use timestamps

### 3. Log Analyzer

Analyze logs using:

```bash
grep
awk
sed
```

### 4. Cron Automation

Automate:

* backups
* cleanup tasks
* scheduled scripts

---

# 🎯 Final Goal

By completing this roadmap, I should be able to:

* navigate Linux comfortably
* manage files and directories
* understand Linux networking basics
* manage users and permissions
* monitor and control processes
* manage Linux services
* use SSH confidently
* automate tasks using cron
* analyze logs
* write Bash scripts
* troubleshoot common Linux issues


