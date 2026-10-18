
# Laboratory 9 — The Cloud Automation Engineer

## Mission Overview

This lab activity aims at automating the management of cloud tasks through Bash scripting and CRON on Linux. A backup script is prepared to archive application files. The script will create a backup file every day at a particular time.

## Objectives

- Understand Bash scripting as well as variables and shebang.
- Write a simple Bash script through Nano editor.
- Run chmod +x to grant execution permission.
- Create and test a compressed backup archive.
- Set a Cron job, which will allow a backup to be created at 2:00 AM every day
- Record the results in Markdown.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
cat app-data/data.txt
nano backup.sh
ls -l backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
tar -tzf backups/backup_*.tar.gz
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

- Know how to write and execute Bash scripts.
- Understand the use of variables and timestamps in automation.
- Work with tar to archive folders.
- Know how to set permissions in Linux.
- Scheduling tasks using Cron.
- Create technical documents in Markdown format.
- Maintaining a GitHub portfolio with screenshots and commits.

## Evidence

- `screenshots/script-execution.png` — Script execution and backup archive verification.
- `screenshots/cron-schedule.png` — Installed Cron schedule.
