# Linux Users & Groups

## 📌 What are Users and Groups?

Linux is a multi-user operating system. Every user belongs to one or more groups. Users and groups help control access to files, directories, and system resources.

---

# Common Commands

| Command | Purpose | Example |
|---------|---------|---------|
| `whoami` | Display the current logged-in user | `whoami` |
| `id` | Display User ID (UID), Group ID (GID), and groups | `id` |
| `who` | Show users currently logged into the system | `who` |
| `groups` | Display groups of the current user | `groups` |
| `sudo` | Execute a command with administrator privileges | `sudo apt update` |
| `su` | Switch to another user | `su root` |
| `useradd` | Create a new user | `sudo useradd john` |
| `passwd` | Create or change a user's password | `sudo passwd john` |

---

# Important Terms

## User (UID)

A unique user account in Linux.

Example:

```bash
id
```

Output:

```text
uid=1000(arfa)
```

---

## Group (GID)

A collection of users with similar permissions.

Example:

```text
gid=1000(arfa)
```

---

## Root User

- Superuser in Linux
- Has full access to the system
- Username: `root`
- UID: `0`

---

## Sudo

`sudo` allows a normal user to execute commands with administrator privileges.

Example:

```bash
sudo apt update
```

---

## Switch User

Switch to another user.

```bash
su root
```

---

## Create a User

```bash
sudo useradd devops
```

---

## Change Password

```bash
sudo passwd devops
```

---

# Common Interview Questions

### 1. What is the difference between `whoami` and `id`?

**whoami**
- Displays only the current username.

**id**
- Displays username, UID, GID, and groups.

---

### 2. What is UID?

UID (User ID) is a unique number assigned to every user.

Example:

```text
uid=1000(arfa)
```

---

### 3. What is GID?

GID (Group ID) identifies the primary group of a user.

---

### 4. Who is the root user?

The root user is the administrator of Linux with unrestricted access to the system.

---

### 5. What is the purpose of `sudo`?

`sudo` allows a normal user to execute commands with administrator privileges.

Example:

```bash
sudo apt install nginx
```

---

### 6. What is the difference between `sudo` and `su`?

| sudo | su |
|------|-----|
| Executes a single command as another user (usually root) | Switches to another user account |
| More secure | Less secure if shared |

---

### 7. How do you check the current user?

```bash
whoami
```

---

### 8. How do you check user details?

```bash
id
```

---

### 9. How do you see the groups of the current user?

```bash
groups
```

---

### 10. Why are groups used in Linux?

Groups make permission management easier by allowing multiple users to share the same access rights.

---

# Quick Revision

```text
whoami   → Current logged-in user
id       → User ID, Group ID, Groups
who      → Logged-in users
groups   → User groups
sudo     → Run command as administrator
su       → Switch user
useradd  → Create user
passwd   → Change password
```