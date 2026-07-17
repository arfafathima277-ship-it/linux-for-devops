# Linux Permissions

## Topics Covered

- File Permissions
- Directory Permissions
- Owner, Group, Others
- Read (r), Write (w), Execute (x)
- chmod Command
- Numeric Permissions (755, 644, 600, 777)
- Symbolic Permissions (+x, -w)

---

## Permission Structure

```text
-rwxr-xr--
```

- `-` → File
- `d` → Directory

Permissions are divided into three groups:

- Owner
- Group
- Others

---

## Numeric Permissions

| Number | Permission |
|---------|------------|
| 7 | rwx |
| 6 | rw- |
| 5 | r-x |
| 4 | r-- |
| 3 | -wx |
| 2 | -w- |
| 1 | --x |
| 0 | --- |

Examples:

```bash
chmod 755 script.sh
chmod 644 notes.txt
chmod 600 secret.txt
chmod +x deploy.sh
chmod -w notes.txt
```

---

## Common Interview Questions

- Difference between 755 and 644
- Difference between file and directory permissions
- Difference between read, write and execute
- Difference between chmod and chown
- Why execute permission is required to run a script