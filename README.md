
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

🧾 Project Structure
pgsql
Copy
Edit
StudentManagementSystem/
├── src/
│   ├── DBConnection.java
│   ├── Student.java
│   ├── StudentDAO.java
│   └── Main.java
├── lib/                       ← Place mysql-connector.jar here
├── bin/                       ← Compiled .class files
├── dbconfig.properties        ← Your local DB credentials (ignored in Git)
├── dbconfig.sample.properties ← Public safe version
├── .gitignore
└── README.md
🚀 How to Run
✅ 1. Clone the repo
bash
Copy
Edit
git clone https://github.com/YOUR_USERNAME/Student-Management-System-Java.git
cd Student-Management-System-Java
✅ 2. Configure MySQL credentials
Create src/dbconfig.properties:

properties
Copy
Edit
db.url=jdbc:mysql://localhost:3306/studentdb
db.user=root
db.password=your_mysql_password
🔐 Don’t commit this file — it's in .gitignore

✅ 3. Add MySQL JDBC driver
Download from: https://dev.mysql.com/downloads/connector/j/

Place the .jar inside the lib/ folder

✅ 4. Compile and Run
bash
Copy
Edit
javac -cp "lib/*" -d bin src/*.java
java -cp "bin;lib/*" Main
