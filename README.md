# SQL-Assignment-10
Q-1. Write an SQL query to determine the 5th highest salary without using TOP or limit
method.

Ans 
Q-2. Write an SQL query to fetch the list of employees with the same salary.

Ans  select  distinct wl.name_employee,wl.salary
    from [dbo].[worker_sal] wl ,[dbo].[worker_sal] ws
    where wl.salary = ws.salary and wl.id_no != ws.id_no
    order by wl.salary
