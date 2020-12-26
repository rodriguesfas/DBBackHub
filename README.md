# DBBackHub

A simple script python to perform database backup for github.

# Single Database Backup

    DB_NAME = 'mydb'


# Multiple Database Backup

To take multiple databases backup, create an text file like ```/backup/dbnames.txt``` and add databases names one per line like below

    # cat /backup/dbnames.txt
    database1
    mydb

And add this file to script like below.

    DB_NAME = '/backup/dbnames.txt'

# Change Backup Location

You can change below variable to change the location of backup path.

    BACKUP_PATH = '/backup/dbbackhub/'

# Execute Python Script

After downloading script make the script executable using following command.

    chmod +x dbbackhub.py

and execute this script like below

    python3 dbbackhub.py

# Appiontment

You can also schedule this script to run daily on regular interval using crontab. Add below command in crontab.

    0 2 * * * /usr/bin/python dbbackhub.py

Read more about crontab at [20 Useful Examples to Schedule Jobs](https://tecadmin.net/crontab-in-linux-with-20-examples-of-cron-schedule/).

# Credits

[Icons](https://www.iconfinder.com/icons/2276058/db_document_extension_file_icon)

# Referencie

[Python Script for MySQL Database Backup](https://tecadmin.net/python-script-for-mysql-database-backup/)

[Mysql Backup Database](https://github.com/AlexWinder/mysql-backup-database)