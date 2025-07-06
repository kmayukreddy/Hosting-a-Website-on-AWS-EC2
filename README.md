# Hosting-a-Website-on-AWS-EC2
# 🌐 Hosting a Static Website on AWS EC2

This project demonstrates how to deploy a basic static website using **Apache2** on an **Amazon EC2** instance running Ubuntu 22.04. It’s part of my cloud computing learning journey.

---

## 📌 Project Summary

- 🔧 **Deployed**: Apache2 on EC2 (Ubuntu 22.04 LTS)
- 🌍 **Hosted Website**: Accessible via Public IPv4
- ☁️ **Platform**: Amazon Web Services (AWS)
- 🔑 **Secure Access**: SSH using `.pem` key
- ✅ **Goal**: Understand cloud VM deployment & basic web hosting

---

## 🧰 Tools & Technologies

- **AWS EC2 (Free Tier)**
- **Ubuntu 22.04 LTS**
- **Apache2**
- **Git Bash** (for SSH on Windows)
- **.pem Key Pair** for secure login
- **Browser** for site access

---

## 🚀 Steps Performed

1. **Launched EC2 Instance**
   - OS: Ubuntu 22.04 LTS
   - Instance Type: t2.micro
   - Auto-assigned Public IP
   - Created key pair (`ec2-key.pem`)

2. **Configured Security Group**
   - Allowed:
     - SSH (TCP 22) from 0.0.0.0/0
     - HTTP (TCP 80) from 0.0.0.0/0

3. **Connected to EC2 via SSH**
   ```bash
   chmod 400 ec2-key.pem
   ssh -i ec2-key.pem ubuntu@<your-ec2-public-ip>

