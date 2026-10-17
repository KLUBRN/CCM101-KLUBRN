# Backup Script Guide

## The Script (backup.sh)

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

## What did chmod +x do?

The `chmod +x backup.sh` command allows Linux to treat the script as an executable file. Before adding this permission, I could not run the script directly. After using the command, I was able to execute it with `./backup.sh` and test if it could create a compressed backup of the application data.

## Cron Expression

```bash
0 2 * * * /home/ccastillo/backup.sh
```

| Field | Value | Meaning |
|---|---|---|
| Minute | 0 | Starts the task when the minute reaches zero. |
| Hour | 2 | Sets the task to run during the 2 AM hour. |
| Day of Month | * | Allows the task to run on any date of the month. |
| Month | * | Allows the task to run in any month. |
| Day of Week | * | Allows the task to run on any day of the week. |

This schedule tells Linux to start the backup script every day at 2:00 AM. It helps keep the client's application data backed up regularly without requiring someone to start the process each night.
