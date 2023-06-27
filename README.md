# SQL-Higher-Than-75-Marks

# Challenge:
- Query the Name of any student in STUDENTS who scored higher than  Marks. Order your output by the last three characters of each name. If two or more students both have names ending in the same last three characters (i.e.: Bobby, Robby, etc.), secondary sort them by ascending ID.

- The STUDENTS table is described as follows: 

![mqrw5ikf 5lk](https://github.com/MarcvWaes/SQL-Higher-Than-75-Marks/assets/120553175/94b2b949-aadd-4539-9f17-abef32369a1d)

-  The Name column only contains uppercase (A-Z) and lowercase (a-z) letters.

![pffxu0cr fut](https://github.com/MarcvWaes/SQL-Higher-Than-75-Marks/assets/120553175/a5bb510f-0f84-4185-9336-ab62a9dd8eb2)

# Solution:
- SELECT Name
- FROM STUDENTS
- WHERE Marks > 75
- ORDER BY RIGHT(Name, 3), ID ASC;

- This query selects the Name column from the STUDENTS table where the Marks column is greater than 75. It then orders the result by the last three characters of each name using the RIGHT function and performs a secondary sort by ascending ID.

# Output:
- Stuart 
- Kristeen 
- Christene 
- Amina 
- Aamina
- .....
