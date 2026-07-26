# Process Management

## Overview

A process is a running program in Linux. Process management helps administrators monitor, manage, and stop running applications.

---

## Common Commands

### View Running Processes

```bash
ps
```

Displays currently running processes.

---

### View All Processes

```bash
ps -ef
```

Shows all running processes on the system.

---

### Monitor Processes

```bash
top
```

Displays real-time CPU and memory usage.

---

### Interactive Process Monitor

```bash
htop
```

Provides an interactive view of running processes.

> Install htop if not available:

```bash
sudo apt install htop
```

---

### Kill a Process

```bash
kill PID
```

Terminates a process using its Process ID (PID).

Example:

```bash
kill 1234
```

---

### Force Kill a Process

```bash
kill -9 PID
```

Forcefully stops a process.

---

### Find a Process

```bash
pgrep nginx
```

Finds the Process ID of a running program.

---

## Commands Practiced

```bash
ps
ps -ef
top
htop
pgrep nginx
kill PID
kill -9 PID
```

---

## What I Learned

- What a Linux process is
- Viewing running processes
- Monitoring CPU and memory usage
- Finding process IDs
- Stopping processes safely