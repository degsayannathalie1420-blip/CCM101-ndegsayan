# Understanding Automation Tools

## 1. Bash Script
A Bash script is a text file that contains commands for Linux to execute automatically. The line `#!/bin/bash` tells the computer to run the file using Bash instead of treating the commands as ordinary text.

## 2. Variables
Variables let us save information and reuse it in a script. For example, `$BACKUP_DIR` represents the folder where backups are stored, so we only need to change the variable if we want to use a different folder.

## 3. Cron Job
A cron job allows Linux to run a command at a scheduled time. It is helpful in cloud computing because administrators can schedule backups and other regular tasks to run even when nobody is manually operating the terminal.
