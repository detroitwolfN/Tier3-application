# Tier3-application
a tier 3 application using nginx, mysql and ec2 t2 instance
# DevOps Project: "Hello World" Web Application on AWS

## Table of Contents

## Project Overview
This project sets up a simple "Hello World" web application hosted on an AWS EC2 instance. The HTML file is served by Nginx and can be accessed via a link stored in a MySQL database. The infrastructure is provisioned using AWS services including VPC, EC2, Internet Gateway, and Nginx, while MySQL is used to store the link on a t2.micro instance.


The architecture includes:
- **VPC**: A Virtual Private Cloud for secure networking.
- **EC2**: Hosts the web server and MySQL database.
- **Internet Gateway**: Provides public access to the EC2 instance.
- **Nginx**: A reverse proxy server to serve the HTML file.
- **MySQL**: Stores the link to the HTML file.

## Technologies Used
- **AWS Services**: EC2, VPC, Internet Gateway
- **Web Server**: Nginx
- **Database**: MySQL on EC2
- **Operating System**: Amazon Linux 2
- **HTML**: A simple "Hello World" file

## Infrastructure Setup

### Prerequisites
Before starting, make sure you have the following:
- AWS Account
- AWS CLI installed and configured
- EC2 key pair for SSH access
- MySQL client installed locally (for interacting with the database)

### Deployment Instructions
1. **Create VPC and Subnet**:
   - Use AWS console to create a VPC with public subnets.
   - Ensure an Internet Gateway is attached to provide public access.

2. **Launch EC2 Instance**:
   - Launch a t2.micro EC2 instance in the VPC.
   - Install Nginx and MySQL on the instance.

3. **SSH into EC2**:
   ```bash
   ssh -i "tier3ap.ppk" ec2-user@18.141.240.44
