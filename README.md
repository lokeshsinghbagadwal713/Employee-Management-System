
# 📌 Employee Management System

A **console-based Java application** to manage employee records including creating, viewing, updating, and deleting employees using a **MySQL database via JDBC**.

---

## 🚀 Features

* ➕ Add New Employees
* 📋 View All Employees
* 🔎 Search Employee by ID
* ✏️ Update Employee Details
* ❌ Delete Employee Records
* 💾 Persistent storage using MySQL via JDBC
* 🛠️ Implements DAO (Data Access Object) Pattern

---

## 🛠️ Tech Stack

* **Java** (OOP + Modular Architecture)
* **MySQL** for data storage
* **JDBC** for database connectivity
* **DAO Design Pattern**

---

## 📁 Project Structure

```
Employee-Management-System/
├── src/com/employee/empapp/
│   ├── DBConnection.java      # Database connectivity (JDBC + MySQL)
│   ├── Employee.java          # Employee model class
│   ├── EmployeeDao.java       # DAO Interface
│   ├── EmployeeDaoImpl.java   # DAO Implementation (CRUD logic)
│   ├── Main.java              # Entry point (menu-driven program)
├── Employee Management System.iml
├── .gitignore
├── README.md
```

---

## ⚙️ How to Run

### 1. Compile the Project

```bash
javac -d out -cp src src\com\employee\empapp\*.java
```

### 2. Run the Application

```bash
java -cp out com.employee.empapp.Main
```

### 3. MySQL Database Setup

Open MySQL CLI or a GUI tool (like MySQL Workbench or phpMyAdmin).

Create a new database:

```sql
CREATE DATABASE employee_db;
```

Create the `employees` table:

```sql
CREATE TABLE employees (
  id INT PRIMARY KEY,
  name VARCHAR(100),
  department VARCHAR(50),
  salary DOUBLE
);
```

Update `DBConnection.java` with your MySQL credentials:

```java
String url = "jdbc:mysql://localhost:3306/employee_db";
String user = "root";      // your MySQL username
String password = "root";  // your MySQL password
```

---

## ✍️ Author

Lokesh Singh Bagadwal
📍 Dehradun, India

---

## 📄 License

This project is licensed under the **MIT License** – feel free to use and modify.


