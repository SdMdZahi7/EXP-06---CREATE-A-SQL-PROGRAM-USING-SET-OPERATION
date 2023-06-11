# EXP-06---CREATE-A-SQL-PROGRAM-USING-SET-OPERATION
[ UNION , UNION ALL ,INTERSECT , EXCEPT ]

## AIM:
To create a sql program using set operation

## ALGORITHM:
Create tables A and B with attributes ID and name
Insert values into the tables
Display the tables
Perform set operations
Union - Combines the distinct rows from both tables A and B
Union All - Combines all rows from both tables A and B, including duplicates
Intersect - Retrieves the common rows between tables A and B
Except - Retrieves the rows from table A that are not present in table B
## PROGRAM:
~~~
java
CREATE TABLE A (
    ID INT,
    name VARCHAR(50)
);

CREATE TABLE B (
    ID INT,
    name VARCHAR(50)
);
INSERT INTO A (ID, name) VALUES (1, 'John');
INSERT INTO A (ID, name) VALUES (2, 'Jane');
INSERT INTO A (ID, name) VALUES (3, 'Alice');

INSERT INTO B (ID, name) VALUES (2, 'Jane');
INSERT INTO B (ID, name) VALUES (3, 'Alice');
INSERT INTO B (ID, name) VALUES (4, 'Mike');
SELECT * FROM A;
SELECT * FROM B;
SELECT * FROM A
UNION
SELECT * FROM B;
SELECT * FROM A
UNION ALL
SELECT * FROM B;
SELECT * FROM A
INTERSECT
SELECT * FROM B;
SELECT * FROM A
EXCEPT
SELECT * FROM B;
~~~
## OUTPUT:
### TABLE A:
![image](https://github.com/SdMdZahi7/EXP-06---CREATE-A-SQL-PROGRAM-USING-SET-OPERATION/assets/94187572/e47a1545-082c-4e6c-b6c0-4597fadeed88)
### TABLE B:
![image](https://github.com/SdMdZahi7/EXP-06---CREATE-A-SQL-PROGRAM-USING-SET-OPERATION/assets/94187572/9c3fc663-c4a1-46d3-a0ea-1764ef2ebf57)
### UNION
![image](https://github.com/SdMdZahi7/EXP-06---CREATE-A-SQL-PROGRAM-USING-SET-OPERATION/assets/94187572/6b40c2f4-f3ad-42dd-9a6b-f5a163fcbbd1)
### UNION ALL:
![image](https://github.com/SdMdZahi7/EXP-06---CREATE-A-SQL-PROGRAM-USING-SET-OPERATION/assets/94187572/c152ce4c-990f-4bfa-a6c2-7301b170eda9)
### INTERSECT:
![image](https://github.com/SdMdZahi7/EXP-06---CREATE-A-SQL-PROGRAM-USING-SET-OPERATION/assets/94187572/c34ad5c7-4fd9-47ee-80a1-73025e82dfd7)
### EXCEPT
![image](https://github.com/SdMdZahi7/EXP-06---CREATE-A-SQL-PROGRAM-USING-SET-OPERATION/assets/94187572/0f51e61e-b9a4-4a4d-86ad-3de869384649)
### RESULT:
Thus we have successfully obtained the required result using the above-given code.

