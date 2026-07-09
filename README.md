# AWS EC2 Website Hosting Assignment

## Project Overview

This project demonstrates how to deploy a simple HTML website on an AWS EC2 Ubuntu instance using the Nginx web server.

The website contains my basic details such as Name, College, Branch, Email, and Date.



## Technologies Used

- AWS EC2
- Ubuntu 24.04 LTS
- Nginx
- Linux
- HTML
  


## Steps Performed

### 1. Launched an EC2 Instance
- Selected Ubuntu 24.04 AMI
- Created a new key pair (.pem)
- Configured Security Group
- Allowed SSH (Port 22)
- Allowed HTTP (Port 80)

### EC2_Dashboard
<img width="960" height="600" alt="EC2_dashboard" src="https://github.com/user-attachments/assets/ef95983a-2296-45b1-adbc-1f4729ee5e03" />


### 2. Connected to EC2

Connected securely using SSH from Windows PowerShell.

### SSH_login
<img width="960" height="600" alt="SSH_login" src="https://github.com/user-attachments/assets/a683f72a-edc7-4a36-82f4-74738c0b3238" />


### 3. Updated the Server

```bash
sudo apt update
```

### 4. Installed Nginx

```bash
sudo apt install nginx -y
```
<img width="960" height="600" alt="nginx_installation" src="https://github.com/user-attachments/assets/3b678dbc-524d-4ae5-a024-0af1ba6eb5a9" />


### 5. Hosted the Website

- Created the HTML file
- Stored it inside:

```text
/var/www/html/
```

###Verified the website using the EC2 Public IP.
<img width="960" height="600" alt="website_output" src="https://github.com/user-attachments/assets/f0063a64-67e4-4b21-8351-77232c0354d0" />




## Linux Commands Used

```bash
sudo apt update
sudo apt install nginx -y
sudo systemctl status nginx
sudo systemctl restart nginx
df -h
free -h
ps aux
```

## Project Architecture

Browser
   │
HTTP Request
   │
AWS EC2 (Ubuntu 24.04)
   │
Nginx
   │
index.html



## Challenges Faced

- Initially, SSH connection timed out.
- Identified that the issue was related to the Security Group inbound rule.
- Updated the SSH rule and successfully connected to the EC2 instance.



## Learning Outcomes

- Launching and configuring an EC2 instance.
- Connecting to EC2 using SSH.
- Installing and managing Nginx.
- Hosting a static website on AWS.
- Basic Linux server administration.
- Troubleshooting Security Group issues.



## Author

**Amrit Raj**

Galgotias University

Electronics & Communication Engineering (AIML)
