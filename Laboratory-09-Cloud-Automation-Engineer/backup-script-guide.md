# Backup Script Guide

## 1. Purpose

This Bash script is meant to simplify the backing up of the application data directory by creating a backup folder as well as packing the application data into a .tar.gz archive named after the date. 

## 2. Complete Bash Script

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

## 3. File Permissions

With the command `chmod +x backup.sh`, execute permissions are granted for Bash scripts. This enables the user to execute `./backup.sh`, as opposed to just treating the file as a simple text file.

## 4. Cron Job Configuration

The Cron expression used in the laboratory activity is:

```cron
0 2 * * * /root/backup.sh
```

### Explanation of the Five Time Fields

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | Runs at minute zero |
| Hour | `2` | Runs at 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

The command `/root/backup.sh` identifies the script that Cron executes.

## 5. Expected Result

When executed, the script is able to create the backups directory with the archived app data. 

## 6. Verification Commands

```bash
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
```

This command allows for checking the execution permissions of the script and testing the process of creating the backup, listing the created archives and displays the current Cron schedule.
