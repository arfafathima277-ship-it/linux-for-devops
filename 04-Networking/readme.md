# Linux Networking

## Overview
Linux networking commands are used to check connectivity, view network configuration, troubleshoot network issues, and communicate with remote systems.

---

## Common Commands

### ping
Checks network connectivity.

```bash
ping google.com
ping -c 4 google.com
```

---

### ip
Displays network configuration.

```bash
ip addr
ip route
```

---

### ifconfig (Legacy)

```bash
ifconfig
```

> Note: `ip addr` is the modern replacement.

---

### hostname
Displays the system hostname.

```bash
hostname
```

---

### ss
Shows active network connections and listening ports.

```bash
ss
ss -tuln
```

---

### netstat (Legacy)

```bash
netstat -tuln
```

---

### curl
Transfers data from a server.

```bash
curl https://example.com
curl -I https://example.com
```

---

### wget
Downloads files.

```bash
wget https://example.com/file.zip
```

---

### nslookup
Finds the IP address of a domain.

```bash
nslookup google.com
```

---

### dig
Displays detailed DNS information.

```bash
dig google.com
```

---

### traceroute
Shows the path packets take to reach a destination.

```bash
traceroute google.com
```

---

### ssh
Connects to a remote server.

```bash
ssh user@server-ip
```

---

### scp
Copies files securely between systems.

```bash
scp file.txt user@server:/home/user/
scp user@server:/home/user/file.txt .
```

---

## Interview Questions

- What is the purpose of the `ping` command?
- Which protocol does `ping` use?
- Difference between `ip` and `ifconfig`?
- Difference between `ss` and `netstat`?
- Difference between `curl` and `wget`?
- How do you connect to a remote Linux server?
- Which command is used to securely copy files?

---

## Quick Reference

| Command | Purpose |
|---------|---------|
| `ping` | Check network connectivity |
| `ip addr` | Show IP address |
| `ip route` | Show routing table |
| `hostname` | Display hostname |
| `ss -tuln` | Show listening ports |
| `curl` | Transfer data |
| `wget` | Download files |
| `nslookup` | DNS lookup |
| `dig` | Detailed DNS lookup |
| `traceroute` | Show packet path |
| `ssh` | Remote login |
| `scp` | Secure file copy |