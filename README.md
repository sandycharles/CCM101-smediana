# Laboratory 09 - Cloud Automation Engineer

## Mission Overview
In this mission, I acted as a Cloud Automation Engineer at CloudNova Technologies. The goal was to remove human error from the backup process by writing a Bash script that compresses an application directory, and scheduling it with cron to run automatically every night at 2:00 AM.

## Objectives
- Understand the basic syntax of a Bash script, including variables and commands
- Use a command-line text editor to write and save scripts
- Modify file permissions using `chmod`
- Understand task scheduling and crontab syntax
- Document automation code and cron configurations using Markdown
- Complete the final chapter of the GitHub Cloud Computing Portfolio

## Commands Executed
```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
cat > ~/backup.sh
./backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
crontab -l
git add .
git commit -m "message"
git push
```

## Skills Learned
- Writing a Bash script with variables and basic commands
- Compressing directories with `tar`
- Changing file permissions with `chmod +x`
- Scheduling automated tasks with cron and reading crontab syntax
- Documenting technical work in Markdown
- Managing a project with Git and GitHub
