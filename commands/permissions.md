# Linux File Permissions

## Overview

Linux file permissions determine who can read, write, or execute files and directories. Proper permission management is essential for securing Linux systems and controlling access to resources.

---

## Permission Types

| Permission | Symbol | Value | Description |
|------------|--------|------:|-------------|
| Read | r | 4 | View file contents or list directory contents |
| Write | w | 2 | Modify a file or create/delete files in a directory |
| Execute | x | 1 | Execute a file or access a directory |

---

## Viewing File Permissions

Display file permissions using:

```bash
ls -l
```

Example:

```text
-rwxr-xr-- 1 mahesh developers 1200 Jul 26 script.sh
```

Permission breakdown:

```text
-rwxr-xr--
│││ │││ │││
│││ │││ └── Others
│││ └────── Group
└────────── Owner
```

---

## Changing Permissions

### Add execute permission

```bash
chmod +x script.sh
```

### Remove write permission

```bash
chmod u-w script.sh
```

### Set permissions using numeric mode

```bash
chmod 755 script.sh
chmod 644 file.txt
chmod 700 private.sh
```

---

## Numeric Permission Values

| Number | Permission |
|--------:|------------|
| 7 | rwx |
| 6 | rw- |
| 5 | r-x |
| 4 | r-- |
| 0 | --- |

Example:

```bash
chmod 755 script.sh
```

Meaning:

- Owner → Read, Write, Execute
- Group → Read, Execute
- Others → Read, Execute

---

## Changing Ownership

Change owner:

```bash
sudo chown mahesh file.txt
```

Change owner and group:

```bash
sudo chown mahesh:developers file.txt
```

Change only group:

```bash
sudo chgrp developers file.txt
```

---

## Recursive Permissions

Apply permissions to all files and directories:

```bash
chmod -R 755 website/
```

Change ownership recursively:

```bash
sudo chown -R mahesh:developers website/
```

---

## Default Permissions (umask)

Display current umask:

```bash
umask
```

Example:

```bash
umask 022
```

---

## Practical Example

Create a file:

```bash
touch demo.txt
```

View permissions:

```bash
ls -l demo.txt
```

Make it executable:

```bash
chmod +x demo.txt
```

Verify:

```bash
ls -l demo.txt
```

---

## Common Interview Questions

### What is the difference between `chmod` and `chown`?

- `chmod` changes file permissions.
- `chown` changes file ownership.

### What does `chmod 755` mean?

- Owner: Read, Write, Execute
- Group: Read, Execute
- Others: Read, Execute

### What is `umask`?

`umask` sets the default permissions assigned to newly created files and directories.

---

## Troubleshooting

### Permission Denied

Error:

```text
Permission denied
```

Solution:

```bash
chmod +x script.sh
```

### Cannot Edit a File

Check ownership:

```bash
ls -l
```

Change owner:

```bash
sudo chown $USER:$USER file.txt
```

---

## Commands Practiced

```bash
ls -l
chmod +x script.sh
chmod 755 script.sh
chmod 644 file.txt
chmod -R 755 directory
chown
chgrp
umask
```

---

## Skills Learned

- Understanding Linux file permissions
- Managing file ownership
- Using symbolic and numeric permission modes
- Applying recursive permissions
- Working with `umask`
- Troubleshooting permission-related issues

