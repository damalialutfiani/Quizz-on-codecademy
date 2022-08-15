Lesson 4 - **Multiple Tables**

1.	What is the best definition of a primary key?

     a.  A primary record in a database that serves as a template for all other records.

     b.  A NULL value.

     c.  **A unique identifier for each row or record in a given table.**

     d.  A foreign key with distinct attributes.

2.	*UNION* allows us to stack one dataset on top of another.

    a.  **True**
    
    b.  False
    
3.	What is the best definition of a foreign key?

    a.  A primary key that is not present when a table is created but is later added.
    
    b.	A unique identifier for each row or record in a given table.
    
    c.  A NULL value.
    
    d.  **A column that contains the primary key of another table in the database.**
    
4.	Which keyword would you use to alias recipes.name and chefs.name in the following query?

    	SELECT recipes.name __ ‘Recipe’ ,

      	     Chefs.name __ ‘Chef’

    	FROM recipes

    	JOIN chefs

    	ON recipes.chef_id = chefs.id;

    a.	**AS**
    
    b.  ALIAS
    
    c.  WITH
    
    d.  ON
    
5.	You have two tables authors and books. Each book belongs to an author and references that author through a foreign key. If the primary key of the authors table is id, what would be the most sensical name for a foreign key in the books table that references the id column in authors?

     a. **author_id**
     
     b. id
     
     c. foreign_key
     
6.	You have two tables teachers and students. Each student belongs to a teacher. Complete the query to join the tables on the teacher id.

          SELECT *
     
          FROM studenrs
     
          Join teachers
     
               ON ____ ;

     a. **students.teacher_id = teachers.id**
     
     b. teachers.id = student_id
     
     c. teacher_id = id
     
     d. teachers = students.id
     
7.	What is the difference between an INNER JOIN and a LEFT JOIN?

     a. An INNER JOIN joins rows within a table. A LEFT JOIN joins rows between tables.

     b. **LEFT JOIN combines rows from two or more tables, but unlike INNER JOIN, it does not require the join condition to be met.**

     c. An INNER JOIN is an obsolete form of a LEFT JOIN.

     d. A LEFT JOIN is an obsolete form of an INNER JOIN.

9.	In a LEFT JOIN, if a join condition is not met, what will it use to fill columns on the right table?
-	column_name.id
-	**NULL values**
-	id
-	primary keys
10.	Why is a CROSS JOIN not so usefull?
-	It nullifies all primary keys.
-	It is no longer supported by SQL.
-	**It combines every row in one table with every row in another table.**
-	It combines all foreign keys into one table called foreign keys.
11.	Which kind of join is in the animation below?

- First Table

| C1 | C2 |
|:--:|:--:|
| A  | B  |
| Q  | W  |
| X  | Y  |

- Second Tablee

| C2 | C3 |
|:--:|:--:|
| B  | C  |
| E  | R  |
| Y  | z  |

- Became : 

| C1 | C2 | C3 |
|:--:|:--:|:--:|
| A  | B  | C  |
| X  | Y  | Z  |

-	Um, none of these?
-	**Oh, that’s a INNER JOIN.**
-	No, it is a CROSS JOIN.
-	This is definitely a LEFT JOIN.
