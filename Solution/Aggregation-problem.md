/*
Query a count of the number of cities in CITY with populations larger than 100,000.

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

Query the total population of all cities in CITY where District is California.

```sql
SELECT SUM(POPULATION)
FROM CITY
WHERE DISTRICT = "California";

```
Query the total population of all cities in CITY where District is California.

```sql
SELECT SUM(POPULATION)
FROM CITY
WHERE DISTRICT='California';
```

Query the difference between the maximum and minimum populations in CITY.

```sql
SELECT MAX(POPULATION)-MIN(POPULATION)
FROM CITY;
```








