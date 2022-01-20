CAMEL-sql EXAMPLE

===========================

To run this example:

1. mvn install

2. mvn compile exec:java -Dexec.mainClass=com.javainuse.main.CamelMain


Output:-

INFO: Executed SQL script from class path resource [db-schema.sql] in 16 ms.
data:[{empid=empId1, empname=emp1}, {empid=empId2, empname=emp2}]
employees:[Employee [empId=empId1, empName=emp1], Employee [empId=empId2, empName=emp2]]

-----------------------------------------------------

Database:-

gte=# select * from employees;
 empid  | empname 
--------+---------
 empId1 | emp1
 empId2 | emp2

