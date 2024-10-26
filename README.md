# My-Simple-Website
A Simple website launch using Apache2 in the OS ubuntu in the cloud AWS

---
Steps to follow:
---
1. Create a VPC
2. Create public subnet
3. Create Route table and configure route with subnet
4. Create an public ec2 instance in ubuntu OS
5. Install Apache Webserver (Apache2)
6. Create Security group and set inbound rules for http and ssh

```
sudo su -
apt update
apt install apache2
```
7. Find the index.html file.If not create a file (/var/www/html/index.html)
8. Now start and enable the apache server
```
systemctl start apache2
systemctl enable apache2
systemctl status apache2
```
9. Now take the public ip address of the ec2 instance and type it on google URL, you will below image on succcessful launching of website.

![image](https://github.com/user-attachments/assets/afad8c7d-7718-40c0-969e-fd80d1b75d48)

(above image is for default index.html)

---
Notes:
---
1. Always check for security groups if http and ssh enabled.
2. Ec2 instance should have public ip address
3. File name always should be index.html or home.html
