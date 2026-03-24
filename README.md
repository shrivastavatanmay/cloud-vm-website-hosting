# Cloud VM Website Hosting

## 1) Project Overview
This is my first cloud project where I hosted a static website on an AWS EC2 instance using Nginx.

---

## 2) What I Did
- Launched an EC2 instance (Ubuntu)
- Configured security groups by allowing ports 22 (SSH) and 80 (HTTP)
- Connected to the instance using SSH
- Installed and started Nginx web server
- Deployed a simple HTML website

---

## 3)Technologies Used
- AWS EC2
- Linux (Ubuntu)
- Nginx
- HTML

---

## 4) Result
The website was successfully hosted and could be accessed using the public IP of the EC2 instance.

---

## 5) Challenges Faced
- Initially, the website was not loading because port 80 was not enabled in the security group. After allowing HTTP traffic, the issue was resolved.
- Faced minor confusion while connecting via SSH, which was fixed by using the correct key pair.
