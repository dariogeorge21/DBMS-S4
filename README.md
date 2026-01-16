# 🗄️ Database Management Systems (DBMS) Lab - S4

<div align="center">

![DBMS](https://img.shields.io/badge/DBMS-Lab%20Course-blue?style=for-the-badge)
![Academic Year](https://img.shields.io/badge/Academic%20Year-2026-green?style=for-the-badge)
![Semester](https://img.shields.io/badge/Semester-S4-orange?style=for-the-badge)

*A comprehensive repository for Database Management Systems laboratory work*

</div>

---

## 📚 About This Repository

This repository contains laboratory exercises, assignments, and projects for the **Database Management Systems (DBMS)** course taught in **Semester 4 (S4)** of the academic year **2026**. The course focuses on practical implementation of database concepts, SQL programming, and database design principles.

## 🎯 Course Objectives

- Understand and apply fundamental database concepts
- Design and implement Entity-Relationship (ER) diagrams
- Master SQL queries and database operations
- Learn normalization and database optimization techniques
- Develop real-world database applications
- Implement database security and transaction management

## 📂 Repository Structure

```
DBMS-S4/
├── README.md                        # This file
├── ER DIAGRAM lab1.drawio.png      # Lab 1 ER Diagram (visual)
└── ER DIAGRAM lab1.html            # Lab 1 ER Diagram (interactive)
```

## 🔬 Laboratory Exercises

### Lab 1: Entity-Relationship Diagram Design

**Objective:** Design a comprehensive ER diagram for a multi-entity database system

**Description:** This lab introduces Entity-Relationship modeling with a complex database schema involving multiple entities and relationships.

#### Database Schema Overview

The ER diagram includes the following entities and their relationships:

##### 📊 Entities

1. **EMPLOYEE**
   - Attributes: `eno` (Employee Number), `name`, `dob` (Date of Birth), `gender`, `panno` (PAN Number), `basic_payee`, `designation`, `doj` (Date of Joining)
   - Primary Key: `eno`

2. **DEPARTMENT**
   - Attributes: `d_no` (Department Number), `dname` (Department Name)
   - Primary Key: `d_no`

3. **PROJECTS**
   - Attributes: `pcode` (Project Code), `pname` (Project Name)
   - Primary Key: `pcode`

4. **STUDENT**
   - Attributes: `roll_no` (Roll Number), `name`, `dob` (Date of Birth), `dept` (Department)
   - Primary Key: `roll_no`

5. **COURSE**
   - Attributes: `course_id`, `title`, `credits`
   - Primary Key: `course_id`

##### 🔗 Relationships

- **WORK**: Connects EMPLOYEE and DEPARTMENT (Employees work in departments)
- **ENROLLS**: Connects DEPARTMENT and PROJECTS (Departments enroll in projects)
- **enrolls**: Connects STUDENT and COURSE (Students enroll in courses)

#### 📸 ER Diagram Visualization

![ER Diagram Lab 1](ER%20DIAGRAM%20lab1.drawio.png)

*The diagram showcases entities (rectangles), attributes (ovals), and relationships (diamonds) following standard ER modeling conventions.*

#### 🌐 Interactive View

For an interactive view of the ER diagram, open the [ER DIAGRAM lab1.html](ER%20DIAGRAM%20lab1.html) file in your web browser.

## 🚀 Getting Started

### Prerequisites

- Basic understanding of database concepts
- Knowledge of SQL
- A database management system (MySQL, PostgreSQL, Oracle, etc.)
- Draw.io or compatible software for viewing/editing ER diagrams

### How to Use This Repository

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dariogeorge21/DBMS-S4.git
   cd DBMS-S4
   ```

2. **View the ER Diagrams:**
   - Open `ER DIAGRAM lab1.drawio.png` for a static image
   - Open `ER DIAGRAM lab1.html` in a web browser for an interactive view
   - Edit with [diagrams.net](https://app.diagrams.net/) if modifications are needed

3. **Implement the Database:**
   - Use the ER diagram as a reference to create database tables
   - Define appropriate data types for each attribute
   - Establish primary keys, foreign keys, and constraints
   - Write SQL CREATE TABLE statements based on the schema

## 💡 Key Concepts Covered

- **Entity-Relationship Modeling**: Understanding entities, attributes, and relationships
- **Primary Keys**: Unique identifiers for database records
- **Foreign Keys**: Establishing relationships between tables
- **Cardinality**: One-to-one, one-to-many, and many-to-many relationships
- **Database Normalization**: Organizing data to reduce redundancy
- **Data Types**: Selecting appropriate data types for attributes

## 📖 Additional Resources

- [Draw.io Documentation](https://www.diagrams.net/)
- [SQL Tutorial](https://www.w3schools.com/sql/)
- [Database Normalization Guide](https://www.guru99.com/database-normalization.html)
- [ER Diagram Best Practices](https://www.lucidchart.com/pages/er-diagrams)

## 🤝 Contributing

This is an academic repository for course work. If you have suggestions for improvements:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📝 License

This repository is for educational purposes as part of the DBMS course curriculum.

## 👤 Author

**dariogeorge21**

---

<div align="center">

**Happy Learning! 📚✨**

*Building strong foundations in Database Management Systems*

</div>
