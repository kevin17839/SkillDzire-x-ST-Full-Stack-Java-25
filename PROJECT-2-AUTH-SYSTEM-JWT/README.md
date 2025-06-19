# 🔐 Project 2: Authentication System with JWT

> Developed as part of SkillDzire’s Full Stack Java Internship Program – May 2025 Batch

## 📌 Project Overview

This project is a secure **Authentication System** built using **Spring Boot** and **JWT (JSON Web Token)**. It handles user registration and login with role-based access control. After a successful login, a JWT is issued, which is used for securing future API requests.

> 🔧 This is part of the module: **“Build Auth System with JWT”** covered during the internship.

---

## 🧱 Tech Stack

| Layer       | Technology                            |
|-------------|----------------------------------------|
| 🧠 Backend     | Java, Spring Boot, Spring Security     |
| 🔐 Auth        | JWT (JSON Web Token)                  |
| 📦 Build Tool | Maven                                 |
| 🗃️ Database    | MySQL                                 |
| 📫 API Test    | Postman                               |

---

## 📂 Folder Structure

```
PROJECT-2-AUTH-SYSTEM-JWT/
├── pom.xml
├── README.md
├── src/
│   └── main/
│       ├── java/
│       │   └── com/example/jwtauth/
│       │       ├── config/          # JWT Security Config
│       │       ├── controller/      # Auth APIs (Login/Register)
│       │       ├── model/           # User entity + DTOs
│       │       ├── repository/      # UserRepository (JPA)
│       │       ├── service/         # UserDetailsService + JWT Utils
│       │       └── JwtAuthApplication.java
│       └── resources/
│           ├── application.properties
│           └── data.sql
```

---

## 🔐 Features

- 👤 Register a new user
- 🔑 Login with username & password
- 🪪 JWT token generation
- ✅ Protect endpoints with token-based access
- 🧩 Role-based access support (ADMIN / USER)
- 📫 Test everything via Postman

---

## 🧪 How to Run

> ✅ Prerequisites: Java 17+, Maven, MySQL, Postman

### 1️⃣ Clone this repository and navigate to the folder

```bash
cd PROJECT-2-AUTH-SYSTEM-JWT
```

### 2️⃣ Setup MySQL

```sql
CREATE DATABASE jwt_auth;

USE jwt_auth;
```

> You can optionally use `data.sql` to preload users.

### 3️⃣ Configure database in `application.properties`

```
spring.datasource.url=jdbc:mysql://localhost:3306/jwt_auth
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

### 4️⃣ Build and run the application

```bash
mvn spring-boot:run
```

Now your backend is running at:

```
http://localhost:8080/
```

---

## 🧪 Postman API Endpoints

### 🔹 Register User

**POST** `/api/auth/register`  
```json
{
  "username": "uday",
  "password": "pass123"
}
```

### 🔹 Login

**POST** `/api/auth/login`  
```json
{
  "username": "uday",
  "password": "pass123"
}
```

Returns:
```json
{
  "token": "eyJhbGciOiJIUzUxMiJ9..."
}
```

Use the token in the `Authorization` header for secured endpoints:
```
Bearer <your-token>
```

---

## ✅ Sample Output

- 200 OK with JWT token
- 403 Forbidden if unauthorized
- Register/login flows tested via Postman

---

## 🔗 Links

- 📹 [YouTube Channel (Demo)](https://www.youtube.com/@udaycodespace)

---

## 🧾 Final Notes

This project showcases:

- Real-world authentication flow in Spring Boot
- Token-based security implementation
- REST API practices with secure role-based routing

> A great foundation for securing full-stack apps and integrating login in frontend frameworks (like React).

---

