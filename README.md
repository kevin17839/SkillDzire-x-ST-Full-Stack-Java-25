# 👨‍💻 SkillDzire x ST – Full Stack Java Internship 2025

Welcome to my repository for the **SkillDzire Technologies x ST Full Stack Java Internship (May-June 2025)**.  
This repository serves as a portfolio of my work throughout the internship — from hands-on backend APIs to full-stack projects with modern Java tech.

> 🎓 This internship is part of my Summer Training from **G. Pulla Reddy Engineering College**, Department of Computer Science and Engineering.  
> I am currently a final-year undergraduate with a strong interest in backend development and Java ecosystems.

---

## 🧑‍🎓 Intern Details

- **Name:** Somapuram Uday  
- **Roll No:** 229X1A2856  
- **Branch:** Computer Science and Technology  
- **Department:** Computer Science and Engineering  
- **Organization:** SkillDzire Technologies Pvt. Ltd.  
- **Internship Title:** Full Stack Java Training  
- **Batch:** May 2025

---

## 📁 Project 1: Student Management System (Spring MVC + MySQL)

### 📌 Project Description

This project is a **Student Management System** built using the **Spring MVC** framework, implementing the **Model-View-Controller** design pattern.  
It performs core CRUD operations — listing, adding, and deleting student records from a MySQL database.

> ✅ Developed as part of **Module: Design Student Schema & Backend APIs (CRUD)** during the Full Stack Java Internship.

---

### 🧱 Tech Stack

| Layer     | Technology                              |
|-----------|------------------------------------------|
| 🧠 Backend   | Java, Spring MVC, JdbcTemplate           |
| 🎨 Frontend | JSP (Java Server Pages), HTML, CSS       |
| 🧰 Build    | Maven                                    |
| 💾 Database | MySQL (XAMPP)                            |
| 🌐 Server   | Jetty (embedded via Maven)               |

---

### 📂 Project Structure

```
student-management/
├── pom.xml
├── README.md
├── src/
│   └── main/
│       ├── java/
│       │   └── com/studentapp/
│       │       ├── config/        # DB & Spring Config
│       │       ├── controller/    # MVC Controllers
│       │       ├── dao/           # DAO + Implementation
│       │       └── model/         # Student POJO
│       └── webapp/
│           └── WEB-INF/
│               ├── views/         # JSP Pages
│               └── web.xml        # DispatcherServlet config
```

---

### ⚙️ Features

- 🔍 View student list  
- ➕ Add a new student  
- ❌ Delete student entries  
- ✅ Backend via Spring JdbcTemplate  
- 🧩 Clean MVC separation  
- ⚡ Deployed on embedded Jetty server for fast local testing

---

### 🧠 Database Setup

Ensure **MySQL is running via XAMPP**, then:

```sql
CREATE DATABASE student_management;

USE student_management;

CREATE TABLE students (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100),
  course VARCHAR(50),
  age INT
);

INSERT INTO students (name, email, course, age) VALUES
('Uday', 'uday@example.com', 'CST', 21),
('Bhavana', 'bhavana@example.com', 'AI', 22);
```

---

### 🧪 How to Run

> 💡 Prerequisites: Java, Maven, XAMPP, Internet Browser

```bash
# Navigate to project folder
cd STUDENT-MANAGEMENT

# Build the project
mvn clean install

# Run Jetty server
mvn jetty:run
```

Then open your browser at:

```
http://localhost:8080/students/
```

---

### 🔗 Links

- 📹 [Project Demo on YouTube](https://youtu.be/AlpD1JL8sf0?si=3fQ4LS5fiu6uL4OH)
- 💻 [View Source on GitHub](https://github.com/udaycodespace/SkillDzire-x-ST-Full-Stack-Java-25/tree/main/student-management)

---

## 📁 Project 2: Authentication System using JWT (Spring Boot)

### 📌 Project Description

This project implements a secure **Authentication System** using **Spring Boot** and **JWT (JSON Web Tokens)**.  
It includes APIs for user registration and login and returns a signed JWT token to be used in subsequent API calls.

> ✅ Developed as part of **Module: Build Auth System with JWT (Register/Login/Logout)** during the Full Stack Java Internship.

---

### 🧱 Tech Stack

| Component   | Technology                              |
|------------|------------------------------------------|
| 🧠 Backend     | Java, Spring Boot, Spring Security        |
| 🔐 Auth       | JWT (JSON Web Tokens)                    |
| 📄 API Format | JSON (RESTful API)                       |
| 🧰 Build      | Maven                                    |
| 💾 Database   | MySQL (via XAMPP)                        |
| 🔬 Testing    | Postman                                  |

---

### 📂 Project Structure

```
PROJECT-2-AUTH-SYSTEM-JWT/
├── pom.xml
├── README.md
├── src/
│   └── main/
│       ├── java/
│       │   └── com/authapp/
│       │       ├── config/        # JWT and Security Configuration
│       │       ├── controller/    # Auth Controller
│       │       ├── dto/           # Request and Response DTOs
│       │       ├── model/         # User Entity
│       │       ├── repo/          # Spring Data JPA Repository
│       │       └── service/       # UserService + JWT Service
│       └── resources/
│           └── application.properties
```

---

### 🔐 API Endpoints

- **POST** `/api/auth/register` – Register a new user  
- **POST** `/api/auth/login` – Login and receive JWT token  
- **GET** `/api/protected` – Example of a protected route (JWT required)

---

### 🧪 How to Run

> 💡 Prerequisites: Java, Maven, XAMPP, Postman

```bash
# Navigate to the project folder
cd PROJECT-2-AUTH-SYSTEM-JWT

# Build and run the Spring Boot app
mvn clean install
mvn spring-boot:run
```

API will run at:

```
http://localhost:8080/
```

Use **Postman** to test endpoints.

---

### 🔗 Links

- 💻 [View Source on GitHub](https://github.com/udaycodespace/SkillDzire-x-ST-Full-Stack-Java-25/tree/main/Project-2-Auth-System-JWT)

---

## 🏁 Conclusion

These projects reflect my internship journey through:

- Spring MVC and Spring Boot ecosystem  
- MySQL backend integration  
- Real-world authentication with JWT  
- RESTful API development and testing with Postman

> Stay tuned for more projects and improvements in this repository!