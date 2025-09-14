# Static Website Hosting on AWS EC2 with Nginx;-

## 📌 Project Overview
This project demonstrates how I hosted a **static website** on an **AWS EC2 instance** using **Nginx web server**.  
The goal was to understand cloud basics,Elastic compute cloud(ec2), Linux commands, and how to deploy a website on a virtual server.

## ⚡ Tech Stack
- **AWS EC2** (Amazon Linux 2, t2.micro – Free Tier)
- **Nginx Web Server**
- **Git Bash** (for SSH)
- **HTML, CSS** (static website)

## 🚀 Deployment Steps
1. **Launched EC2 Instance**  
   - Selected Amazon Linux 2 AMI and free tier `t2.micro`.  
   - Configured Security Group to allow **HTTP (80)** and **SSH (22)** traffic.  

2. **Connected via SSH**  
    Used Git Bash to connect:  
     ssh -i keypair.pem ec2-user@<public-ip>
     
3. **Installed Nginx**  
   sudo yum update -y
   sudo yum install nginx -y
   sudo systemctl start nginx
    
4. Deploy Website**
- Navigate to Nginx default HTML directory:
  cd /usr/share/nginx/html/
  sudo rm index.html
  sudo nano index.html (website content)
  http://<user-ec2-public-ip>



   

   sudo systemctl start nginx

