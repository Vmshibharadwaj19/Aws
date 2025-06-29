<img width="929" alt="Screenshot 2025-06-26 110954" src="https://github.com/user-attachments/assets/19592ecf-e343-4885-a845-07d7e918d560" />
# Full Stack Portfolio Website Deployment on AWS EC2 Using Apache and GitHub

**Candidate**: Vamshi Prasad Goteti  
**Project Title**: Full Stack Portfolio Website Deployment on AWS  
**Technology Stack**: AWS EC2 (Amazon Linux 2023), Apache HTTP Server, GitHub, HTML/CSS/JS  
**Hosting IP**: http://44.203.4.136  
**GitHub Repository**: https://github.com/Vmshibharadwaj19/Aws  
**Project Owner**: Vamshi Prasad Goteti  
**Program**: MSc Computing, University of East London  
**Contact**: vamshibharadwaj19@gmail.com

---

## 📘 Overview

This project demonstrates the complete process of deploying a personal portfolio website on an Amazon EC2 instance using the AWS Free Tier. The website is sourced from a GitHub repository and hosted using Apache HTTP Server on an Amazon Linux 2023 AMI. This deployment showcases practical skills in cloud provisioning, Linux system configuration, Apache web server setup, and GitHub integration.

---

## 🚀 1. AWS EC2 Instance Launch

- **AMI**: Amazon Linux 2023 (Free Tier Eligible)  
- **Instance Type**: t2.micro  
- **Key Pair**: PEM file used for SSH access  
- **Security Group Configuration**:
  - **Inbound Rules**:
    - HTTP (Port 80) from 0.0.0.0/0  
    - HTTPS (Port 443) from 0.0.0.0/0  
    - SSH (Port 22) from My IP

### Screenshot References

<img width="959" alt="Screenshot 2025-06-26 110838" src="https://github.com/user-attachments/assets/b1d3dcfa-c0e1-4107-8c1a-d04c3bd3daed" />
- EC2 instance launch success confirmation  
- Security group with HTTP/HTTPS access  

---

## ⚙️ 2. Server Setup Commands (Executed in EC2 Terminal)

```bash
# Connect to your EC2 instance
ssh -i "your-key.pem" ec2-user@44.203.4.136

# Update the system
sudo yum update -y

# Install Apache HTTP Server
sudo yum install httpd -y

# Start and enable Apache service
sudo systemctl start httpd
sudo systemctl enable httpd

# Check Apache status
sudo systemctl status httpd
```

---

## 📂 3. Git and Project Files

```bash
# Install Git
sudo yum install git -y

# Clone your GitHub repository
git clone https://github.com/Vmshibharadwaj19/Aws

# Copy all project files to Apache's root directory
sudo cp -r Aws/* /var/www/html/

# Set appropriate permissions
sudo chmod -R 755 /var/www/html/
```

---

## 🌐 4. Deploy Website

**Final Output**: Access the live website at: http://44.203.4.136

The deployed site includes:
- CV Download  
- Technology Stack Overview  
- Contact Form/Section  

---

## 🖼️ 5. Screenshots Included

- EC2 instance creation confirmation  
- Security group with HTTP/HTTPS access  
- Git clone and deployment steps  
- Final portfolio website displayed in browser  

---

## 🛠️ Skills Demonstrated

- AWS EC2 provisioning and usage of Amazon Linux 2023  
- Apache HTTP Server installation and configuration  
- GitHub integration and code deployment  
- Linux command-line proficiency (file system navigation, permissions)  
- Hosting static websites on AWS infrastructure  
- Understanding of security groups and SSH access  

---
## **Live Images**
<img width="712" alt="Screenshot 2025-06-26 153533" src="https://github.com/user-attachments/assets/7d181bb2-0a0e-4fd6-a108-92ae48894260" />
<img width="712" alt="Screenshot 2025-06-26 153533" src="https://github.com/user-attachments/assets/7d181bb2-0a0e-4fd6-a108-92ae48894260" />
<img width="712" alt="Screenshot 2025-06-26 153533" src="https://github.com/user-attachments/assets/7d181bb2-0a0e-4fd6-a108-92ae48894260" />
<img width="959" alt="Screenshot 2025-06-26 110838" src="https://github.com/user-attachments/assets/b1d3dcfa-c0e1-4107-8c1a-d04c3bd3daed" />
## 🔗 Useful Links

- **Live Website**: http://44.203.4.136  
- **Source Code**: https://github.com/Vmshibharadwaj19/Aws  

---


