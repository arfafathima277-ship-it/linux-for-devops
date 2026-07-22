# SSH (Secure Shell)

## What is SSH?

SSH (Secure Shell) is a secure network protocol used to remotely connect to and manage Linux servers over an encrypted connection.

It allows administrators and DevOps engineers to securely access remote systems, transfer files, and execute commands.

---

# Why Use SSH?

- Secure remote login
- Encrypted communication
- Remote server administration
- Secure file transfer
- Passwordless authentication using SSH keys
- Widely used in DevOps and Cloud environments

---

# Default SSH Port

```
22
```

---

# Basic SSH Syntax

```bash
ssh username@hostname
```

Example:

```bash
ssh ubuntu@192.168.1.100
```

Using a custom port:

```bash
ssh -p 2222 ubuntu@192.168.1.100
```

---

# SSH Key Authentication

Generate an SSH key pair:

```bash
ssh-keygen
```

Default key location:

```text
~/.ssh/
```

Files created:

- `id_rsa` → Private key
- `id_rsa.pub` → Public key

---

# Copy Public Key to Remote Server

```bash
ssh-copy-id username@hostname
```

Example:

```bash
ssh-copy-id ubuntu@192.168.1.100
```

This enables passwordless login.

---

# Connect Using an SSH Key

```bash
ssh -i ~/.ssh/id_rsa username@hostname
```

Example:

```bash
ssh -i ~/.ssh/id_rsa ubuntu@192.168.1.100
```

---

# Secure File Transfer (SCP)

Copy a file to a remote server:

```bash
scp file.txt ubuntu@192.168.1.100:/home/ubuntu
```

Copy a file from a remote server:

```bash
scp ubuntu@192.168.1.100:/home/ubuntu/file.txt .
```

Copy a directory:

```bash
scp -r project ubuntu@192.168.1.100:/home/ubuntu
```

---

# Secure File Transfer (SFTP)

Start an SFTP session:

```bash
sftp ubuntu@192.168.1.100
```

Exit SFTP:

```bash
exit
```

---

# Check SSH Service Status

Ubuntu/Debian:

```bash
systemctl status ssh
```

RHEL/CentOS/Amazon Linux:

```bash
systemctl status sshd
```

---

# Start SSH Service

Ubuntu/Debian:

```bash
systemctl start ssh
```

RHEL/CentOS:

```bash
systemctl start sshd
```

---

# Stop SSH Service

Ubuntu/Debian:

```bash
systemctl stop ssh
```

RHEL/CentOS:

```bash
systemctl stop sshd
```

---

# Restart SSH Service

Ubuntu/Debian:

```bash
systemctl restart ssh
```

RHEL/CentOS:

```bash
systemctl restart sshd
```

---

# Enable SSH at Boot

Ubuntu/Debian:

```bash
systemctl enable ssh
```

RHEL/CentOS:

```bash
systemctl enable sshd
```

---

# Disable SSH at Boot

Ubuntu/Debian:

```bash
systemctl disable ssh
```

RHEL/CentOS:

```bash
systemctl disable sshd
```

---

# Display SSH Public Key

```bash
cat ~/.ssh/id_rsa.pub
```

---

# List SSH Files

```bash
ls -la ~/.ssh
```

---

# Set Secure Permissions

Private key:

```bash
chmod 600 ~/.ssh/id_rsa
```

Public key:

```bash
chmod 644 ~/.ssh/id_rsa.pub
```

SSH directory:

```bash
chmod 700 ~/.ssh
```

---

# Common SSH Commands

| Command | Purpose |
|---------|---------|
| `ssh user@host` | Connects to a remote server. |
| `ssh -p port user@host` | Connects using a custom port. |
| `ssh-keygen` | Generates an SSH key pair. |
| `ssh-copy-id user@host` | Copies the public key to a remote server. |
| `ssh -i key user@host` | Connects using a specific private key. |
| `scp` | Securely copies files between systems. |
| `sftp` | Starts a secure file transfer session. |
| `systemctl status ssh` | Checks the SSH service status. |
| `systemctl restart ssh` | Restarts the SSH service. |
| `cat ~/.ssh/id_rsa.pub` | Displays the public SSH key. |

---

# Advantages of SSH

- Secure encrypted communication
- Remote server access
- Passwordless authentication
- Secure file transfer
- Easy server management
- Essential for cloud platforms like AWS

---

# Real-Time DevOps Use Cases

SSH is commonly used to:

- Connect to AWS EC2 instances
- Manage Linux servers remotely
- Deploy applications
- Transfer configuration files
- Restart services
- Troubleshoot production servers
- Access Jenkins, Docker, and Kubernetes nodes

---

# Common Interview Questions

## 1. What is SSH?

SSH (Secure Shell) is a secure protocol used to remotely access and manage Linux servers.

---

## 2. What is the default SSH port?

```
22
```

---

## 3. What is the difference between SSH and Telnet?

| SSH | Telnet |
|------|--------|
| Encrypted communication | Plain-text communication |
| Secure | Not secure |
| Default port 22 | Default port 23 |

---

## 4. What is passwordless authentication?

It is a method of logging into a remote server using an SSH key pair instead of a password.

---

## 5. What is `scp`?

`scp` (Secure Copy Protocol) is used to securely copy files between local and remote systems over SSH.

---

## 6. What is `sftp`?

SFTP (Secure File Transfer Protocol) is used to securely transfer files over an SSH connection.

---

## Best Practices

- Never share your private key (`id_rsa`).
- Use strong passphrases for SSH keys.
- Disable password authentication when using key-based login.
- Keep SSH software updated.
- Use SSH keys instead of passwords whenever possible.

---

# Summary

- SSH provides secure remote access to Linux servers.
- SSH encrypts all communication between client and server.
- SSH keys enable passwordless authentication.
- `scp` and `sftp` are used for secure file transfers.
- SSH is one of the most essential tools for Linux administrators and DevOps engineers.