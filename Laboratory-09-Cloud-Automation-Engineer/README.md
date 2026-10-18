
# Laboratory 9 — The Cloud Automation Engineer

## Mission Overview

This laboratory activity focuses on automating cloud administration tasks using Bash scripting and the Linux Cron scheduler. A backup script was created to compress application data into a timestamped archive and prepare it for automatic daily execution.

## Objectives

- Understand Bash scripting, variables, and the shebang.
- Create and save a Bash script using Nano.
- Use `chmod +x` to grant execute permission.
- Create and verify a compressed backup archive.
- Configure a Cron job to schedule a daily backup at 2:00 AM.
- Document the implementation and results using Markdown.
- Complete the ninth chapter of the GitHub Cloud Computing Portfolio.

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

- Writing and executing Bash scripts.
- Using variables and timestamps in automation.
- Compressing directories with `tar`.
- Managing Linux file permissions.
- Scheduling tasks using Cron.
- Creating technical documentation in Markdown.
- Maintaining a GitHub portfolio with screenshots and commits.

## Evidence

- `screenshots/script-execution.png` — Script execution and backup archive verification.
- `screenshots/cron-schedule.png` — Installed Cron schedule.
