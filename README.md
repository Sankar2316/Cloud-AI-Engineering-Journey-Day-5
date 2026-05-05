# 🚀 Day 05 – Networking (VPC, Subnets, Internet Gateway)

---

## 📌 Overview

On Day 05, I learned about **Cloud Networking**, focusing on how resources communicate securely inside a cloud environment using Virtual Private Cloud (VPC).

---

## 🌐 What is VPC?

A **Virtual Private Cloud (VPC)** is a logically isolated network in the cloud where you can launch your resources securely.

👉 Think of it as your **own private network inside the cloud**

---

## 🧱 Core Components of VPC

### 1. Subnets

* Divisions of VPC network
* Used to organize resources

👉 Types:

* **Public Subnet** → Accessible from internet
* **Private Subnet** → Not directly accessible

---

### 2. Internet Gateway (IGW)

* Allows communication between VPC and internet

---

### 3. Route Tables

* Define how traffic flows inside the network

---

### 4. NAT Gateway

* Allows private subnet instances to access internet
* But blocks incoming traffic

---

## 🔐 Security in Networking

* **Security Groups** → Instance-level firewall
* **Network ACLs** → Subnet-level firewall

---

## ⚙️ Workflow Diagram

![VPC Workflow](diagram.png)

### (Text Version)

```plaintext
Internet
   ↓
Internet Gateway
   ↓
Public Subnet (Web Server)
   ↓
Private Subnet (Database)
```

---

## 🌍 Real-World Architecture Example

* Web Server → Public Subnet
* Application Server → Private Subnet
* Database → Private Subnet

👉 Secure + scalable architecture

---

## 🔟 Real-World Use Cases

1. Host secure web applications
2. Multi-tier architecture (Frontend, Backend, DB)
3. Isolate sensitive data
4. Internal microservices communication
5. Secure enterprise networks
6. Hybrid cloud setup
7. VPN connections
8. Load balancer setups
9. API backend isolation
10. Zero-trust architecture

---

## 🧠 What I Learned

* VPC fundamentals
* Subnet types
* Internet Gateway & NAT
* Network security layers

---
# 🚀 Mini Project – VPC Architecture Setup

## 📌 Objective

Design a secure cloud network using VPC with public and private subnets.

---

## 🏗️ Architecture

* Public Subnet → Web Server (EC2)
* Private Subnet → Backend / Database
* Internet Gateway → Internet access
* NAT Gateway → Private subnet outbound access

---

## ⚙️ Steps

1. Create VPC (10.0.0.0/16)
2. Create Subnets:

   * Public Subnet (10.0.1.0/24)
   * Private Subnet (10.0.2.0/24)
3. Attach Internet Gateway
4. Create Route Table:

   * Public → IGW
5. Launch EC2 in Public Subnet
6. (Optional) Setup NAT Gateway for Private Subnet

---

## 🔐 Security

* Allow HTTP/SSH in Security Group
* Keep DB in private subnet

---

## 🌍 Outcome

* Public EC2 accessible from internet
* Private resources secured

---

## 🧠 Learning

* Real VPC architecture
* Subnet isolation
* Secure networking

---

## 🚀 Next Step (Day 06)

* Databases (RDS, DynamoDB)

---

## 📌 Author

**Sankar S**
Cloud & AI Learning Journey 🚀
