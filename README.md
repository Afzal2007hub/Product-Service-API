# 🛍️ Spring Boot Product Service API

A RESTful Product Service built using **Spring Boot** that provides CRUD operations for managing product information. This project is part of a **Microservices Architecture** and can communicate with other services such as **Customer Service** through REST APIs.

---

## 🚀 Features

- ➕ Add a Product
- 📄 View All Products
- 🔍 View Product by ID
- ✏️ Update Product Details
- ❌ Delete a Product
- 💾 H2 In-Memory Database
- 🗃️ Spring Data JPA
- 🌐 RESTful APIs
- 📦 Maven Project

---

## 🛠️ Technologies Used

- Java 17
- Spring Boot
- Spring Web
- Spring Data JPA
- H2 Database
- Maven
- REST API
- IntelliJ IDEA / Eclipse

---

## 📂 Project Structure

```
Spring-boot-ProductService-Api
│
├── src
│   ├── main
│   │   ├── java
│   │   │   ├── controller
│   │   │   ├── entity
│   │   │   ├── repository
│   │   │   ├── service
│   │   │   └── ProductServiceApplication.java
│   │   │
│   │   └── resources
│   │       ├── application.properties
│   │
│   └── test
│
├── pom.xml
└── README.md
```

---

## ⚙️ Prerequisites

Before running the project, ensure you have installed:

- Java 17 or later
- Maven
- IntelliJ IDEA / Eclipse
- Git

---

## 📥 Clone the Repository

```bash
git clone https://github.com/<your-username>/Spring-boot-ProductService-Api.git
```

Navigate to the project:

```bash
cd Spring-boot-ProductService-Api
```

---

## ▶️ Run the Application

Using Maven:

```bash
mvn spring-boot:run
```

Or from your IDE, run:

```
ProductServiceApplication.java
```

---

## 🌐 Server

```
http://localhost:8081
```

*(Change the port if configured differently in `application.properties`.)*

---

## 🗄️ H2 Database

Open your browser:

```
http://localhost:8081/h2-console
```

Example configuration:

| Property | Value |
|----------|-------|
| JDBC URL | jdbc:h2:mem:productdb |
| Username | sa |
| Password | *(leave empty)* |

---

## 📡 REST API Endpoints

### Get All Products

```
GET /products
```

### Get Product by ID

```
GET /products/{id}
```

### Add Product

```
POST /products
```

Sample JSON

```json
{
  "productName": "Laptop",
  "price": 65000,
  "quantity": 10
}
```

### Update Product

```
PUT /products/{id}
```

### Delete Product

```
DELETE /products/{id}
```

---

## 🧪 Testing

You can test the APIs using:

- Postman
- Swagger (if configured)
- cURL

Example:

```bash
curl http://localhost:8081/products
```

---

## 🔗 Microservices

This Product Service can be integrated with:

- Customer Service
- API Gateway
- Eureka Server
- Config Server

Typical architecture:

```
Client
   │
   ▼
API Gateway
   │
   ├──────────────┐
   ▼              ▼
Customer      Product
 Service       Service
```

---

## 📌 Future Enhancements

- Spring Cloud Gateway
- Eureka Discovery Server
- OpenFeign
- MySQL / PostgreSQL
- Docker
- Kubernetes
- JWT Authentication
- Swagger/OpenAPI Documentation
- Resilience4j Circuit Breaker

---

## 👨‍💻 Author

**Afzal**

BTech IT Student

Learning Spring Boot, Java, and Microservices.

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub!

---

## 📄 License

This project is intended for educational and learning purposes.
