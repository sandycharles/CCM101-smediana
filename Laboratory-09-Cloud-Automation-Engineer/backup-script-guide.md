# Backup Script Guide

This guide documents the automated backup solution for CloudNova Technologies so the client's IT team can understand how it works.

## 1. The Backup Script (`backup.sh`)

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. What `chmod +x` Did

New files in Linux do not have execute permission, so running `./backup.sh` first gave a "Permission denied" error. The command `chmod +x backup.sh` added the execute (`x`) permission to the file. The permissions changed from `-rw-r--r--` to `-rwxr-xr-x`, so the system could run it as a program.

## 3. The Cron Expression

```
0 2 * * * /root/backup.sh
```

| Field | Value | Meaning |
|---|---|---|
| Minute | 0 | At minute 0 (the start of the hour) |
| Hour | 2 | At 2 AM (24-hour format) |
| Day of Month | * | Every day of the month |
| Month | * | Every month |
| Day of Week | * | Every day of the week |

Together, this runs the backup script **every night at exactly 2:00 AM** without anyone pressing a button.
