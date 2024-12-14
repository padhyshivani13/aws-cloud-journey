# Day 1: Amazon EC2  

## 📚 What I Learned:  
Amazon EC2 is AWS's IaaS (Infrastructure-as-a-Service) offering, providing scalable virtual servers. Here's a breakdown of my learning:  

1. **Core Concepts:**  
   - Instance Types (t2.micro for free-tier eligibility).  
   - Security Groups for access control.  
   - Key Pairs for secure SSH connections.  

2. **Key Features Explored:**  
   - Launching an EC2 instance.  
   - Configuring basic security settings.  
   - Running a simple web server.  

---

![napkin-selection](https://github.com/user-attachments/assets/fbe472cf-28ce-4d7e-aa17-1449d3546479)


## 🛠️ Hands-On Practice:  

1. **Launch an EC2 Instance:**  
   - AMI: Amazon Linux 2  
   - Instance Type: t2.micro  
   - Key Pair: Generated a new Key Pair for secure access.  

2. **Configure Security Group:**  
   - Allowed inbound traffic for SSH (port 22) and HTTP (port 80).  

3. **Host a Simple Web Page:**  
   - SSH into the instance using terminal:  
     ```bash  
     ssh -i "my-key.pem" ec2-user@<Public-IP>  
     ```  
   - Install Apache Web Server:  
     ```bash  
     sudo yum update -y  
     sudo yum install httpd -y  
     sudo systemctl start httpd  
     ```  
   - Deployed a basic HTML page at `/var/www/html/index.html`.  

---

## ✅ Outcome:  
- Successfully launched and configured an EC2 instance.  
- Learned the basics of hosting a web server in the cloud.  

---

## 🔗 Resources:  
- [AWS EC2 Documentation](https://docs.aws.amazon.com/ec2/)  
- [AWS Free Tier Details](https://aws.amazon.com/free/)  

---

## 🚀 Next Steps:  
Explore Elastic Load Balancing and EC2 Auto Scaling!  
