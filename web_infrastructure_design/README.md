# Web Infrastructure Design

## Overview

This project focuses on designing and explaining various web infrastructure setups. You will create diagrams for different configurations, from a simple single-server setup to a complex, secured, and monitored distributed architecture.

## Learning Objectives

At the end of this project, you will be able to explain:
- Basic web infrastructure components
- The role of domain names and DNS records
- How web servers, application servers, and databases work together
- Load balancing concepts and algorithms
- Database replication (Primary-Replica/Master-Slave)
- Security measures (firewalls, SSL/HTTPS)
- Monitoring and data collection
- Scaling strategies and their trade-offs

## Requirements

### General
- A `README.md` file must be at the root of the project folder
- For each task, create a whiteboard diagram (on actual whiteboard, paper, or software)
- Take a screenshot/picture of each diagram
- Upload screenshots to an image hosting service (e.g., imgur)
- Insert the image links into your answer files
- Push your answer files to GitHub
- You must whiteboard each task in front of a mentor, staff, or student
- No computer or notes allowed during whiteboarding sessions
- You have 30 minutes per exercise
- Focus on what the requirements ask for - avoid unnecessary details

## Project Structure

```
web_infrastructure_design/
├── README.md
├── 0-simple_web_stack
├── 1-distributed_web_infrastructure
├── 2-secured_and_monitored_web_infrastructure
└── 3-scale_up
```

## Tasks

### 0. Simple Web Stack
Design a one-server web infrastructure hosting www.foobar.com

**Components:**
- 1 domain name (foobar.com) with www record pointing to 8.8.8.8
- 1 server containing:
  - Web server (Nginx)
  - Application server
  - Application files
  - Database (MySQL)

**Key Concepts to Explain:**
- Server definition and role
- Domain name purpose
- DNS record types (www)
- Web server vs application server roles
- Database function
- Client-server communication

**Issues to Address:**
- Single Point of Failure (SPOF)
- Downtime during maintenance
- Inability to scale under high traffic

### 1. Distributed Web Infrastructure
Design a three-server infrastructure for www.foobar.com

**Components:**
- 1 load balancer (HAproxy)
- 2 servers (each with complete stack)
- Primary-Replica database setup

**Key Concepts to Explain:**
- Reason for each additional component
- Load balancing algorithms
- Active-Active vs Active-Passive setups
- Primary-Replica database cluster
- Primary vs Replica node differences

**Issues to Address:**
- Remaining SPOFs
- Security concerns (no firewall, no HTTPS)
- Absence of monitoring

### 2. Secured and Monitored Web Infrastructure
Design a secure, monitored three-server infrastructure

**Additional Components:**
- 3 firewalls
- 1 SSL certificate (HTTPS)
- 3 monitoring clients

**Key Concepts to Explain:**
- Firewall purposes
- HTTPS importance
- Monitoring benefits
- Data collection methods
- QPS monitoring setup

**Issues to Address:**
- SSL termination at load balancer
- Single MySQL write server
- Identical server components problem

### 3. Scale Up
Design a scaled-up infrastructure with component separation

**Additional Components:**
- 1 additional server
- 1 additional load balancer (HAproxy cluster)
- Component separation: web server, application server, database on separate servers

**Key Concepts to Explain:**
- Reason for each addition
- Benefits of component separation

## Submission

1. Create your diagrams
2. Take screenshots/photos
3. Upload to image hosting service
4. Include image links in answer files
5. Push to GitHub repository
6. Submit GitHub file links

## Repository Information

- **GitHub repository:** holbertonschool-system_engineering-devops
- **Directory:** web_infrastructure_design
- **Files:** 
  - 0-simple_web_stack
  - 1-distributed_web_infrastructure
  - 2-secured_and_monitored_web_infrastructure
  - 3-scale_up

## Tips for Success

- Practice explaining concepts clearly and concisely
- Draw clear, labeled diagrams
- Focus on the specific requirements
- Prepare for whiteboarding sessions
- Understand the "why" behind each component

---

*Remember: All explanations must be in English to improve your technical communication skills.*
