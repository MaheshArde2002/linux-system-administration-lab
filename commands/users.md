# User Management

## Overview

User management is used to create, modify, and delete user accounts in Linux. It also helps control who can access the system and what they are allowed to do.

---

## Commands

### Check Current User

```bash
whoami
```

This command shows the name of the currently logged-in user.

Example:

```text
mahesh
```

---

### View User Information

```bash
id
```

This command displays the User ID (UID), Group ID (GID), and the groups the user belongs to.

Example:

```text
uid=1000(mahesh) gid=1000(mahesh) groups=1000(mahesh),27(sudo)
```

---

### Create a New User

```bash
sudo adduser yash
```

This command creates a new user named **yash**.

After running the command, Linux asks you to:

- Enter a password
- Confirm the password
- Enter optional user information (press Enter to skip)

---

### Change User Password

```bash
sudo passwd yash
```

This command changes or sets the password for the user **yash**.

---

### Add User to the Sudo Group

```bash
sudo usermod -aG sudo yash
```

This command gives the user **yash** administrator (sudo) privileges.

---

### Check User Groups

```bash
groups yash
```

This command displays all the groups that the user belongs to.

Example:

```text
yash : yash sudo
```

---

### Delete a User

```bash
sudo deluser yash
```

This command deletes the user account.

To delete the user's home directory as well:

```bash
sudo deluser --remove-home yash
```

---

## Commands Practiced

```bash
whoami
id
sudo adduser yash
sudo passwd yash
sudo usermod -aG sudo yash
groups yash
sudo deluser yash
```

---

## What I Learned

- How to check the current user.
- How to view user information.
- How to create a new user.
- How to change a user's password.
- How to give a user sudo access.
- How to check user groups.
- How to delete a user account.

---

## Conclusion

In this lab, I learned the basic Linux user management commands. These commands are useful for creating users, managing permissions, and controlling access to a Linux system.