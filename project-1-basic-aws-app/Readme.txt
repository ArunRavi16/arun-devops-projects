# Basic AWS Two-Tier Application

This project demonstrates how to deploy a **Frontend + Backend** application on AWS using:

- VPC
- Public & Private Subnets
- Internet Gateway
- NAT Gateway (optional)
- EC2 (Frontend in Public, Backend in Private)
- Security Groups
- NACLs
- PM2 for backend service management

##  Architecture Overview
Frontend → Public Subnet → Calls Backend API (Private Subnet via Security Group Rules)

## Tech Stack
- Frontend: HTML + JavaScript
- Backend: Node.js (Express)
- AWS EC2
- Linux
- PM2

## How to Run Locally
cd backend
npm install
node server.js
Open:
frontend/index.htm

## How to Deploy
1. Launch EC2 in public subnet for frontend  
2. Launch EC2 in private subnet for backend  
3. Allow only frontend SG → backend SG  
4. Run backend with PM2  
5. Update frontend JS with backend private IP  

# Why this project?
This proves your understanding of **AWS networking**, **EC2**, **security**, **frontend-backend communication**, and **Linux administration**.

