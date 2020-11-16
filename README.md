# sql-day2
the second day work of sql has been attached


#01 higher than 75 marks
SELECT NAME FROM STUDENTS WHERE MARKS > 75 ORDER BY SUBSTR(NAME, LENGTH(NAME)-2, 3), ID;    

#02 employee Names
select name from EMPLOYEE order by name asc;

#03 employee salaries
select name from Employee where salary>2000 and months<10 order by employee_id asc;

#04 weather observation station 10
select distinct city from station 
where city not like '%a' and
city not like '%e' and
 city not like '%i'
and
 city not like '%o'
and
 city not like '%u'
order by city;

#05 weather observation station 11
select distinct CITY from STATION where (CITY not like 'A%' and CITY not like 'E%' and CITY not like 'I%' and CITY not like 'O%' and CITY not like 'U%' ) or (CITY not like '%a' and CITY not like '%e' and CITY not like '%i' and CITY not like '%o' and CITY not like '%u' ) order by CITY;

#06 weather observation station 12
SELECT DISTINCT CITY FROM STATION WHERE LOWER(SUBSTR(CITY,1,1)) NOT IN ('a','e','i','o','u') AND LOWER(SUBSTR(CITY,LENGTH(CITY),1)) NOT IN ('a','e','i','o','u');
