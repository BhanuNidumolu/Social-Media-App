 🌐 Social Media App (Spring Boot)

![Java](https://img.shields.io/badge/Java-21-orange?logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.0-brightgreen?logo=springboot)
![Maven](https://img.shields.io/badge/Maven-Build-blue?logo=apachemaven)
![Database](https://img.shields.io/badge/Database-MySQL%2FPostgres-blue?logo=mysql)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Contributions](https://img.shields.io/badge/Contributions-Welcome-purple)

A **social media backend application** built with **Spring Boot**, enabling users to share posts, like, and comment.  
This project is designed to showcase **REST API development, JWT authentication, and relational database modeling** for a social networking platform.

---

## 📸 Screenshots

### 🔑 Authentication
<img width="1811" height="918" alt="image" src="https://github.com/user-attachments/assets/c43e9607-7349-4801-bc0e-3875fb0f9604" />


### 📝 Posts
<img width="1353" height="919" alt="image" src="https://github.com/user-attachments/assets/40b64706-cd14-4c65-9b2e-f7db27d6dcac" />


### 💬 Comments
<img width="1762" height="956" alt="image" src="https://github.com/user-attachments/assets/7e8f3c97-9905-4f0e-918e-e78de1c853b3" />


---

## ✨ Features

- 🔐 **User Authentication** – Register, Login with JWT  
- 📝 **Posts** – Create, update, delete, and fetch text posts  
- ❤️ **Likes** – Like/unlike posts  
- 💬 **Comments** – Comment on posts  
- 👤 **User Profiles** – View user posts and activity  
- 📰 **Feed** – Get posts sorted by latest  

---

## 🛠️ Tech Stack

- **Backend:** Spring Boot, Spring Security, JPA/Hibernate  
- **Database:** MySQL / PostgreSQL  
- **Build Tool:** Maven  
- **Authentication:** JWT (JSON Web Tokens)  
- **API Documentation:** Swagger (optional)  
- **Frontend (optional):** React / Angular / Thymeleaf  

---

## 📂 Project Structure
```
social-media-app/
├── src/main/java/com/example/socialmedia/
│ ├── controller/ # REST controllers
│ ├── model/ # Entities (User, Post, Comment, Like)
│ ├── repository/ # Spring Data JPA interfaces
│ ├── service/ # Business logic
│ └── SocialMediaApp.java # Entry point
│
├── src/main/resources/
│ └── application.properties # DB & JWT configs
│
├── docs/screenshots/ # Screenshots for README
├── pom.xml # Maven config
└── README.md
```
yaml
Copy code

---

## 🚀 Getting Started

### ✅ Prerequisites
- Java 17+  
- Maven  
- MySQL/PostgreSQL  

### ⚙️ Setup

1. **Clone the repo**
   ```bash
   git clone https://github.com/BhanuNidumolu/Social-Media-App.git
   cd Social-Media-App
Configure Database (application.properties)

properties
Copy code
spring.datasource.url=jdbc:mysql://localhost:3306/socialmedia
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
Run the application

bash
Copy code
mvn spring-boot:run
Visit API at 👉 http://localhost:8080/api/

📌 API Endpoints
🔑 Authentication
POST /api/auth/register → Register user

POST /api/auth/login → Authenticate & receive JWT

📝 Posts
POST /api/posts → Create post

GET /api/posts → Fetch all posts

DELETE /api/posts/{id} → Delete post

❤️ Likes
POST /api/posts/{id}/like → Like/unlike a post

💬 Comments
POST /api/posts/{id}/comments → Add comment

GET /api/posts/{id}/comments → Fetch comments

🗂️ Database Schema (Simplified ERD)
bash
Copy code
Users (id, username, email, password, created_at)
Posts (id, user_id, content, created_at)
Likes (id, user_id, post_id)
Comments (id, post_id, user_id, content, created_at)
📖 Documentation
Swagger UI available at: http://localhost:8080/swagger-ui.html (if enabled)

API collection can be imported into Postman for testing.

🤝 Contributing
Contributions are welcome!

Fork the repo

Create a feature branch: git checkout -b feature/new-feature

Commit changes: git commit -m "Add new feature"

Push branch: git push origin feature/new-feature

Open a Pull Request 🚀

📜 License
This project is licensed under the MIT License.

👨‍💻 Author
 Bhanu Nidumolu 🚀

yaml
Copy code

---
