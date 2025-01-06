# Three-Tier Web Architecture on AWS

This project demonstrates the deployment of a **Three-Tier Web Architecture** using AWS services. It showcases a highly available, fault-tolerant, and scalable architecture by leveraging components like **Elastic Load Balancers (ELB)**, **Amazon EC2 instances**, and **Amazon Aurora**.

## 📃 **Project Overview**

The architecture consists of three main tiers:
1. **Web Tier**: Public-facing Nginx web servers serve a React.js website.
2. **Application Tier**: Internal-facing Node.js services handle backend logic and API calls.
3. **Database Tier**: Amazon Aurora MySQL with Multi-AZ replication stores and manages data.

**Key Features:**
- High Availability and Scalability
- Load Balancing and Auto Scaling
- Secure Private Subnets for Application and Database Tiers
- Health Checks for Instance Monitoring

---

## 🛠️ **Technology Stack**

### AWS Components:
- **VPC**: Virtual Private Cloud for network isolation
- **Elastic Load Balancer**: Public and Internal load balancing
- **Amazon EC2**: Web and application tier hosting
- **Amazon Aurora MySQL**: Database tier with read replica
- **Security Groups**: Fine-grained access control

### Tools and Frameworks:
- **Nginx**: Reverse proxy and static content hosting
- **React.js**: Frontend framework
- **Node.js**: Backend application
- **PM2**: Process manager for Node.js
- **MySQL**: Relational database system

---

## 📁 **Project Structure**

```bash
ThreeTierWebArchitecture/
├── web-tier/
│   ├── nginx.conf
│   └── ReactApp/
├── app-tier/
│   ├── index.js
│   ├── TransactionService.js
│   └── package.json
├── db-tier/
│   └── aurora-scripts.sql
└── README.md
