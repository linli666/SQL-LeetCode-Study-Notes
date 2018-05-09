# 176. Second Highest Salary
####
This question will require to return Null if there is no second highest value. Here using max() function would make sure to return Null if it doesn't find max value.
```
select max(Salary) as SecondHighestSalary from employee
where Salary < (select max(salary) from employee);
```
If it doesn't require to return Null vavlue, the following method works.
```
select Salary as SecondHighestSalary from employee
order by salary desc 
**limit 1,1**;
```
**LIMIT n, m**
After order the data, exclude first n values and then select the following m values.
