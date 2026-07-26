# Cron Jobs

## Overview

Cron is a Linux utility used to schedule tasks automatically at a specific time or date. These scheduled tasks are called **Cron Jobs**.

Cron is useful for automating tasks like backups, log cleanup, and running scripts.

---

## Common Commands

### Open Crontab

```bash
crontab -e
```

Opens the crontab file to create or edit scheduled tasks.

---

### View Scheduled Cron Jobs

```bash
crontab -l
```

Displays all scheduled cron jobs for the current user.

---

### Remove All Cron Jobs

```bash
crontab -r
```

Deletes all scheduled cron jobs.

> **Note:** Be careful while using this command.

---

## Cron Job Format

```text
* * * * * command
│ │ │ │ │
│ │ │ │ └── Day of Week (0-7)
│ │ │ └──── Month (1-12)
│ │ └────── Day of Month (1-31)
│ └──────── Hour (0-23)
└────────── Minute (0-59)
```

---

## Examples

Run a script every day at 9:00 AM

```text
0 9 * * * /home/mahesh/backup.sh
```

Run a command every minute

```text
* * * * * date
```

Run every Sunday at 10:30 PM

```text
30 22 * * 0 echo "Weekly Backup"
```

---

## Commands Practiced

```bash
crontab -e
crontab -l
crontab -r
```

---

## What I Learned

- What Cron is
- How to create a Cron Job
- How to view Cron Jobs
- How to remove Cron Jobs
- Understanding Cron schedule format

---

## Conclusion

In this lab, I learned how to automate tasks using Cron Jobs. I practiced creating, viewing, and deleting scheduled tasks using the crontab command.

