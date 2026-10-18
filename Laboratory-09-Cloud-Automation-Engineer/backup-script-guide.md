# Backup Script Guide

## 1. Purpose

The purpose of this Bash script is to automate the backup of the application data directory. It creates a backup directory and compresses the application files into a timestamped `.tar.gz` archive.

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

The command `chmod +x backup.sh` grants execute permission to the Bash script. This allows the user to run the script directly using `./backup.sh`, rather than only treating it as a text file.

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

When the script executes successfully, it creates the `backups` directory and a compressed archive containing the `app-data` directory. The timestamp in the archive filename helps distinguish backups created at different times.

## 6. Verification Commands

```bash
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
```

These commands verify the script's executable permission, test the backup process, list the generated archive, and display the configured Cron schedule.
