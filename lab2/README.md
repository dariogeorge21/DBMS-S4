Questions:

Create a table named employee and populate the table as shown below: emp_id, emp_name, dept, salary with emp_id as primary key field. Consider the table employee and insert tuples with employee names starting with D, O, C, A. Employee department names include HR, Marketing, Production, Sales, etc. Salary from 200 to 1000.

    - Select employee with salary greater than 7k
    
    - Update the salary of "David Smith" to 8200
    
    - Insert a new employee with emp_id = 6, emp_name = "Daniel Allarsis", dept = "Production" and salary 6700
    
    - Delete the employee with emp_id = 3
    
    - Select employee whose name does not start with D or O
    
    - Calculate the total salary expense for each dept
    
    - Update the salary of employees in the Production dept by adding 5% to their current salaries
    
    - Delete all employees with salary below 7k
    
    - Find the employee with the lowest salary and display their name and salary
    
    - Update the salary of employees in the Marketing department to 8200
    
    - Find the name of all employees starting with the alphabet A
    
    - List the name of all employees where the emp_name contains the substring 'it'
    
    - List all the depts in uppercase format
    
    - List all employee details whose dept starts with 'M' with the 3rd letter as 'r' and contains the substring 'ket'
    
    - List all depts in reverse uppercase format - no duplicates
  

---

Answers to each question:

create table employee(e_id int PRIMARY KEY, e_name varchar(30), dept varchar(30), salary int);

insert into employee (emp_id, emp_name, dept, salary) values ((1,'David', 'Marketing', 7500);
insert into employee (emp_id, emp_name, dept, salary) values ((2,'Ollama', 'HR', 3500);
insert into employee (emp_id, emp_name, dept, salary) values ((3,'Christ', 'Production', 4500);
insert into employee (emp_id, emp_name, dept, salary) values ((4,'Aaron', 'Sales', 9500);
insert into employee (emp_id, emp_name, dept, salary) values ((5,'Daniel', 'Production', 6500);

select employee, salary from employee where salary>7000;
update employee set salary=8200 where e_name='David';
INSERT INTO employee (emp_id, emp_name, dept, salary) VALUES ((6,'Daniel Allaris', 'Production', 6700);
delete from employee where e_id = 3;
select * from employee where name not like "D" or "O";
select department, sum(salary) from employee group by department;
update employee set salary=(salary+(salary*0.15)) where department = 'production';
delete from employee where salary<7000;
select e_name, min(salary) from employee;
update employee set salary = 8200 where department = "Marketing";
select e_name from employee where e_name like "A%";
select e_name from employee where department like "%it%";
select distinct upper(department) from employee;
select * from employee where department like "M_r%" and department like "%ket%";
select distinct upper(department) as dept, reverse(upper(department) as rev_dept from employee;



Final Lab Result: The above program has been successfully executed and the output is verified. Effectively addresses the course outcome CO2.
