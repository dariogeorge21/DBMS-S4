<div align="center">

# 🗄️ Database Management Systems (DBMS) Lab - S4

![DBMS](https://img.shields.io/badge/DBMS-Lab%20Course-blue?style=for-the-badge)
![Academic Year](https://img.shields.io/badge/Academic%20Year-2026-green?style=for-the-badge)
![Semester](https://img.shields.io/badge/Semester-S4-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

**A comprehensive repository for Database Management Systems laboratory work**

[📚 About](#-about) • [🎯 Objectives](#-course-objectives) • [🧪 Labs](#-laboratory-exercises) • [🚀 Getting Started](#-getting-started) • [📖 Resources](#-resources)

</div>

---

## 📑 Table of Contents

- [📚 About](#-about)
- [🎯 Course Objectives](#-course-objectives)
- [🧪 Laboratory Exercises](#-laboratory-exercises)
- [📂 Repository Structure](#-repository-structure)
- [🚀 Getting Started](#-getting-started)
- [💡 Key Concepts](#-key-concepts)
- [📖 Resources](#-resources)
- [🤝 Contributing](#-contributing)
- [👤 Author](#-author)

---

## 📚 About

This repository contains laboratory exercises, assignments, and projects for the **Database Management Systems (DBMS)** course taught in **Semester 4 (S4)** of the academic year **2026**. The course emphasizes practical implementation of database concepts, SQL programming, and database design principles through hands-on laboratory work.

### What You'll Find Here

- 📊 **Entity-Relationship Diagrams**: Complete ER diagrams with multiple entities, relationships, and cardinality notations
- 💻 **SQL Scripts**: Comprehensive SQL queries covering DDL and DML operations
- 📸 **Screenshots**: Step-by-step visual documentation of query execution and results
- 📝 **Lab Documentation**: Detailed explanations, objectives, and learning outcomes for each exercise

---

## 🎯 Course Objectives

This course aims to provide students with comprehensive knowledge and practical skills in database management:

| Objective | Description |
|-----------|-------------|
| 🏗️ **Database Design** | Understand and apply fundamental database concepts and design principles |
| 📐 **ER Modeling** | Design and implement Entity-Relationship (ER) diagrams for complex systems |
| 🔍 **SQL Mastery** | Master SQL queries, joins, subqueries, and advanced database operations |
| ⚡ **Optimization** | Learn normalization techniques and database optimization strategies |
| 🛠️ **Application Development** | Develop real-world database applications with proper schema design |
| 🔐 **Security & Transactions** | Implement database security measures and transaction management |

---

## 🧪 Laboratory Exercises

### Lab 1: Entity-Relationship Diagram Design
**📋 Objective:** Design a comprehensive ER diagram for a multi-entity database system

**🔑 Key Topics:**
- Entity-Relationship modeling with multiple entities
- Primary and foreign key relationships
- Cardinality and relationship types
- Database schema design

**📁 Contents:**
- ER diagram visualization (PNG and HTML formats)
- Detailed entity and relationship documentation
- [View Lab 1 →](./lab1)

**🗂️ Schema Overview:**
- **Entities:** EMPLOYEE, DEPARTMENT, PROJECTS, STUDENT, COURSE
- **Relationships:** 
  - WORK (Employees ↔ Departments)
  - ENROLLS (Departments ↔ Projects)
  - enrolls (Students ↔ Courses)

---

### Lab 2: SQL Data Manipulation Language (DML)
**📋 Objective:** Master SQL commands for data manipulation and querying

**🔑 Key Topics:**
- Table creation with constraints (PRIMARY KEY)
- Data insertion and population
- SELECT queries with various filtering conditions
- UPDATE and DELETE operations
- Aggregate functions (SUM, MIN, MAX)
- String manipulation functions (UPPER, REVERSE)
- Pattern matching with LIKE operator

**📁 Contents:**
- Complete SQL scripts for all DML operations
- Step-by-step screenshots demonstrating query execution and results
- [View Lab 2 →](./lab2)

**💡 Skills Practiced:**
- Creating employee tables with primary key constraints
- Inserting and updating employee records
- Complex WHERE clauses with multiple conditions
- Salary calculations and percentage-based updates
- String functions and pattern matching
- Department-wise salary aggregations
- Finding minimum/maximum salary values

---

## 📂 Repository Structure

```
DBMS-S4/
│
├── README.md                          # Main documentation (this file)
│
├── lab1/                              # Lab 1: ER Diagram Design
│   ├── README.md                      # Lab 1 detailed documentation
│   └── lab1 tasks.html               # Lab 1 task specifications
│
├── lab2/                              # Lab 2: SQL DML Operations
│   ├── README.md                      # Lab 2 documentation with all SQL queries
│   └── screenshots/                   # Query execution result screenshots
│
├── ER DIAGRAM lab1.drawio.png        # Lab 1 ER Diagram (PNG format)
└── ER DIAGRAM lab1.html              # Lab 1 ER Diagram (interactive HTML)
```

> 📸 **Note:** Each lab includes detailed screenshots documenting the execution and results of all exercises.

---

## 🚀 Getting Started

### 📋 Prerequisites

Before you begin, ensure you have the following:

- ✅ Basic understanding of database concepts
- ✅ Knowledge of SQL syntax and commands
- ✅ A database management system installed:
  - MySQL (recommended)
  - PostgreSQL
  - Oracle Database
  - SQLite
- ✅ [Draw.io](https://app.diagrams.net/) or compatible software for viewing/editing ER diagrams
- ✅ Text editor or IDE (VS Code, DataGrip, MySQL Workbench, etc.)

### 🔧 Installation & Setup

#### 1️⃣ Clone the Repository

```bash
git clone https://github.com/dariogeorge21/DBMS-S4.git
cd DBMS-S4
```

#### 2️⃣ Set Up Your Database Environment

**For MySQL:**
```sql
-- Create and use the database
CREATE DATABASE dbms_lab;
USE dbms_lab;

-- Follow the lab-specific SQL scripts in each lab folder
-- Example: Execute queries from lab2/README.md
```

**For PostgreSQL:**
```sql
-- Create and connect to the database
CREATE DATABASE dbms_lab;
\c dbms_lab

-- Follow the lab-specific SQL scripts in each lab folder
```

#### 3️⃣ View and Edit ER Diagrams

**View Static Image:**
```bash
# Open the PNG file in your preferred image viewer
open "ER DIAGRAM lab1.drawio.png"
# On Linux: xdg-open "ER DIAGRAM lab1.drawio.png"
# On Windows: start "ER DIAGRAM lab1.drawio.png"
```

**View Interactive Diagram:**
```bash
# Open the HTML file in your web browser
open "ER DIAGRAM lab1.html"
# On Linux: xdg-open "ER DIAGRAM lab1.html"
# On Windows: start "ER DIAGRAM lab1.html"
```

**Edit Diagrams:**
1. Visit [diagrams.net](https://app.diagrams.net/)
2. Click "Open Existing Diagram"
3. Upload the PNG or HTML file
4. Make your modifications
5. Export in your preferred format (PNG, HTML, XML, etc.)

#### 4️⃣ Explore Individual Labs

Navigate to each lab directory for specific instructions and exercises:

```bash
cd lab1  # For ER Diagram design exercises
cd lab2  # For SQL DML operations and queries
```

Each lab folder contains:
- Detailed README with complete instructions
- SQL scripts and queries
- Screenshots of execution results

---

## 💡 Key Concepts

This course covers essential database management concepts:

### 🏗️ Database Design
- **Entity-Relationship Modeling**: Understanding entities, attributes, and relationships
- **Normalization**: 1NF, 2NF, 3NF, and BCNF for optimal database design
- **Schema Design**: Creating efficient and scalable database structures

### 🔑 Data Integrity
- **Primary Keys**: Unique identifiers for database records
- **Foreign Keys**: Establishing and maintaining referential integrity
- **Constraints**: NOT NULL, UNIQUE, CHECK, DEFAULT

### 🔗 Relationships
- **Cardinality**: One-to-one, one-to-many, and many-to-many relationships
- **Participation**: Total vs. partial participation
- **Weak Entities**: Entities dependent on other entities

### 💻 SQL Operations
- **DDL (Data Definition Language)**: CREATE, ALTER, DROP
- **DML (Data Manipulation Language)**: SELECT, INSERT, UPDATE, DELETE
- **Aggregate Functions**: COUNT, SUM, AVG, MIN, MAX
- **Joins**: INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN
- **Subqueries**: Nested queries for complex data retrieval

### ⚡ Optimization
- **Indexing**: Improving query performance
- **Query Optimization**: Writing efficient SQL queries
- **Transaction Management**: ACID properties and concurrency control

---

## 📖 Resources

### 📚 Recommended Documentation

| Resource | Description | Link |
|----------|-------------|------|
| 🎨 **Draw.io** | ER diagram creation tool | [diagrams.net](https://www.diagrams.net/) |
| 📘 **SQL Tutorial** | Comprehensive SQL learning resource | [W3Schools SQL](https://www.w3schools.com/sql/) |
| 📗 **Normalization Guide** | Database normalization explained | [Guru99](https://www.guru99.com/database-normalization.html) |
| 📙 **ER Diagram Best Practices** | ER modeling guidelines | [Lucidchart](https://www.lucidchart.com/pages/er-diagrams) |
| 📕 **MySQL Documentation** | Official MySQL reference | [MySQL Docs](https://dev.mysql.com/doc/) |

### 🎓 Additional Learning Materials

- [Stanford Database Course](https://www.edx.org/course/databases-5-sql) - Free online course
- [PostgreSQL Tutorial](https://www.postgresqltutorial.com/) - Comprehensive PostgreSQL guide
- [SQL Exercises](https://www.sql-practice.com/) - Practice SQL queries online
- [Database Design Tutorial](https://www.tutorialspoint.com/dbms/index.htm) - DBMS fundamentals

---

## 🤝 Contributing

This is an academic repository created for coursework. Contributions, suggestions, and improvements are welcome!

### How to Contribute

1. 🍴 **Fork** the repository
2. 🌿 **Create** a feature branch (`git checkout -b feature/improvement`)
3. ✍️ **Commit** your changes (`git commit -m 'Add some improvement'`)
4. 📤 **Push** to the branch (`git push origin feature/improvement`)
5. 🔃 **Open** a Pull Request

### Contribution Guidelines

- Follow the existing code style and structure
- Add appropriate comments and documentation
- Test your SQL queries before submitting
- Update the README if you add new content
- Include screenshots for visual changes

---

## 👤 Author

**dariogeorge21**

- 📧 GitHub: [@dariogeorge21](https://github.com/dariogeorge21)
- 🗄️ Repository: [DBMS-S4](https://github.com/dariogeorge21/DBMS-S4)

---

## 📄 License

This project is created for academic purposes as part of the Database Management Systems laboratory coursework. Feel free to use this repository as a reference for your learning.

---

<div align="center">

### 📚 Happy Learning! ✨

**Building Strong Foundations in Database Management Systems**

*Semester 4 | Academic Year 2026*

---

⭐ Star this repository if you find it helpful! ⭐

Made with ❤️ for DBMS Students

</div>
