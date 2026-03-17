# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: MYVIZHI S
* **Register Number**: 212224040209
* **Date of Submission**:17.03.2026

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1. I logged in to the **AWS Management Console** and launched an **EC2 instance** using Amazon Linux 2.
2. I configured the **security group** to allow **SSH (port 22)** and **database port (3306/5432)** access.
3. I connected to the EC2 instance using **SSH** from my local machine.
4. I installed a **database server (MySQL/MariaDB/PostgreSQL)** and started the service.
5. I created a **sample database, table, inserted records**, and tested the database using **SQL queries**.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server

<img width="1919" height="1139" alt="Screenshot 2026-03-15 134924" src="https://github.com/user-attachments/assets/fc732f5c-13be-4bcc-afc6-4674f5c420f5" />

---

### Screenshot 2: Database Service Running
<img width="1918" height="1135" alt="Screenshot 2026-03-15 140034" src="https://github.com/user-attachments/assets/568fb5f5-b386-4cbf-8c6d-8df5ff267609" />


---

### Screenshot 3: Sample Database and Table

<img width="1919" height="1085" alt="Screenshot 2026-03-15 140612" src="https://github.com/user-attachments/assets/2b7a8d88-460a-49ac-8b8f-e236fa22c0ea" />


---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were understand.
