# Automation Research

## Bash Script
A Bash script is a plain text file containing a list of Linux commands that run one after another. It lets a person automate repetitive tasks instead of typing each command manually. The first line, `#!/bin/bash` (the shebang), tells the system to use the Bash interpreter to run the file.

## Variables
Variables store a value, such as a folder path, under a name like `$BACKUP_DIR`. Programmers use them so the path only has to be defined once and can be reused anywhere in the script. This reduces typing mistakes, and if the path ever changes, only one line needs to be edited.

## Cron Job
A cron job is a task that the Linux cron scheduler runs automatically at a set time or interval, based on a schedule written in the crontab. It works in the background without anyone needing to press a button. It is essential for cloud operations because tasks like backups, updates, and log cleanups must run reliably and on time, without depending on people to remember them.
