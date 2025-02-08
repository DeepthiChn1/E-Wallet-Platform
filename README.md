# 💰 E-Wallet Platform  

## 📌 Overview  
The **E-Wallet Platform** is a digital wallet system that enables users to **send and receive money securely**, view transaction history, and manage accounts. Built using **Spring Boot microservices architecture**, it ensures **scalability, security, and seamless financial transactions**.

---

## **🚀 Features**
✅ **P2P Transfers** – Send money to other registered users  
✅ **Wallet Management** – Check balance, view transaction history  
✅ **Email Notifications** – Get notified for every transaction  
✅ **Secure Authentication** – OAuth2 & Spring Security  
✅ **Admin Controls** – Fetch user details (Admin Only)  

---

## **🛠️ Tech Stack**
- **Backend:** Spring Boot (Microservices)  
- **Event Streaming:** Apache Kafka  
- **Security:** OAuth2, Spring Security  
- **Database:** MySQL / PostgreSQL (per microservice)  
- **API Management:** Spring Cloud Gateway  

---

## **📌 API Endpoints**
### **Transaction Controller**
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/txn` | `POST` | Initiate a P2P transaction |

### **User Controller**
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/user` | `POST` | Register a new user |
| `/user` | `GET` | Fetch authenticated user details |
| `/admin/all/users` | `GET` | Get details of all users (Admin Only) |
| `/admin/user/{id}` | `GET` | Fetch specific user details (Admin Only) |

---

<!-- ## **📥 Setup & Installation**

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/DeepthiChn1/E-Wallet-Platform.git
cd E-Wallet-Platform
2️⃣ Configure Databases
Ensure MySQL or PostgreSQL is installed and running.
Create separate databases for each microservice:

sql
Copy
Edit
CREATE DATABASE user_service_db;
CREATE DATABASE transaction_service_db;
CREATE DATABASE wallet_service_db;
CREATE DATABASE notification_service_db;
Update application.properties in each microservice with the correct database credentials:

properties
Copy
Edit
spring.datasource.url=jdbc:mysql://localhost:3306/user_service_db
spring.datasource.username=root
spring.datasource.password=yourpassword
3️⃣ Ensure Kafka is Running
Start Apache Kafka before running the services:

bash
Copy
Edit
kafka-server-start.sh config/server.properties
If using Docker, start Kafka with:

bash
Copy
Edit
docker-compose up -d
4️⃣ Run Each Microservice
Navigate to each service folder and start them:

bash
Copy
Edit
cd user-service && mvn spring-boot:run
cd ../transaction-service && mvn spring-boot:run
cd ../wallet-service && mvn spring-boot:run
cd ../notification-service && mvn spring-boot:run
📜 License
This project is MIT Licensed – feel free to modify and use it. -->