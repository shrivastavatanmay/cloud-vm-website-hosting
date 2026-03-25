# 🚀 Cloud VM Website Hosting (AWS EC2 + Nginx)

## 📌 Project Overview
This project demonstrates how to host a static website on an AWS EC2 instance using Nginx as a web server.

The goal was to understand core cloud concepts like instance provisioning, networking, and web server configuration.

---

## 🏗️ Architecture
- User accesses website via Public IP  
- Traffic goes through **Security Group (Port 80)**  
- EC2 instance (Ubuntu) processes request  
- Nginx serves static HTML content  

---

## ⚙️ Steps Performed

### 1. Launch EC2 Instance
- OS: Ubuntu  
- Instance Type: t2.micro  
- Region: Asia Pacific (Mumbai)  

---

### 2. Configure Security Group
- Port 22 → SSH access  
- Port 80 → HTTP access  

---

### 3. Connect to Instance
```bash
ssh -i your-key.pem ubuntu@your-public-ip
```

---

### 4. Install Nginx
```bash
sudo apt update
sudo apt install nginx -y
```

---

### 5. Start & Enable Nginx
```bash
sudo systemctl start nginx
sudo systemctl enable nginx
```

---

### 6. Deploy Website
```bash
cd /var/www/html
sudo nano index.html
```

Paste your HTML and save.

---

## 🖥️ Output
Website accessible via:
```
http://<your-public-ip>
```

---

## 🧠 What I Learned
- How EC2 works in real-world deployment  
- Importance of security groups (ports control everything)  
- Basics of Nginx as a web server  
- How public IP routing works  

---

## ⚠️ Challenges Faced
- Website not loading due to closed port 80  
- Initial SSH connection issues (wrong key usage)  

---

## 📸 Screenshots

### 🔹 Nginx Running on EC2
![Nginx Status](./screenshots/nginx-status.png)

### 🔹 Security Group Configuration
![Security Group](./screenshots/security-group.png)

### 🔹 Final Website Output
![Website Output](./screenshots/final-output.png)

---

## 🛠️ Tech Stack
- AWS EC2  
- Ubuntu Linux  
- Nginx  
- HTML & CSS  

---

## 🔗 Project Link
👉 https://github.com/shrivastavatanmay/cloud-vm-website-hosting

---

## 👨‍💻 Author
**Tanmay Srivastava**  
Aspiring Cloud Engineer 🚀
