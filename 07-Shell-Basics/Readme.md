# Shell Basics

## What is a Shell?

A **Shell** is a command-line interpreter that acts as an interface between the user and the Linux kernel. It accepts user commands, sends them to the kernel for execution, and displays the output.

**Flow:**

```
User → Shell → Kernel → Hardware
```

---

## What is Bash?

**Bash (Bourne Again Shell)** is the default shell in most Linux distributions.

It provides features such as:

- Command execution
- Command history
- Auto-completion
- Variables
- Environment variables
- Input and output redirection
- Pipes
- Aliases

---

## Types of Shells

| Shell | Description |
|--------|-------------|
| sh | Bourne Shell |
| bash | Bourne Again Shell |
| zsh | Z Shell |
| ksh | Korn Shell |
| csh | C Shell |

Check the current shell:

```bash
echo $SHELL
```

Example Output:

```text
/bin/bash
```

---

# Basic Shell Commands

## Print Text

```bash
echo "Hello World"
```

---

## Display Current User

```bash
whoami
```

---

## Display Current Directory

```bash
pwd
```

---

## Display Current Date

```bash
date
```

---

## Display Calendar

```bash
cal
```

---

## Display System Uptime

```bash
uptime
```

---

## Display Hostname

```bash
hostname
```

---

## Display Linux Kernel Information

```bash
uname
```

Detailed information:

```bash
uname -a
```

---

# Variables

Variables are used to store values.

Example:

```bash
name="Arfa"

echo $name
```

Output:

```text
Arfa
```

---

# User Input

```bash
read name

echo $name
```

Or with a prompt:

```bash
read -p "Enter your name: " name

echo "Welcome $name"
```

---

# Environment Variables

Display the home directory:

```bash
echo $HOME
```

Display the current user:

```bash
echo $USER
```

Display the current shell:

```bash
echo $SHELL
```

Display executable search paths:

```bash
echo $PATH
```

---

# Command Substitution

Store command output in a variable.

```bash
today=$(date)

echo $today
```

---

# Quotes

## Single Quotes

Variables are not expanded.

```bash
echo '$HOME'
```

Output:

```text
$HOME
```

---

## Double Quotes

Variables are expanded.

```bash
echo "$HOME"
```

Output:

```text
/home/arfa
```

---

# Aliases

Create an alias:

```bash
alias ll='ls -la'
```

Use the alias:

```bash
ll
```

Remove the alias:

```bash
unalias ll
```

---

# Command History

View command history:

```bash
history
```

Run the previous command again:

```bash
!!
```

Run a command by its history number:

```bash
!50
```

---

# Wildcards

List all text files:

```bash
ls *.txt
```

List all shell scripts:

```bash
ls *.sh
```

List files starting with the letter 'a':

```bash
ls a*
```

---

# Input and Output Redirection

Overwrite a file:

```bash
echo "Hello" > file.txt
```

Append to a file:

```bash
echo "World" >> file.txt
```

Read input from a file:

```bash
cat < file.txt
```

---

# Pipes

Pass the output of one command as the input to another.

Example:

```bash
ls -l | grep test
```

Another example:

```bash
ps -ef | grep ssh
```

---

# Help Commands

Manual page:

```bash
man ls
```

Short help:

```bash
ls --help
```

---

# Exit the Shell

```bash
exit
```

---

# Common Shell Commands

| Command | Purpose |
|---------|---------|
| `echo` | Displays text or variable values. |
| `pwd` | Displays the current working directory. |
| `whoami` | Displays the current logged-in user. |
| `date` | Displays the current system date and time. |
| `cal` | Displays the calendar. |
| `uptime` | Displays system uptime and load. |
| `hostname` | Displays the system hostname. |
| `uname` | Displays basic kernel information. |
| `uname -a` | Displays detailed system information. |
| `history` | Displays previously executed commands. |
| `alias` | Creates a shortcut for a command. |
| `unalias` | Removes an alias. |
| `man` | Displays the manual page of a command. |
| `exit` | Exits the current shell session. |

---

# Advantages of Shell

- Fast command execution
- Easy system administration
- Supports automation
- Lightweight interface
- Used by Linux administrators and DevOps engineers
- Enables scripting for repetitive tasks

---

# Real-Time DevOps Use Cases

Shell is commonly used to:

- Connect to Linux servers
- Manage files and directories
- Monitor system resources
- Install software packages
- Run Docker commands
- Execute shell scripts
- Automate server administration tasks

---

# Common Interview Questions

## 1. What is a Shell?

A shell is a command-line interpreter that allows users to interact with the Linux operating system.

---

## 2. What is Bash?

Bash (Bourne Again Shell) is the default shell used in most Linux distributions.

---

## 3. What is the difference between Shell and Kernel?

| Shell | Kernel |
|--------|--------|
| Interface between the user and the operating system | Core component of the operating system |
| Accepts user commands | Manages hardware and system resources |
| Runs in user space | Runs in kernel space |

---

## 4. What are Environment Variables?

Environment variables store system information such as:

- `$HOME`
- `$USER`
- `$PATH`
- `$SHELL`

---

## 5. Difference between `>` and `>>`

| `>` | `>>` |
|------|-------|
| Overwrites existing file content | Appends content to the end of the file |

---

## 6. Difference between Single Quotes and Double Quotes

- **Single quotes (`'`)** display text literally and do not expand variables.
- **Double quotes (`"`)** expand variables and command substitutions.

---

# Summary

- Shell is the command-line interface for interacting with Linux.
- Bash is the most commonly used Linux shell.
- Shell Basics covers commands, variables, environment variables, pipes, redirection, aliases, and history.
- Understanding Shell Basics is the foundation for Shell Scripting and DevOps automation.