# Automation Research

## 1. Bash Script

A Bash script is a text file containing commands that the Bash shell can execute in sequence. It helps automate repetitive tasks instead of requiring a user to type each command manually. The line `#!/bin/bash` is called the shebang, and it tells the operating system which interpreter should run the script when it is executed directly.

## 2. Variables

Variables store values that a script can reuse, such as directory paths, filenames, and timestamps. For example, `$BACKUP_DIR` represents the value assigned to the backup directory variable. Variables make scripts easier to maintain because a path can be changed in one place rather than being rewritten throughout the script.

## 3. Cron Job

A cron job is a scheduled task in Linux that runs a command or script at specified times. It is useful in cloud operations because administrators can automate recurring tasks such as backups, maintenance, and log cleanup. Proper scheduling reduces repetitive manual work, although scheduled scripts must still be tested and monitored to avoid errors.
