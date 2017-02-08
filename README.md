MongoDB Backup
===

This repository contains mongo backup script to automate backup process .
You must to create a schedule on the operate system to running this script properly

Install
```
git clone https://github.ns2online.com.br/infraweb/mongo-backup.git /tmp/mongo-backup
cp -r /tmp/mongo-backup/*.sh /usr/local/bin/.
```

Crontab Example:
```
$ cat /etc/cron.d/mongoBackup
03 */3 * * * root /usr/local/bin/mongoBackup.sh
```
