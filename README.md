Gym Management System

A Java-based Gym Management System with both Console and Swing GUI interfaces. This project uses JDBC with MySQL to manage gym operations like members, trainers, and workouts.

📌 Features
🔹 Console Application
View Members
View Trainers
View Workouts
Add Member
Update Member Fee
Delete Member
🔹 GUI Application (Swing)
Tab-based interface:
Members
Trainers
Workouts
Perform CRUD operations:
Add
Update
Delete
Load Data
User-friendly dialog input using JOptionPane
🛠️ Technologies Used
Java (Core + Swing)
JDBC (Java Database Connectivity)
MySQL Database
AWT & Swing for GUI
🗄️ Database Setup
1. Create Database
CREATE DATABASE project;
USE project;
2. Create Tables
Member Table
CREATE TABLE member (
    member_id VARCHAR(10) PRIMARY KEY,
    name VARCHAR(50),
    age INT,
    plan VARCHAR(20),
    fee INT
);
Trainer Table
CREATE TABLE trainer (
    trainer_id VARCHAR(10) PRIMARY KEY,
    name VARCHAR(50),
    specialization VARCHAR(50)
);
Workout Table
CREATE TABLE workout (
    workout_id VARCHAR(10) PRIMARY KEY,
    member_id VARCHAR(10),
    type VARCHAR(50),
    duration INT
);
⚙️ Configuration

Update your database credentials in both files:

static final String DB_URL = "jdbc:mysql://localhost:3306/project";
static final String USER = "root";
static final String PASS = "dbms";
▶️ How to Run
1. Compile
javac GymManagementSystem.java
javac GymManagementGUI.java
2. Run Console Version
java GymManagementSystem
3. Run GUI Version
java GymManagementGUI

💡 Key Concepts Used
JDBC Connection
PreparedStatement
ResultSet Handling
Swing Components (JFrame, JTable, JButton)
Event Handling
MVC-like structure
🚀 Future Enhancements
Login Authentication System
Payment Tracking
Attendance Management
Search & Filter Options
Reports & Analytics
👩‍💻 Author
Kaviyarasi
