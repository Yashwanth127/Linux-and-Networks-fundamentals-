# Linux Process Management Practice (Day 1)

## Overview

Today I practiced the fundamentals of Linux process management on Ubuntu. The goal was to understand how Linux creates, manages, monitors, and terminates processes using commonly used command-line utilities.

---

## Topics Covered

- What is a Process?
- Process ID (PID)
- Parent Process ID (PPID)
- Foreground vs Background Processes
- Process Signals
- Process Monitoring
- Job Control

---

## Commands Practiced

### Process Listing

```bash
ps
ps aux
```

Learned how to view currently running processes and understand process information such as:

- PID
- CPU Usage
- Memory Usage
- Running Command

---

### System Monitoring

```bash
top
```

Observed:

- CPU Usage
- Memory Usage
- Running Processes
- Process States

Exited using:

```text
q
```

---

### Finding Processes

```bash
pgrep firefox
pidof firefox
```

Used process names to find their corresponding Process IDs.

---

### Background Processes

Started a background process:

```bash
sleep 100 &
```

Verified running jobs:

```bash
jobs
```

---

### Foreground Process

Moved the background process back to the terminal.

```bash
fg
```

---

### Stopping a Process

Paused a running process using:

```text
Ctrl + Z
```

---

### Resuming a Background Process

```bash
bg
```

Continued the stopped process in the background.

---

### Terminating a Process

Stopped a process using:

```bash
kill <PID>
```

Also learned that attempting to terminate processes owned by another user may return:

```text
Operation not permitted
```

---

## Concepts Learned

- Every running program is a process.
- Every process has a unique Process ID (PID).
- Linux schedules CPU time among multiple processes.
- Processes can run in the foreground or background.
- Job control commands help manage terminal processes.
- Signals are used to communicate with running processes.

---

## Commands Practiced

```bash
ps
ps aux
top
pgrep
pidof
sleep 100
sleep 100 &
jobs
fg
bg
kill
```

---

## Next Topics

- nice
- renice
- nohup
- kill -9
- Process Priorities
- Linux Scheduling

---

## Learning Outcome

After completing this practice, I am able to:

- View running processes
- Identify process IDs
- Monitor system resources
- Run background processes
- Move processes between foreground and background
- Pause and resume jobs
- Terminate running processes safely
- Understand basic Linux process management