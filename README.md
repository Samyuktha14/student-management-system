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

## 🔐 Secure DB Credentials (Recommended)

To **hide your MySQL password**, use a `.properties` config file.

### Step 1: Create `dbconfig.properties` in your `src/` folder:

```properties
db.url=jdbc:mysql://localhost:3306/studentdb
db.user=root
db.password=your_mysql_password
