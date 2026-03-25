Find the longest time that an employee has been at the studio
SELECT MAX(Years_employed) FROM Employees;

For each role, find the average number of years employed by employees in that role
SELECT Role, AVG(Years_employed) AS Average_Years FROM Employees GROUP BY Role;

Find the total number of employee years worked in each building
SELECT Building, SUM(Years_employed) FROM Employees GROUP BY Building;
