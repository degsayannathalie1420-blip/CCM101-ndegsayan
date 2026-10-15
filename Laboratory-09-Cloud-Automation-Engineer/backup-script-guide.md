# Backup Script Documentation

## 1. Complete Script

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup location
mkdir -p "$BACKUP_DIR"

# Save the source folder as a compressed archive
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. Why chmod +x Is Needed

The command `chmod +x backup.sh` makes the file executable. It allows Linux to run the script directly instead of requiring the commands to be copied and entered individually.

## 3. Understanding the Cron Schedule

```bash
0 2 * * * /root/backup.sh
```

The cron schedule has five time fields:

1. **Minute:** `0` means the task starts at the beginning of the hour.
2. **Hour:** `2` means the task runs at 2 AM.
3. **Day of Month:** `*` means it runs on every day of the month.
4. **Month:** `*` means it runs during every month.
5. **Day of Week:** `*` means it runs on every day of the week.

Together, these settings schedule the backup script to run every day at 2 AM. The specified file path must point to the actual script location.
