# Linux File System Commands

## 1. Print Working Directory

### Command

```bash
pwd
```

### Description

Displays the current working directory.

### Example

```bash
pwd
```

**Output**

```text
/home/arfa/linux-for-devops
```

---

# 2. List Files and Directories

### Command

```bash
ls
```

### Description

Lists all files and directories in the current location.

### Example

```bash
ls
```

**Output**

```text
README.md
01-file-system
```

---

# 3. List Files (Detailed)

### Command

```bash
ls -l
```

### Description

Displays detailed information such as permissions, owner, size, and modification date.

---

# 4. List Hidden Files

### Command

```bash
ls -la
```

### Description

Displays all files, including hidden files.

---

# 5. Change Directory

### Command

```bash
cd
```

### Description

Changes the current directory.

### Examples

Go to Home Directory

```bash
cd ~
```

Go to Root Directory

```bash
cd /
```

Go to Parent Directory

```bash
cd ..
```

Go to a Specific Folder

```bash
cd linux-for-devops
```

---

# 6. Create Directory

### Command

```bash
mkdir
```

### Example

```bash
mkdir DevOps
```

Creates a new directory named **DevOps**.

---

# 7. Create Multiple Directories

### Command

```bash
mkdir -p Projects/Linux/File-System
```

Creates nested directories.

---

# 8. Remove Empty Directory

### Command

```bash
rmdir DevOps
```

Deletes an empty directory.

---

# 9. Create File

### Command

```bash
touch notes.txt
```

Creates an empty file.

---

# 10. Copy File

### Command

```bash
cp notes.txt backup.txt
```

Copies **notes.txt** to **backup.txt**.

---

# 11. Move or Rename File

### Command

```bash
mv backup.txt notes_backup.txt
```

Renames or moves a file.

---

# 12. Delete File

### Command

```bash
rm notes_backup.txt
```

Deletes a file.

---

# 13. Delete Directory

### Command

```bash
rm -r Projects
```

Deletes a directory and all its contents.

---

# 14. Find Files

### Command

```bash
find . -name "*.txt"
```

Searches for all `.txt` files in the current directory and its subdirectories.

---

# 15. View File Contents

### Command

```bash
cat notes.txt
```

Displays the contents of a file.

---

# 16. View Large Files

### Command

```bash
less notes.txt
```

Opens a file page by page.

Press:

- `Space` → Next page
- `b` → Previous page
- `q` → Quit

---

# 17. Display First 10 Lines

### Command

```bash
head notes.txt
```

Displays the first 10 lines of a file.

---

# 18. Display Last 10 Lines

### Command

```bash
tail notes.txt
```

Displays the last 10 lines of a file.

---

# Summary

| Command | Purpose |
|----------|---------|
| `pwd` | Show current directory |
| `ls` | List files and directories |
| `ls -l` | Detailed list |
| `ls -la` | Show hidden files |
| `cd` | Change directory |
| `mkdir` | Create directory |
| `rmdir` | Remove empty directory |
| `touch` | Create file |
| `cp` | Copy file |
| `mv` | Move or rename file |
| `rm` | Delete file |
| `find` | Search for files |
| `cat` | Display file contents |
| `less` | View large files |
| `head` | Show first 10 lines |
| `tail` | Show last 10 lines |