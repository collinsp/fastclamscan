# fastclamscan
simple script to only scan new or updated files since last scan with improved exclude rules

problems are reported to clamscan.log and syslog
```
# install
sudo su
cd /opt
git clone https://github/fastclamscan
yum install -y clamav clamav-update

# configure a cron job to scan new files
cd /etc.cron.hourly
ln -s /opt/fastclamscan/fastclamscan```
