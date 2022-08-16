Lesson 3 - **Aggregate Functions**

1.	Aggregate function

	a.	Return the total sum of the values in a numeric colum.

	b.	**Compute a single result set from a set values.**

	c.	Round the values of a colomn.

	d.	Count the number of rows where the value(s) is not NULL.

2.	How would you calculate the minimum number of stops from train table?

	a.
	>	**SELECT MIN(stops)**

	>	**FROM train;**

	b.	
	>	SELECT SUM(stops)

	>	FROM train;

	c.	
	>	SELECT AVG(stops)

	>	FROM train;

	d.	
	>	SELECT MAX(stops)

	>	FROM train;

3.	What does the *COUNT()* function take as argument(s)?

	a.	__The name of a column or *.__

	b.	The name of a row.

	c.	The name of a table.

	d.	The name of a database.

4.	What does the *ROUND* function take as argument(s)?

	a.	The table name.

	b.	The column name, and a + or – sign to indicate rounding up or rounding down.

	c.	It does not take an argument.

	d.	**The column name, and the number of decimal places to round the values in the column to.**

5.	Which function takes a column and returns the total sum of the numeric values in that column?

	a.	**SUM()**

	b.	MAX()

	c.	AVG()

	d.	COUNT()

6.	What does the following query do?

		SELECT genre,
	
			SUM(downloads)

		FROM kindle

		GROUP BY genre;


	a.	It returns the total amount of downloads.

	b.	It returns the average number of downloads – for each genre.

	c.	It returns the highest number of downloads – for each genre.

	d.	**It returns the total amount of downloads – for each genre.**

7.	The *WHERE* clause filters rows, whereas the having clause filter groups.

a.	False

b.	**True**

8.	What does the following query do?

>	SELECT price,

>		COUNT(*)

>	FROM menu

>	WHERE orders > 50

>	GROUP BY price;

a.	It calculates the total number of menu items that have been ordered more than 50 times – sorted by price.

b.	**It calculates the total number of menu items that have been ordered more than 50 times – for each price.**

c.	It calculates the total number of menu items.

d.	It calculates the total number of menu items that have been ordered more than 50 times.

9.	Find the error in this code:

>	SELECT COUNT(*)

>	FROM songs

>	HAVING plays > 100;

a.	There is no error.

b.	There is no such thing as COUNT(*).

c.	It should be GROUP BY instead of HAVING.

d.	**It should be WHERE instead of HAVING.**

10.	What does the following query do?

>	SELECT neighborhood,

>		AVG(price)

>	FROM apartments

>	GROUP BY neighborhood;

a.	**It calculates the average price of apartments in each neighborhood.**

b.	It calculates the lowest price of apartments in each neighborhood.

c.	It calculates the highest price of apartments in each neighborhood.

d.	It calculates the total number of apartments in each neighborhood.

