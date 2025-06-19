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
cd student-management

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

### 🧾 Sample Output

- ✅ Displays student list in table
- ✏️ Option to add/delete students
- 📁 Data pulled live from MySQL

---

### 🔗 Links

- 📹 [Project Demo on YouTube](https://youtu.be/AlpD1JL8sf0?si=3fQ4LS5fiu6uL4OH)
- 💻 [View Source on GitHub](https://github.com/udaycodespace/SkillDzire-x-ST-Full-Stack-Java-25/tree/main/student-management)

---

## 📅 Internship Timeline Highlights

This project is part of a **multi-week Java internship program** that covered:

| Date         | Topic                                           |
|--------------|--------------------------------------------------|
| 05–10 May    | Java OOPs (Encapsulation, Inheritance, Polymorphism) |
| 14–21 May    | REST APIs, DB Integration, React Frontend         |
| 22–27 May    | Authentication System + React Dashboard           |
| 27–31 May    | Bookstore App with Cart & Payment Integration     |
| 03–07 Jun    | Job Portal + Recruiter Role Management            |
| 10–13 Jun    | Microservices + Docker + REST Gateway             |

> 🧪 Multiple assessments and hands-on modules were conducted throughout the training.

---

## 🔮 What’s Next?

- 🔜 Additional Projects will be added here soon  
- 🧠 Planning to expand this repo into a **multi-project showcase**, with microservices, JWT auth systems, and more React-integrated apps

---

## 🏁 Conclusion

This project serves as a **foundational demonstration** of my skills in:

- Spring MVC architecture  
- Backend-DB integration with JDBC  
- JSP and Servlet-based UI rendering  
- CRUD operations with clean separation of concerns

> It's just the beginning — more complex full-stack builds are on the way!

---
