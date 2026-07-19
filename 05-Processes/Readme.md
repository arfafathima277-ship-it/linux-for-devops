# Linux Processes

## What is a Process?

A process is a program that is currently running in memory. 
Every process has a unique Process ID (PID) assigned by the operating system.

---

# Process Commands

| Command | Purpose |
|---------|---------|
| ps | Display running processes for current session |
| ps -ef | Display all running processes with detailed information |
| ps aux | Display processes with CPU and memory usage |
| top | Monitor processes and system resources in real time |
| htop | Interactive process monitoring tool |
| ps -ef \| grep <process_name> | Search for a specific process |
| kill <PID> | Gracefully terminate a process |
| kill -9 <PID> | Forcefully terminate a process |
| pkill <process_name> | Kill process by name |
| killall <process_name> | Kill all processes with exact name |
| jobs | Display background jobs |
| bg | Resume stopped job in background |
| fg | Bring background job to foreground |
| echo $$ | Display current shell PID |
| sleep | Pause execution for specified time |
| nohup | Run process even after logout |
| pidof | Find PID of a process |
| pstree | Display parent-child process tree |
| nice | Start process with custom priority |
| renice | Change priority of running process |

---

# Process States

| State | Meaning |
|-------|---------|
| R | Running |
| S | Sleeping |
| D | Uninterruptible sleep (waiting for I/O) |
| T | Stopped/Traced |
| Z | Zombie Process |

---

# Important Concepts

## PID
PID stands for Process ID. It is a unique number assigned to every running process.

## Zombie Process
A zombie process is a completed process that still exists in the process table because the parent process has not collected its exit status.

## Process Priority

Linux uses nice values to manage process priority.

Range:

- -20 → Highest priority
- 0 → Default priority
- 19 → Lowest priority

---

# Common Interview Questions

### 1. Difference between program and process?

Program is a set of instructions stored on disk.
Process is the running instance of that program in memory.

### 2. Difference between kill and kill -9?

kill sends SIGTERM and allows graceful termination.
kill -9 sends SIGKILL and immediately terminates the process.

### 3. Difference between ps and top?

ps gives a snapshot of processes.
top provides real-time process monitoring.

### 4. Difference between nice and renice?

nice starts a process with a priority.
renice changes priority of an already running process.