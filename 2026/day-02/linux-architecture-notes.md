# Day 2 - Linux Architecture, Processes, and systemd 🐧

## Understanding Linux Architecture

Linux is an operating system that acts as a bridge between hardware and users. It is mainly divided into three important parts:

### 1. Kernel

The kernel is the core component of Linux. It directly interacts with the hardware and manages:

* CPU
* Memory
* Devices
* Processes
* File systems

It is responsible for efficient communication between software and hardware.

### 2. User Space

User space is where users interact with the operating system through applications and commands.

Examples:

* Terminal
* Shell
* Browsers
* Text editors
* Applications

User space communicates with the kernel using system calls.

### 3. Init / systemd

When Linux boots, the kernel starts the first process called init.

Modern Linux distributions use systemd as the init system.

systemd manages:

* Services
* Background processes
* Boot process
* Logging
* System startup

---

## How Processes Are Created and Managed

A process is simply a running program.

Whenever a command or application is executed, Linux creates a process.

Important concepts:

* Every process has a unique PID (Process ID)
* Parent processes can create child processes
* Linux manages process priority and resources
* Processes can run in foreground or background

Useful commands:
```
ps
top
htop
kill
```

These commands help monitor and manage system processes.

---

## What systemd Does and Why It Matters

systemd is a system and service manager in Linux.

It is responsible for:

* Starting services during boot
* Managing background services
* Restarting failed services
* Maintaining logs
* Improving boot performance

Useful commands:

```
systemctl status nginx
systemctl start nginx
systemctl stop nginx
systemctl restart nginx
```

As a DevOps engineer, understanding systemd is important because most Linux servers and services are managed through it.

---

##
5 Commands used daily

```

* ps or top : Provides process ID, memory usage, CPU time and command name which is crucial for monitoring system performance and troubleshooting.
* chmod : Changing permission of files.
* ssh : Provides secure shell connecting to remote server.
* systemctl : Managing system services (starting, stopping).
* df /du : df is used to monitor disk space usage and du is used to estimate size of a specific directory.
```

## Key Takeaway

Linux architecture, process management, and systemd form the foundation of system administration and DevOps troubleshooting.

Understanding these concepts will help in managing servers, debugging issues, and automating infrastructure efficiently.

