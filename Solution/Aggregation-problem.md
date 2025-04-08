/*
1.Query a count of the number of cities in CITY with populations larger than 100,000.

## Input Format

The CITY table is described as follows:

+-------------+--------------+
| Field       | Type         |
+-------------+--------------+
| ID          | NUMBER       |
| NAME        | VARCHAR2(17) |
| COUNTRYCODE | VARCHAR2(3)  |
| DISTRICT    | VARCHAR2(20) |
| POPULATION  | NUMBER       |
+-------------+--------------+
*/
```sql
SELECT COUNT(*)
FROM CITY
WHERE POPULATION>100000;
```
/*

2.Query the total population of all cities in CITY where District is California.

```sql
SELECT SUM(POPULATION)
FROM CITY
WHERE DISTRICT = "California";

```
3.Query the total population of all cities in CITY where District is California.

```sql
SELECT SUM(POPULATION)
FROM CITY
WHERE DISTRICT='California';
```

4.Query the difference between the maximum and minimum populations in CITY.

```sql
SELECT MAX(POPULATION)-MIN(POPULATION)
FROM CITY;
```
5.Samantha was tasked with calculating the average monthly salaries for all employees in the EMPLOYEES table, but did not realize her keyboard's  key was broken until after completing the calculation. She wants your help finding the difference between her miscalculation (using salaries with any zeros removed), and the actual average salary.

Write a query calculating the amount of error (i.e.:  average monthly salaries), and round it up to the next integer.

```sql
SELECT CEIL(AVG(SALARY)-AVG(REPLACE(SALARY,'0','')))
FROM EMPLOYEES;
```







