# Laboratory 09: The Cloud Automation Engineer

## Mission Overview
This activity demonstrates how to automate application backups on a Linux system using Bash scripts and cron jobs.

## Objectives
- Learn the basics of Bash scripting.
- Create a sample application data directory.
- Write a script that compresses files into a backup archive.
- Make the script executable.
- Schedule automatic backups using cron.
- Document the commands and results.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned
I learned how to write a simple Bash script, create directories, store values in variables, compress files, change permissions, and schedule commands using cron. I also practiced documenting my work using Markdown.
