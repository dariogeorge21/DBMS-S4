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
- **ENROLLS**: Connects DEPARTMENT and PROJECTS (Departments are assigned to/manage projects)
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
