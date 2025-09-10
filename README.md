# Internship Task-2: Basic CRUD Application (PHP + MySQL)

This repository contains the code for **Task-2** of the ApexPlanet Web Development Internship.  
The task was to build a **Basic CRUD (Create, Read, Update, Delete) Application** with **User Authentication** using PHP and MySQL.

---

## 🚀 Features
- **User Registration** (with password hashing for security)  
- **User Login & Logout** (session-based authentication)  
- **Create Post** (add new blog posts)  
- **Read Posts** (list all posts with timestamp)  
- **Update Post** (edit existing posts)  
- **Delete Post** (remove posts)  

---

## 🗄️ Database Setup
Run the following SQL in **phpMyAdmin** or MySQL CLI:

```sql
CREATE DATABASE blog;
USE blog;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(100) UNIQUE,
    password VARCHAR(255) NOT NULL
);

CREATE TABLE posts (
    id INT AUTO_INCREMENT PRIMARY KEY,
    title VARCHAR(255) NOT NULL,
    content TEXT NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
# task-2
