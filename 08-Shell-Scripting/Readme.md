# Shell Scripting

## What is Shell Scripting?

Shell scripting is the process of writing a sequence of Linux commands in a file and executing them automatically.

A shell script helps automate repetitive tasks such as backups, deployments, user management, and system monitoring.

Scripts are usually saved with the `.sh` extension.

---

# Why Use Shell Scripting?

- Automates repetitive tasks
- Saves time and effort
- Reduces manual errors
- Improves productivity
- Simplifies system administration
- Used extensively in DevOps automation

---

# Shell Script File Extension

```
.sh
```

Example:

```
backup.sh
```

---

# Shebang

Every shell script should begin with:

```bash
#!/bin/bash
```

The shebang tells Linux which interpreter should execute the script.

---

# Creating a Shell Script

Create a new script:

```bash
touch hello.sh
```

Edit the script:

```bash
nano hello.sh
```

Example:

```bash
#!/bin/bash

echo "Hello, World!"
```

---

# Execute Permission

Before running a script, give it execute permission:

```bash
chmod +x hello.sh
```

---

# Running a Script

Method 1:

```bash
./hello.sh
```

Method 2:

```bash
bash hello.sh
```

---

# Variables

Variables store data.

Example:

```bash
#!/bin/bash

name="Arfa"

echo "Welcome $name"
```

---

# User Input

```bash
#!/bin/bash

read -p "Enter your name: " name

echo "Hello $name"
```

---

# Command Line Arguments

Arguments can be passed while executing a script.

Example:

```bash
#!/bin/bash

echo "First Argument: $1"
echo "Second Argument: $2"
```

Run:

```bash
bash script.sh DevOps Docker
```

Output:

```
First Argument: DevOps
Second Argument: Docker
```

---

# Conditional Statements

## if Statement

```bash
#!/bin/bash

age=20

if [ $age -ge 18 ]
then
    echo "Eligible to vote"
fi
```

---

## if-else Statement

```bash
#!/bin/bash

age=16

if [ $age -ge 18 ]
then
    echo "Eligible"
else
    echo "Not Eligible"
fi
```

---

# For Loop

```bash
#!/bin/bash

for i in 1 2 3 4 5
do
    echo $i
done
```

---

# While Loop

```bash
#!/bin/bash

count=1

while [ $count -le 5 ]
do
    echo $count
    count=$((count+1))
done
```

---

# Functions

```bash
#!/bin/bash

greet() {
    echo "Welcome to DevOps"
}

greet
```

---

# Exit Status

Check whether the previous command executed successfully.

```bash
echo $?
```

- `0` → Success
- Non-zero → Failure

---

# Comments

Single-line comment:

```bash
# This is a comment
```

---

# Common Shell Script Commands

| Command | Purpose |
|---------|---------|
| `touch file.sh` | Creates a shell script file. |
| `nano file.sh` | Opens the script for editing. |
| `chmod +x file.sh` | Gives execute permission. |
| `bash file.sh` | Executes the script using Bash. |
| `./file.sh` | Executes the script directly. |
| `echo` | Displays output. |
| `read` | Accepts user input. |
| `date` | Displays the current date and time. |
| `pwd` | Displays the current working directory. |
| `whoami` | Displays the current user. |
| `hostname` | Displays the hostname. |
| `clear` | Clears the terminal screen. |

---

# Real-Time DevOps Use Cases

Shell scripting is commonly used to:

- Automate deployments
- Backup files and databases
- Monitor CPU, memory, and disk usage
- Restart failed services
- Schedule tasks using Cron
- Automate Docker commands
- Generate log reports
- Perform server health checks

---

# Common Interview Questions

## 1. What is Shell Scripting?

Shell scripting is the process of writing Linux commands into a script file to automate tasks.

---

## 2. What is Bash?

Bash (Bourne Again Shell) is the default command-line interpreter in most Linux distributions.

---

## 3. What is the purpose of the shebang (`#!/bin/bash`)?

It tells Linux to execute the script using the Bash interpreter.

---

## 4. How do you execute a shell script?

```bash
bash script.sh
```

or

```bash
./script.sh
```

(after giving execute permission)

---

## 5. What does `chmod +x` do?

It gives execute permission to a shell script.

---

## 6. What are `$1`, `$2`, `$3`?

They represent command-line arguments passed to the script.

---

## 7. What does `$?` represent?

It stores the exit status of the previously executed command.

- `0` → Success
- Non-zero → Failure

---

# Best Practices

- Use meaningful variable names.
- Add comments to improve readability.
- Keep scripts simple and modular.
- Handle errors whenever possible.
- Test scripts before using them in production.

---

# Summary

- Shell scripting automates Linux tasks.
- Scripts use the `.sh` extension.
- `#!/bin/bash` specifies the Bash interpreter.
- Variables, loops, conditions, and functions help build automation scripts.
- Shell scripting is an essential skill for Linux administrators and DevOps engineers.