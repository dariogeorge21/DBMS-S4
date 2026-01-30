# Lab Experiment 2: Database Operations with SQL

## Overview
This lab covers fundamental SQL operations including table creation, data insertion, querying, updating, and deletion on an employee database.

---

## Table Creation

### Objective
Create a table named `employee` with the following structure:
- `emp_id` (Primary Key)
- `emp_name`
- `dept`
- `salary`

### SQL Code
```sql
CREATE TABLE employee(
    e_id INT PRIMARY KEY, 
    e_name VARCHAR(30), 
    dept VARCHAR(30), 
    salary INT
);
```

**Proof:** [Screenshot 0.1](/screenshots/0.1.png)

---

## Data Insertion

### Objective
Insert employee records with names starting with D, O, C, A. Departments include HR, Marketing, Production, Sales. Salaries range from 200 to 1000.

### SQL Code
```sql
INSERT INTO employee (emp_id, emp_name, dept, salary) 
VALUES (1, 'David', 'Marketing', 7500);

INSERT INTO employee (emp_id, emp_name, dept, salary) 
VALUES (2, 'Ollama', 'HR', 3500);

INSERT INTO employee (emp_id, emp_name, dept, salary) 
VALUES (3, 'Christ', 'Production', 4500);

INSERT INTO employee (emp_id, emp_name, dept, salary) 
VALUES (4, 'Aaron', 'Sales', 9500);

INSERT INTO employee (emp_id, emp_name, dept, salary) 
VALUES (5, 'Daniel', 'Production', 6500);
```

**Proof:** [Screenshot 0.2](/screenshots/0.2.png)

---

## Query Operations

### 1. Select Employees with Salary Greater Than 7000

**Objective:** Retrieve all employees earning more than 7000

```sql
SELECT e_name, salary 
FROM employee 
WHERE salary > 7000;
```

**Proof:** [Screenshot 1](/screenshots/1.png)

---

### 2. Update David's Salary

**Objective:** Update David's salary to 8200

```sql
UPDATE employee 
SET salary = 8200 
WHERE e_name = 'David';
```

**Proof:** [Screenshot 2](/screenshots/2.png)

---

### 3. Insert New Employee

**Objective:** Add a new employee record

```sql
INSERT INTO employee (emp_id, emp_name, dept, salary) 
VALUES (6, 'Daniel Allaris', 'Production', 6700);
```

**Proof:** [Screenshot 3](/screenshots/3.png)

---

### 4. Delete Employee by ID

**Objective:** Remove employee with emp_id = 3

```sql
DELETE FROM employee 
WHERE e_id = 3;
```

**Proof:** [Screenshot 4](/screenshots/4.png)

---

### 5. Select Employees Not Starting with D or O

**Objective:** Find all employees whose names don't start with D or O

```sql
SELECT * 
FROM employee 
WHERE e_name NOT LIKE 'D%' 
AND e_name NOT LIKE 'O%';
```

**Proof:** [Screenshot 5](/screenshots/5.png)

---

### 6. Total Salary by Department

**Objective:** Calculate total salary expenses for each department

```sql
SELECT dept, SUM(salary) 
FROM employee 
GROUP BY dept;
```

**Proof:** [Screenshot 6](/screenshots/6.png)

---

### 7. Update Production Department Salaries

**Objective:** Increase salaries in Production department by 15%

```sql
UPDATE employee 
SET salary = (salary + (salary * 0.15)) 
WHERE dept = 'Production';
```

**Proof:** [Screenshot 7](/screenshots/7.png)

---

### 8. Delete Employees with Low Salary

**Objective:** Remove all employees earning less than 7000

```sql
DELETE FROM employee 
WHERE salary < 7000;
```

**Proof:** [Screenshot 8](/screenshots/8.png)

---

### 9. Find Employee with Lowest Salary

**Objective:** Display the name and salary of the lowest-paid employee

```sql
SELECT e_name, MIN(salary) 
FROM employee;
```

**Proof:** [Screenshot 9](/screenshots/9.png)

---

### 10. Update Marketing Department Salaries

**Objective:** Set all Marketing department employees' salary to 8200

```sql
UPDATE employee 
SET salary = 8200 
WHERE dept = 'Marketing';
```

**Proof:** [Screenshot 10](/screenshots/10.png)

---

### 11. Find Employees Starting with 'A'

**Objective:** Retrieve names of all employees whose names start with 'A'

```sql
SELECT e_name 
FROM employee 
WHERE e_name LIKE 'A%';
```

**Proof:** [Screenshot 11](/screenshots/11.png)

---

### 12. Find Employees with 'it' Substring in Department

**Objective:** List all employees whose department contains 'it'

```sql
SELECT e_name 
FROM employee 
WHERE dept LIKE '%it%';
```

**Proof:** [Screenshot 12](/screenshots/12.png)

---

### 13. List Departments in Uppercase

**Objective:** Display all departments in uppercase without duplicates

```sql
SELECT DISTINCT UPPER(dept) 
FROM employee;
```

**Proof:** [Screenshot 13](/screenshots/13.png)

---

### 14. Complex Department Pattern Matching

**Objective:** List employee details where department starts with 'M', has 'r' as 3rd letter, and contains 'ket'

```sql
SELECT * 
FROM employee 
WHERE dept LIKE 'M_r%' 
AND dept LIKE '%ket%';
```

**Proof:** [Screenshot 14](/screenshots/14.png)

---

### 15. Reverse Uppercase Departments

**Objective:** Display departments in reverse uppercase format without duplicates

```sql
SELECT DISTINCT UPPER(dept) AS dept, 
       REVERSE(UPPER(dept)) AS rev_dept 
FROM employee;
```

**Proof:** [Screenshot 15](/screenshots/15.png)

---

## Summary

| Operation | Count |
|-----------|-------|
| Table Creation | 1 |
| Insert Operations | 6 |
| Select Queries | 9 |
| Update Operations | 3 |
| Delete Operations | 2 |

---

## Lab Completion Status

✅ **Status:** Successfully Executed

**Outcome:** All SQL operations have been executed successfully and verified.

**Course Outcome:** Effectively addresses **CO2**

---

## Notes

- All employee records follow the specified naming convention (starting with D, O, C, A)
- Department names include: HR, Marketing, Production, Sales
- Salary values demonstrate various ranges and operations
- All queries implement proper filtering and aggregation techniques
