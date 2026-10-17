# Automation Research

## Bash Script

A Bash script is a file where I can put several Linux commands and run them together. The `#!/bin/bash` line tells Linux that Bash should be used to execute the commands inside the file. This makes it easier to perform tasks without entering every command one by one.

## Variables

Variables are used to keep values that a script needs, such as the location of a backup folder. For example, `$BACKUP_DIR` lets me use the same folder name in different parts of my script. If I need to change the folder name later, I only need to update the variable instead of changing every command.

## Cron Job

A cron job allows Linux to run a command or script according to a schedule. In cloud operations, it helps perform repeated tasks automatically, such as creating backups every night. This is useful because important tasks can run on time even when no one is available to start them manually.
