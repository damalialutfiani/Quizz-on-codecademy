Lesson 2 – **Queries**

1.	How would you query all the unique genres from the *books* table?

	a.
	
	**SELECT DISTINCT genres**

	**FROM books;**
	
	b.	
	
	FROM books

	SELECT DISTINCT genres;
	
	c. 	
	
	SELECT UNIQUE genres

	FROM books;
	
	d.	
	
	SELECT genres

	FROM books;

2.	What code would you add to this query to order colors by name alphabetically (Z to A)?
	
		SELECT *

		FROM colors

		______________;

	a.	ORDER BY name ASC

	b.	GRUP BY name ASC

	c.	**ORDER BY name DESC**

	d.	ORDER BY name

3.	What is *LIMIT*?

	a.	**A clause that lets you specify the maximum number of rows the result set will have.**

	b.	A clause that restricts our query results in order to obtain only the information we want.

	c.	A clause that lets you specify the maximum number of column the result set will have.

	d.	A clause that is used to return unique values in the output.

4.	Which of the following is *NOT* a comparison operator in SQL?

	a.	__~__

	b.	!=

	c.	<

	d.	>=

5.	What does the wildcard character % in the following SQL statement do?

		SELECT *

		FROM sports

		WHERE name LIKE ‘%ball’;

	a.	It matches all sports that contain ‘ball’.

	b.	It matches all sports that begin with ‘ball’.

	c.	It matches all sports that have a pattern like ‘ball’, such as ‘b3ll’ and ‘b@ll’.

	d.	**It matches all sports that end with ‘ball’.**

6.	What is the correct syntax to query both the name and date columns from the database?

>	SELECT _____

>	FROM album;

a.	name & date

b.	**name, date**

c.	name; date

d.	name + date

7.	Which operator would you use to query values that meet all conditions in a *WHERE* clause?

a.	BETWEEN

b.	**AND**

c.	LIKE

d.	OR

8.	What is *ORDER BY*?

a.	An operator used with the WHERE clause.

b.	A clause that sorts the result set in alphabetical order only.

c.	**A clause that sorts the result set alphabetically or numerically.**

d.	A clause that allows you to select unique values.

9.	*IS NULL* condition returns true if the field is empty.

a.	False

b.	**True**

10.	What is *LIKE*?

a.	**A special operator that can be used with the WHERE clause to search for a pattern.**

b.	A clause used to bookmark columns that are frequently queried.

c.	A statement that allows us to create different outputs.

d.	A clause used to selet unique values from a table.

11.	What is the correct query to select only the cities with temperatures less than 35?

a.
>	SELECT *

>	FROM cities;

b.
>	__SELECT *__

>	**FROM cities**

>	**WHERE temperature < 35;**

c.
>	SELECT *

>	FROM cities

>	WHERE temperature = 35;

d.
>	SELECT *

>	FROM cities

>	WHERE temperature != 35;

12.	Find the error in this code:

>	SELECT name,

>		CASE

>			WHEN imdb_rating > 8 THEN ‘Oscar’

>			WHEN imdb_rating > 7 THEN ‘Good’

>			WHEN imdb_rating > 6 THEN ‘Fair’

>	FROM movies;

a.	The column was not removed.

b.	Not enough WHEN/THEN statements.

c.	Missing ELSE statement.

d.	**Missing END statement.**
