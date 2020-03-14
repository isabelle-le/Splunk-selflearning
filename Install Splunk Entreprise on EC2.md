# Install Splunk Entreprise on EC2. It runs very quickly
# Step 0: Assuming that you re familiar with AWS platform and EC2 instance.
It is guideline for OS Linux. You need to ensure security group (networking) open to port 8000.

# Step 1: Create a user account and download Splunk Entreprise. I am using Splunk 7 at this time.
https://www.splunk.com/en_us/download/splunk-enterprise.html#tabs/linux

# Step 2: Log into VM with key pair
open your terminal

make new folder (ex:SSH) mkdir SSH

move key file(ex filename.pem) to the folder: mv filename.pem SSH

chmod 400 filename.SSH

connect syntax: ssh username@ip_add -i key.pem
                ssh ec2-user@ip-name -i filename.pem
                
Check disk space on ec2 : df -hT /dev/xvda1

*where username = ec2-user (as default) and ip-name is your Private IPv4 Addresses from AWS console


# Step 3: Copy rpm to cloud server
your Splunk entreprise is rpm format, use this to copy it to your VM (tmp dir)

scp -i ~/Downloads/SSH/filename.pem splunk-7.2.4.2-fb30470262e3-linux-2.6-x86_64.rpm ec2-user@xx.xx.xx.xx:/tmp

*splunk-7.2.4.2-fb30470262e3-linux-2.6-x86_64.rpm you cane change it to your actual rmp file

# Step 4: install rpm -i directory
sudo su

rpm -i /tmp/splunk-7.2.4.2-fb30470262e3-linux-2.6-x86_64.rpm 

ll /opt/splunk  to see all folder


# Step 5: create admin credential inside user-seed.conf
vim /opt/splunk/etc/system/local/user-seed.conf

write this to the file

[user_info]
USERNAME= admin
PASSWORD= $plunkEntr3prise (strong pw of your choice)

*press SHIFT and type :w to save then :q to exist

# Step 6: boot for production
ll /opt/splunk   to see all folder, care for bin

/opt/splunk/bin/splunk enable boot-start --accept-license

ll /etc/systemd/system    to see Splunkd.service

systemctl status Splunkd  current status is disable

systemctl start Splunkd   start Splunk

ll var/log/splunk/        to check a bunch of log file

# Step 7 : access to public on web browser Your-IP4:8000

# Congrat! you have finished an Splunk Entrepise standalone installation on an EC2 
