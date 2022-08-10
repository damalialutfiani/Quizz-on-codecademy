Lesson 2 – **Queries**
1.	How would you query all the unique genres from the *books* table?
-	**SELECT DISTINCT genres**
**FROM books;**
-	FROM books
SELECT DISTINCT genres;
-	SELECT UNIQUE genres
FROM books;
-	SELECT genres
FROM books;
2.	What code would you add to this query to order colors by name alphabetically (Z to A)?
> SELECT *

> FROM colors

> ______________;
-	ORDER BY name ASC
-	GRUP BY name ASC
-	**ORDER BY name DESC**
-	ORDER BY name
3.	What is *LIMIT*?
-	**A clause that lets you specify the maximum number of rows the result set will have.**
-	A clause that restricts our query results in order to obtain only the information we want.
-	A clause that lets you specify the maximum number of column the result set will have.
-	A clause that is used to return unique values in the output.
4.	Which of the following is *NOT* a comparison operator in SQL?
-	**~**
-	!=
-	<
-	>=
5.	What does the wildcard character % in the following SQL statement do?
SELECT *
FROM sports
WHERE name LIKE ‘%ball’;
-	It matches all sports that contain ‘ball’.
-	It matches all sports that begin with ‘ball’.
-	It matches all sports that have a pattern like ‘ball’, such as ‘b3ll’ and ‘b@ll’.
-	**It matches all sports that end with ‘ball’.**
6.	What is the correct syntax to query both the name and date columns from the database?
SELECT _____
FROM album;
-	name & date
-	**name, date**
-	name; date
-	name + date
7.	Which operator would you use to query values that meet all conditions in a *where* clause?
-	BETWEEN
-	**AND**
-	LIKE
-	OR
8.	What is *ORDER BY*?
-	An operator used with the WHERE clause.
-	A clause that sorts the result set in alphabetical order only.
-	**A clause that sorts the result set alphabetically or numerically.**
-	A clause that allows you to select unique values.
9.	*IS NULL* condition returns true if the field is empty.
-	False
-	**True**
10.	What is *LIKE*?
-	**A special operator that can be used with the WHERE clause to search for a pattern.**
-	A clause used to bookmark columns that are frequently queried.
-	A statement that allows us to create different outputs.
-	A clause used to selet unique values from a table.
11.	What is the correct query o select only the cities with temperatures less than 35?
-	SELECT *
FROM cities;
-	**SELECT**
**FROM cities**
**WHERE temperature < 35;**
-	SELECT *
FROM cities
WHERE temperature = 35;
-	SELECT *
FROM cities
WHERE temperature != 35;
12.	Find the error in this code:
SELECT name,
	CASE
		WHEN imdb_rating > 8 THEN ‘Oscar’
		WHEN imdb_rating > 7 THEN ‘Good’
		WHEN imdb_rating > 6 THEN ‘Fair’
FROM movies;
-	The column was not removwed.
-	Not enough WHEN/THEN statements.
-	Missing ELSE statement.
-	**Missing END statement.**
