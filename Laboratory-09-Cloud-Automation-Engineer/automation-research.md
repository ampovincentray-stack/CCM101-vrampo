# Automation Research

## 1. Bash Script

A script written using the Bash language is a compilation of instructions that the Bash shell performs in order, which means that it can carry out any kind of task without requiring the user to enter every command. first line of a Bash script begins with a special sign `#!/bin/bash`, indicating the operating system which interpret
er to call for executing the script.

## 2. Variables

Variables are a way of saving particular values which can be used at different points in the script such as, directory names, filenames, timestamps, and so on. For example, the value of the variable `$BACKUP_DIR` is the value specified for the backup directory variable. The use of variables simplifies the maintenance of scripts, as a directory path will need to be changed only once instead of being rewritten every time in the scripts.

## 3. Cron Job

A cron job is a scheduled task in Linux that runs a command or script at specified times. It is useful in cloud operations because administrators can automate recurring tasks such as backups, maintenance, and log cleanup.A cron job refers to a scheduled task in Linux which runs any command or script at certain specified times. This could be useful in cloud operation practice since it allows the administrator to automate job execution that is carried out on an ongoing basis such as backups, maintenance, etc. Proper scheduling reduces repetitive manual work, although scheduled scripts must still be tested and monitored to avoid errors.
