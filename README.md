# Linux for DevOps 🐧

This repository documents my Linux learning journey for becoming a DevOps Engineer.

## 📚 Topics Covered

- File System
- Permissions
- Users & Groups
- Processes
- Networking Commands
- Package Managers
- Shell Scripting

## 📁 Repository Structure

```
linux-for-devops/
│
├── 01-file-system/
├── 02-permissions/
├── 03-users-and-groups/
├── 04-processes/
├── 05-networking/
├── 06-package-managers/
└── 07-shell-scripting/


# Linux Mint Installation using VMware Workstation

This guide explains how to install Linux Mint as a guest operating system on a Windows machine using VMware Workstation.

---

# Prerequisites

Before installing Linux Mint, make sure you have:

- Windows operating system
- VMware Workstation Player or Pro
- Linux Mint ISO image
- Minimum 20 GB free disk space
- At least 4 GB RAM (8 GB recommended)

---

# Step 1: Install VMware Workstation

1. Download VMware Workstation from the official VMware website.
2. Run the installer.
3. Accept the license agreement.
4. Choose the installation options.
5. Complete the installation.
6. Launch VMware Workstation.

---

# Step 2: Download Linux Mint

Visit the official Linux Mint website and download the latest ISO.

Available editions:

- Cinnamon (Recommended)
- MATE
- Xfce

---

# Step 3: Create a Virtual Machine

1. Open VMware Workstation.
2. Click **Create a New Virtual Machine**.
3. Select **I will install the operating system later**.
4. Select **Linux**.
5. Choose **Ubuntu 64-bit**.
6. Give the VM a name (Example: Linux Mint).
7. Allocate at least **20 GB** of disk space.
8. Click **Finish**.

---

# Step 4: Configure the Virtual Machine

Open **Edit Virtual Machine Settings**.

Recommended configuration:

| Component | Recommended Value |
|-----------|-------------------|
| RAM | 4 GB |
| CPU | 2 Cores |
| Disk | 20 GB or more |
| Video Memory | 128 MB |
| ISO Image | Linux Mint ISO |

Attach the downloaded Linux Mint ISO file under **CD/DVD**.

---

# Step 5: Install Linux Mint

1. Power on the Virtual Machine.
2. Linux Mint Live Environment will start.
3. Click **Install Linux Mint**.
4. Select your preferred language.
5. Choose the keyboard layout.
6. Select **Erase disk and install Linux Mint** (This only affects the virtual machine.)
7. Create a username and password.
8. Click **Install Now**.
9. Wait until the installation completes.
10. Restart the virtual machine.

---

# Step 6: Remove the ISO

Before restarting:

- Open VM Settings.
- Select **CD/DVD**.
- Uncheck **Connected** or remove the ISO file.

This prevents the installer from booting again.

---

# Step 7: Login

After reboot:

- Enter your username.
- Enter your password.
- Linux Mint is now ready to use.

---

# Recommended VM Configuration

| Resource | Value |
|----------|-------|
| RAM | 4 GB |
| CPU | 2 Cores |
| Storage | 20 GB |
| Video Memory | 128 MB |

---

# Advantages of Using VMware

- No changes to the Windows operating system.
- Safe environment for learning Linux.
- Easy snapshot and recovery.
- Supports multiple operating systems.
- Ideal for DevOps practice.

---

# Interview Questions

1. What is VMware Workstation?
2. Why do we use virtual machines?
3. What is a Guest Operating System?
4. What is a Host Operating System?
5. Why is Ubuntu selected while creating a Linux Mint VM?
6. What is an ISO file?
7. How much RAM is recommended for Linux Mint?
8. Why should the ISO be removed after installation?
9. What are the advantages of virtualization?
10. What is the difference between VMware Player and VMware Pro?

---

# Quick Revision

- VMware is virtualization software.
- Linux Mint runs as a Guest OS.
- Windows acts as the Host OS.
- Download the Linux Mint ISO.
- Create a virtual machine.
- Attach the ISO file.
- Install Linux Mint.
- Restart the VM.
- Remove the ISO.
- Login and start using Linux Mint.
```

## 🎯 Goal

Master Linux fundamentals required for DevOps, Cloud, and Site Reliability Engineering through hands-on practice and real-world examples.

## 🛠️ Tools

- Ubuntu (WSL2)
- VS Code
- Git
- GitHub

---
⭐ This repository is updated regularly as I progress in my DevOps learning journey.
