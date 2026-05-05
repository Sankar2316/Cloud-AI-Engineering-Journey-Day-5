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

## 🚀 Next Step (Day 06)

* Databases (RDS, DynamoDB)

---

## 📌 Author

**Sankar S**
Cloud & AI Learning Journey 🚀
