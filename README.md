# AWS EC2 – Cloud Server Deployment

## Project Overview

This project demonstrates the process of launching, configuring, and deploying a web application on an Amazon EC2 (Elastic Compute Cloud) instance. It provides hands-on experience with AWS cloud infrastructure, server configuration, networking, and web hosting.

## Technologies Used

- Amazon Web Services (AWS)
- Amazon EC2
- Linux
- Apache Web Server
- HTML
- SSH
- Security Groups

## Project Objectives

- Launch and configure an EC2 instance.
- Connect to a Linux server using SSH.
- Configure inbound and outbound network access.
- Install and configure the Apache web server.
- Create and deploy a basic HTML website.
- Access the hosted website through a public IP address.

## Implementation Steps

### 1. Launch EC2 Instance
- Open the AWS Management Console.
- Navigate to the EC2 dashboard.
- Launch a new EC2 instance.
- Select an Amazon Linux AMI.
- Choose an appropriate instance type.
- Configure the required network settings.

### 2. Connect to EC2 Instance
- Download the EC2 key pair.
- Connect to the instance using SSH.
- Verify the Linux server connection.

### 3. Configure Security Group
- Allow SSH traffic on port 22.
- Allow HTTP traffic on port 80.
- Configure inbound rules according to security requirements.

### 4. Install Apache Web Server

Update the Linux packages:

```bash
sudo dnf update -y
```

Install Apache:

```bash
sudo dnf install httpd -y
```

Start Apache:

```bash
sudo systemctl start httpd
```

Enable Apache:

```bash
sudo systemctl enable httpd
```

### 5. Deploy HTML Website

Create an HTML file:

```bash
sudo nano /var/www/html/index.html
```

Add your website content and save the file.

Restart Apache:

```bash
sudo systemctl restart httpd
```

### 6. Access the Website

Copy the EC2 instance's Public IPv4 address and open it in a web browser:

```text
http://YOUR-EC2-PUBLIC-IP
```

The deployed website should be accessible through the browser.

## Project Outcomes

- Gained practical experience with AWS EC2.
- Learned Linux server administration.
- Understood SSH connectivity and network configuration.
- Successfully installed and configured Apache.
- Deployed and accessed a website using an EC2 public IP address.

## Conclusion

This project provided practical knowledge of AWS cloud infrastructure, EC2 instance management, Linux commands, web server configuration, and basic website deployment.
