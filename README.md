# Student Management System

A full-stack, responsive Student Management System designed to handle complete CRUD (Create, Read, Update, Delete) operations for student profiles. This project features a robust RESTful API backend built with Spring Boot and a dynamic, modern user interface powered by React.

---

## 🚀 Features

* **Full CRUD Functionality:** Dynamically add, view, update, and delete student profiles.
* **Real-Time Notifications:** Integrated UI alerts tracking the status of system actions (success/error states).
* **Responsive Layout:** Adaptive CSS styling optimized across both desktop and mobile screen footprints.
* **Globally Handled Errors:** Backend exception handling that safely catches runtime bugs and serves structured JSON responses.
* **CORS Configured:** Secure cross-origin resource sharing allowing the decoupled frontend to seamlessly hit backend endpoints.

---

## 🛠️ Technology Stack

### Backend
* **Java:** 17+
* **Framework:** Spring Boot 3.2.0 (Spring Data JPA, Spring Web)
* **Database:** MySQL 8.0+
* **Build Tool:** Maven
* **Boilerplate Reduction:** Lombok

### Frontend
* **Library:** React 18+
* **Build & Tooling:** Vite
* **HTTP Client:** Axios
* **Styling:** CSS3 (featuring custom animations and responsive media queries)

---

## 📁 Project Structure

```text
student-management-system/
├── student-management/          # Spring Boot Backend
│   ├── src/main/java/com/example/student/
│   │   ├── config/              # WebConfig.java (CORS Settings)
│   │   ├── controller/          # StudentController.java (REST Endpoints)
│   │   ├── exception/           # GlobalExceptionHandler.java
│   │   ├── model/               # Student.java (JPA Entity)
│   │   ├── repository/          # StudentRepository.java (Data Access)
│   │   └── service/             # Service interfaces and implementations
│   ├── src/main/resources/      # application.properties
│   └── pom.xml
│
└── student-frontend/            # React Frontend (Vite)
    ├── public/
    ├── src/
    │   ├── components/          # StudentForm, StudentList, Notification
    │   ├── services/            # StudentService.js (Axios API configuration)
    │   ├── App.jsx              # Main App Component & state engine
    │   └── main.jsx             # React entry point
    ├── package.json
    └── vite.config.js
