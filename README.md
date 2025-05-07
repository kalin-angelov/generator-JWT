A Java-based web application for user registration, login, and profile editing. This project is built using **Spring Boot**, **Spring Security**, **JWT (JSON Web Token)** for authentication, and **MySQL** for persistent data storage.

---

## 🚀 Features

- 🔐 User Registration  
- 🔓 Secure Login with JWT-based Authentication  
- 📝 Edit Profile Information
- 🛡️ Password Encryption with BCrypt
- 🔑 Secret Key Management via `.env`
- 🌐 RESTful API endpoints  
- 💾 MySQL integration with JPA/Hibernate  

---

## 🧰 Tech Stack

- **Backend**: Java, Spring Boot  
- **Security**: Spring Security, JWT  
- **Database**: MySQL  
- **ORM**: Spring Data JPA  

---

## 📦 Installation

### 1. Download/Clone the repository

### 2. Create and Configure `.env` File
Create a `.env` file in the root directory with the following content:

```bash
  JWT_SECRET_KEY=your_jwt_secret
```

### 3. Configure MySQL
Create a MySQL database and update your application.properties:
   
---

## 📫 API Endpoints

| Method | Endpoint                  | Description                   |
| ------ | ------------------------- | ----------------------------- |
| POST   | `/api/v1/auth/register`   | Register a new user           |
| POST   | `/api/v1/auth/login`      | Login and get JWT token       |
| GET    | `/api/v1/users/profile`   | Get user profile (secured)    |
| PUT    | `/api/v1/users/{id}/edit` | Update user profile (secured) |

JWT token must be sent as Authorization: `Bearer <token>` in secured endpoints.

---

## 🧪 Testing
You can use Postman to test the APIs. Make sure to first register a user, then login to receive the JWT, and use it in subsequent requests.
