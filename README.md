# userdata-script
user data shell script
#!/bin/bash
yum -y install httpd
echo "*this ec2 web srv is user data script based**"
>/var/www/html/index.html
systemctl enable --now httpd
