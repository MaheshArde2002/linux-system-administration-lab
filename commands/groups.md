# Group Management

## Overview

Group management is used to organize users into groups in Linux. Groups make it easier to manage permissions because multiple users can share the same access rights.

---

## Commands

### Create a New Group

```bash
sudo groupadd developers
```

This command creates a new group named **developers**.

---

### Add a User to a Group

```bash
sudo usermod -aG developers sagar
```

This command adds the user **sagar** to the **developers** group.

> **Note:** The `-aG` option adds the user to the group without removing them from their existing groups.

---

### Check User Groups

```bash
groups sagar
```

This command displays all the groups that the user **sagar** belongs to.

Example:

```text
sagar : sagar developers
```

---

### View Group Information

```bash
getent group developers
```

This command displays information about the **developers** group.

Example:

```text
developers:x:1002:sagar
```

---

### Delete a Group

```bash
sudo groupdel developers
```

This command deletes the **developers** group.

> **Note:** A group cannot be deleted if it is the primary group of an existing user.

---

## Commands Practiced

```bash
sudo groupadd developers
sudo usermod -aG developers sagar
groups sagar
getent group developers
sudo groupdel developers
```

---

## What I Learned

- How to create a new group.
- How to add a user to a group.
- How to check a user's group membership.
- How to view group information.
- How to delete a group.

---

## Conclusion

In this lab, I learned the basics of Linux group management. I practiced creating groups, adding users to groups, checking group membership, and deleting groups. Group management helps administrators manage permissions efficiently and securely.