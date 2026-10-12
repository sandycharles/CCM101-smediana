# Automation Research

## Bash Script
A Bash script is a plain text file containing a list of Linux commands that run one after another, so a task can be repeated without typing each command by hand. The first line, `#!/bin/bash` (the shebang), tells the system to use the Bash interpreter to run the file.

## Variables
Variables store a value, like a folder path, under a name such as `$BACKUP_DIR`. Instead of typing the full path in many places, a programmer defines it once and reuses it. This reduces typos, and if the path changes, only one line needs to be edited.

## Cron Job
A cron job is a task that the Linux cron scheduler runs automatically at a set time or interval, based on a schedule written in the crontab. It is essential for cloud operations because backups, updates, and log cleanups must happen reliably without a person remembering to do them.
