# Disk Management

## Overview

Disk management is used to check storage devices, monitor disk usage, and manage mounted file systems in Linux. These commands help administrators identify available disk space and troubleshoot storage-related issues.

---

## Common Commands

### Check Disk Usage

```bash
df -h
```

Displays the available and used disk space in a human-readable format.

---

### Check Directory Size

```bash
du -sh
```

Displays the size of the current directory.

To check another directory:

```bash
du -sh /home
```

---

### List Storage Devices

```bash
lsblk
```

Displays all available storage devices and partitions.

---

### Display Disk Partitions

```bash
sudo fdisk -l
```

Shows all disk partitions on the system.

---

### View Mounted File Systems

```bash
mount
```

Displays all currently mounted file systems.

---

### Unmount a File System

```bash
sudo umount /dev/sdb1
```

Unmounts a mounted file system.

> Replace **/dev/sdb1** with your actual device name.

---

## Commands Practiced

```bash
df -h
du -sh
du -sh /home
lsblk
sudo fdisk -l
mount
sudo umount /dev/sdb1
```

---

## What I Learned

- How to check disk usage
- How to check directory size
- How to view storage devices
- How to list disk partitions
- How to view mounted file systems
- How to unmount a file system

---

## Conclusion

In this lab, I learned the basic Linux disk management commands. These commands help monitor storage usage and manage disks and partitions on a Linux system.
