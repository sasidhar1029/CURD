📘 JDBC Student Management System

This is a console-based Java application built using JDBC that performs basic CRUD operations (Create, Read, Update, Delete) on a students table in a MySQL database.

🛠️ Technologies Used

Java (Core Java)

JDBC (Java Database Connectivity)

MySQL

MySQL Connector/J

Eclipse / IntelliJ IDEA

Command Line (Console Input)

📂 Project Structure
jdbcProject
│
├── DBConnection.java
├── InsertStudent.java
├── ViewStudents.java
├── SelectById.java
├── UpdateStudents.java
├── DeleteStudents.java
└── StudentDriverClass.java

📌 Database Details

Database Name: sasidharreddy
Table Name: students

📄 Table Structure
CREATE TABLE students (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    branch VARCHAR(50)
);

🔗 Database Connection

All database connectivity is handled in the DBConnection class.

DriverManager.getConnection(
    "jdbc:mysql://localhost:3306/sasidharreddy",
    "root",
    "root"
);

🚀 Features (CRUD Operations)
1️⃣ Insert Student

Class: InsertStudent

Takes student id, name, and branch

Inserts data into the students table

2️⃣ View All Students

Class: ViewStudents

Fetches and displays all records from the table

3️⃣ Select Student by ID

Class: SelectById

Fetches a student using ID

Displays message if record not found

4️⃣ Update Student

Class: UpdateStudents

Updates name and branch based on ID

5️⃣ Delete Student

Class: DeleteStudents

Deletes a student record using ID

▶️ How to Run the Project

Import the project into Eclipse / IntelliJ

Add MySQL Connector JAR to the project build path

Ensure MySQL server is running

Create database and table as mentioned above

Run StudentDriverClass.java

🧪 Execution Flow

When you run StudentDriverClass, the following operations execute sequentially:

Insert Student

View All Students

Select Student by ID

Update Student

Delete Student

⚠️ Important Notes

User input is taken using Scanner

Database connection errors are handled using try-catch

PreparedStatement is used to prevent SQL Injection

Connections are reused via DBConnection class

✅ Sample Output
Enter user id: 1
Enter user name: Sasi
Enter user Branch: CSE
1 Rows inserted

1 Sasi CSE

Enter an id: 1
1 Sasi CSE

1 rows updated

1 rows deleted

📈 Future Enhancements

Menu-driven program (switch case)

Close resources using finally or try-with-resources

Exception custom handling

Convert to GUI / Web Application

Add validation for duplicate IDs

👨‍💻 Author

Korrapolu Sasidhar Reddy
Java Full Stack Learner
