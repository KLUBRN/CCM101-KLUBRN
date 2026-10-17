# Laboratory 09: Cloud Automation Engineer

## Mission Overview

In this laboratory activity, I learned how to automate tasks in a Linux environment using Bash scripting and cron jobs. I created a sample application folder, wrote a backup script, and tested it to create a compressed copy of the data. I also configured a schedule so the script could run automatically every night at 2:00 AM.

## Objectives

* Understand how Bash scripts work and how they help automate Linux commands.
* Learn how to use variables to store folder names and other values.
* Create a script that compresses application data into a backup file.
* Use `chmod +x` to give permission to execute a script.
* Configure a cron job to run the backup script at a scheduled time.
* Document the commands and results in my GitHub Cloud Computing portfolio.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
./backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
crontab -l
```

## Skills Learned

Through this activity, I practiced writing and running Bash scripts in Linux. I learned how to create folders, store test data, compress files, and check the generated backup. I also learned how file permissions work and how to schedule tasks using cron. These skills helped me understand how automation can save time, reduce repeated manual work, and make cloud operations more reliable.
