
# 🧑‍🎓 Student Management System – Java + JDBC + MySQL

A **console-based CRUD application** to manage student records, built using **Java**, **JDBC**, and **MySQL**.

---

## 📌 Features

- ➕ Add new students
- 📋 View all student records
- 🔍 Search student by ID
- ✏️ Update student by ID
- ❌ Delete student by ID
- 💾 Persistent storage using MySQL

---

## 🛠 Tech Stack

- **Java** (Console App)
- **MySQL** (Database)
- **JDBC** (Java Database Connectivity)
- **VS Code** + Extensions
- Git + GitHub

---

## 🗃️ Database Setup

Run these queries in MySQL Shell or any SQL client:

```sql
CREATE DATABASE studentdb;
USE studentdb;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    grade VARCHAR(10)
);
