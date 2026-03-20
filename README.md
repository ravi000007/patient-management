# 🏥 Patient Management System (Microservices Architecture)

A scalable **microservices-based backend system** built using **Spring Boot**, demonstrating real-world backend architecture with **gRPC, Kafka, API Gateway, and JWT authentication**.

---

## 🚀 Tech Stack

- **Backend:** Java, Spring Boot
- **Communication:** gRPC (sync), Apache Kafka (async)
- **Security:** Spring Security, JWT
- **API Gateway:** Spring Cloud Gateway
- **Database:** MySQL
- **Containerization:** Docker
- **Documentation:** Swagger (OpenAPI)

---

## 🧠 Architecture Overview

This system is designed using a **microservices architecture**, where each service is independently deployable and communicates via efficient protocols.

### 🔹 Services:

- **Patient Service** → Handles patient CRUD operations  
- **Billing Service** → Manages billing logic (via gRPC)  
- **Analytics Service** → Consumes Kafka events for data processing  
- **Auth Service** → Handles authentication & JWT token generation  
- **API Gateway** → Single entry point for routing & security  

---

## 🔄 Communication Flow

1. Client sends request → **API Gateway**
2. Gateway validates JWT → routes request
3. Patient Service:
   - Calls **Billing Service via gRPC**
   - Publishes events to **Kafka**
4. Analytics Service consumes Kafka events
5. Response returned via Gateway

---

## 🔐 Authentication Flow

- User logs in via **Auth Service**
- Receives **JWT token**
- Token is validated at **API Gateway**
- Secured endpoints accessed via token

---

## ⚙️ Features

- ✅ Microservices architecture with modular design  
- ✅ gRPC-based inter-service communication  
- ✅ Event-driven architecture using Kafka  
- ✅ Secure authentication using JWT  
- ✅ Centralized routing via API Gateway  
- ✅ Request validation and global exception handling  
- ✅ Integration testing for core APIs  
- ✅ Dockerized services for easy deployment  

---

## 📂 Project Structure
## 🐳 Running the Project (Docker)

### Step 1: Clone the repository
### Step 2: Start services


### Step 3: Access services
- API Gateway → http://localhost:8080
- Swagger Docs → http://localhost:8080/swagger-ui.html

---

## 🧪 Testing

- Integration tests implemented for:
  - Authentication APIs
  - Patient APIs
- Can be run using:

  
---

## 📊 Key Learnings

- Designing scalable microservices architecture  
- Implementing async communication with Kafka  
- Using gRPC for efficient service-to-service calls  
- Securing APIs using JWT and Spring Security  
- Dockerizing and orchestrating multiple services  

---

## 🚀 Future Improvements

- Add Redis caching  
- Implement service discovery (Eureka)  
- Add centralized logging (ELK stack)  
- Add monitoring (Prometheus + Grafana)  

---

## 👨‍💻 Author

**Ravi Singh**  
- LinkedIn: https://linkedin.com/in/ravi-singh-22319b1b4  
- Email: rssingh8736@gmail.com  

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
