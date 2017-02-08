MongoDB Backup
===

This repository contains mongo backup script to automate backup process.
You must to create a schedule on the operate system to running this script properly

Install
```
git clone https://github.com/daniloharuo/mongo-backup.git /tmp/mongo-backup
cp -r /tmp/mongo-backup/mongo-backup.sh /usr/local/bin/mongo-backup
chmod +x /usr/local/bin/mongo-backup
```

Crontab Example:
```
$ cat /etc/cron.d/mongo-backup
03 */3 * * * root /usr/local/bin/mongo-backup
```
