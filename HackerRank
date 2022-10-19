--Problem Statement

/*
Given a table TRIANGLES that holds data for three fields namely A, B, C.
+-------------+------------+
| Column      |   Type     |
+-------------+------------+
| A           | INTEGER    |
| B           | INTEGER    |
| C           | INTEGER    |
+-------------+------------+
 
Write a query identifying the type of each record in the TRIANGLES table using its three side lengths. Output one of the following statements for each record in the table:
Equilateral   : It's a triangle with  sides of equal length.
Isosceles     : It's a triangle with  sides of equal length.
Scalene       : It's a triangle with  sides of differing lengths.
Not A Triangle: The given values of A, B, and C don't form a triangle.
*/

--Solution

SELECT IF( (A+B<=C) OR (B+C<=A) OR (C+A<=B),"Not A Triangle",
            IF( (A=B) AND (B=C),"Equilateral",
                IF((A=B) OR (B=C) OR (C=A),"Isosceles","Scalene"))) FROM TRIANGLES;
