# 176. Second Highest Salary
####
```
select Salary as SecondHighestSalary from employee
order by salary desc 
limit 1,1
```
**LIMIT n, m**
After order the data, exclude first n values and then select the following m values.
