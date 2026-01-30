## Lab Experiment 2

Questions:

Create a table named employee and populate the table as shown below: emp_id, emp_name, dept, salary with emp_id as primary key field. 

Code:
```
create table employee(e_id int PRIMARY KEY, e_name varchar(30), dept varchar(30), salary int);
```
Proof: [img href=/screenshots/0.1.png]


Consider the table employee and insert tuples with employee names starting with D, O, C, A. Employee department names include HR, Marketing, Production, Sales, etc. Salary from 200 to 1000.

Code:
```
insert into employee (emp_id, emp_name, dept, salary) values ((1,'David', 'Marketing', 7500);
insert into employee (emp_id, emp_name, dept, salary) values ((2,'Ollama', 'HR', 3500);
insert into employee (emp_id, emp_name, dept, salary) values ((3,'Christ', 'Production', 4500);
insert into employee (emp_id, emp_name, dept, salary) values ((4,'Aaron', 'Sales', 9500);
insert into employee (emp_id, emp_name, dept, salary) values ((5,'Daniel', 'Production', 6500);
```

Proof: [img href=/screenshots/0.2.png]

    - Select employee with salary greater than 7k
    Code:
    ```
    select employee, salary from employee where salary>7000;
    ```
    Proof: [img href=/screenshots/1.png]

    
    - Update the salary of "David Smith" to 8200
    ```
    update employee set salary=8200 where e_name='David';
    ```
        Proof: [img href=/screenshots/2.png]

    
    - Insert a new employee with emp_id = 6, emp_name = "Daniel Allarsis", dept = "Production" and salary 6700
    ```
    INSERT INTO employee (emp_id, emp_name, dept, salary) VALUES ((6,'Daniel Allaris', 'Production', 6700);
    ```
        Proof: [img href=/screenshots/3.png]

    
    - Delete the employee with emp_id = 3
    ```
    delete from employee where e_id = 3;
    ```
        Proof: [img href=/screenshots/4.png]

    
    - Select employee whose name does not start with D or O
    ```
    select * from employee where name not like "D" or "O";
    ```
        Proof: [img href=/screenshots/5.png]

    
    - Calculate the total salary expense for each dept
    ```
    select department, sum(salary) from employee group by department;
    ```
        Proof: [img href=/screenshots/6.png]

    
    - Update the salary of employees in the Production dept by adding 5% to their current salaries
    ```
    update employee set salary=(salary+(salary*0.15)) where department = 'production';
    ```
        Proof: [img href=/screenshots/7.png]

    
    - Delete all employees with salary below 7k
    ```
    delete from employee where salary<7000;
    ```
        Proof: [img href=/screenshots/8.png]

    
    - Find the employee with the lowest salary and display their name and salary
    ```
    select e_name, min(salary) from employee;
    ```
        Proof: [img href=/screenshots/9.png]

    
    - Update the salary of employees in the Marketing department to 8200
    ```
    update employee set salary = 8200 where department = "Marketing";
    ```
        Proof: [img href=/screenshots/10.png]

    
    - Find the name of all employees starting with the alphabet A
    ```
    select e_name from employee where e_name like "A%";
    ```
        Proof: [img href=/screenshots/11.png]

    - List the name of all employees where the emp_name contains the substring 'it'
    ```
    select e_name from employee where department like "%it%";
    ```
        Proof: [img href=/screenshots/12.png]

    
    - List all the depts in uppercase format
    ```
    select distinct upper(department) from employee;
    ```
        Proof: [img href=/screenshots/13.png]

    
    
    - List all employee details whose dept starts with 'M' with the 3rd letter as 'r' and contains the substring 'ket'
    ```
    select * from employee where department like "M_r%" and department like "%ket%";
    ```
        Proof: [img href=/screenshots/14.png]

    
    - List all depts in reverse uppercase format - no duplicates
    ```
    select distinct upper(department) as dept, reverse(upper(department) as rev_dept from employee;
    ```
        Proof: [img href=/screenshots/15.png]

  

---




Final Lab Result: The above program has been successfully executed and the output is verified. Effectively addresses the course outcome CO2.
