#!/bin/bash
yum update -y
yum install httpd -y
systemctl start httpd
systemctl enable httpd
cd /var/www/html
echo "THIS THE TEST WORK GITHUB" >index.html
sudo systemctl restart httpd
