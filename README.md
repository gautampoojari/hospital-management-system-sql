<div align="center">

# 🏥 Hospital Management System Database

### MySQL Database Project for Hospital Operations Management

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=24&pause=1000&color=36BCF7&center=true&vCenter=true&width=600&lines=Hospital+Management+System;MySQL+Database+Project;Relational+Database+Design;Built+with+MySQL+Workbench" alt="Typing SVG" />

<br>

![MySQL](https://img.shields.io/badge/MySQL-Database-blue?style=for-the-badge\&logo=mysql)
![SQL](https://img.shields.io/badge/SQL-Queries-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Project-Completed-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

</div>

---

# Hospital Management System Database

## 📌 Project Overview

The Hospital Management System is a relational database project developed using MySQL to efficiently manage hospital operations, including doctors, patients, nurses, appointments, and payment records.

This project demonstrates database design concepts such as table creation, primary keys, foreign keys, relationships, normalization, and SQL queries used in real-world healthcare management systems.

---

## 🚀 Technologies Used

* MySQL
* MySQL Workbench
* SQL (DDL & DML)

---

## 🗄️ Database Structure

### Doctor Table

Stores information about hospital doctors.

**Attributes:**

* Doctor_ID (Primary Key)
* Doctor_Name
* Specialization
* Phone_Number
* Email

### Patient Table

Stores patient records.

**Attributes:**

* Patient_ID (Primary Key)
* Patient_Name
* Date_Of_Birth
* Gender
* Phone_Number

### Nurse Table

Stores nurse information.

**Attributes:**

* Nurse_ID (Primary Key)
* Nurse_Name
* Gender
* Age
* Contact_Number

### Appointment Table

Manages appointment scheduling between doctors and patients.

**Attributes:**

* Appointment_ID (Primary Key)
* Appointment_Date
* Appointment_Time
* Doctor_ID (Foreign Key)
* Patient_ID (Foreign Key)

### Payment Table

Stores payment details related to patient services and appointments.

**Attributes:**

* Payment_ID (Primary Key)
* Patient_ID (Foreign Key)
* Payment_Amount
* Payment_Date
* Payment_Method

---

## 🔗 Database Relationships

* One Doctor can manage multiple Appointments.
* One Patient can book multiple Appointments.
* Appointment records connect Doctors and Patients through Foreign Keys.
* Payment records are linked to Patients.
* Relational integrity is maintained using Primary and Foreign Key constraints.

---

## ✨ Key Features

* Doctor Information Management
* Patient Record Management
* Nurse Data Management
* Appointment Scheduling System
* Payment Tracking and Management
* Relational Database Design
* Data Integrity through Constraints
* SQL Query Execution and Data Retrieval

---

## 📊 Entity Relationship Diagram (ERD)

<p align="center">
  <img src="https://github.com/user-attachments/assets/8aa0e40b-4ff8-4c6c-ac73-7b9fd94ac300" >
</p>

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/hospital-management-system-database.git
```

### 2. Open MySQL Workbench

Create a new database:

```sql
CREATE DATABASE hospital;
USE hospital;
```

### 3. Import SQL Script

1. Open MySQL Workbench
2. Navigate to **File → Open SQL Script**
3. Select `hospital.sql`
4. Execute the script to create all tables and insert sample data

---

## 🔍 Sample SQL Queries

### View All Doctors

```sql
SELECT * FROM doctor;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/3abee984-674f-454f-bf97-04cf64aef4f1" >
</p>


### View All Patients

```sql
SELECT * FROM patient;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/0b6c8e52-fdba-4357-9f71-00d0337880e3" >
</p>


### View Appointments

```sql
SELECT * FROM appointment;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/6449a63a-0f24-4405-9aa9-051fd8ba6716" >
</p>


### View Payment Records

```sql
SELECT * FROM payment;
```
<p align="center">
  <img src="https://github.com/user-attachments/assets/89b41774-d865-4395-90b6-5a48474908b3" >
</p>


### Find Appointments with Doctor and Patient Details

```sql
SELECT
a.Appointment_ID,
a.Appointment_Date,
d.Doctor_Name,
p.Patient_Name
FROM appointment a
JOIN doctor d ON a.Doctor_ID = d.Doctor_ID
JOIN patient p ON a.Patient_ID = p.Patient_ID;
```

---

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

* Relational Database Design
* Primary Key & Foreign Key Implementation
* SQL Table Creation
* Data Manipulation and Retrieval
* Query Optimization Basics
* Database Relationship Management
* Real-World Healthcare Data Modeling

---

## 👨‍💻 Author

**Gautam Poojari**

B.Sc. Information Technology Graduate

Aspiring Full Stack Developer

Thane, India

⭐ If you found this project useful, consider giving it a star.

