Lesson 4 – **Loops**

1.	What would be the output of the following code:

        numbers = [2, 4, 6, 8]

        for number in numbers:
  
          print(“hello!”)

	a.	hello!
	
	b.	
	
	**hello!**
		
	**hello!**
	
	**hello!**
		
	**hello!**
	
	c.	2 4 6 8
	
	d.	2 hello! 4 hello! 6 hello! 8 hello!
	
2.	What would be the output of the following code:

	for i in range(3):
		print(i)
		
	a.	
		
	**0**
	
	**1**
	
	**2**
	
	b.	
	
		1
	
		2
		
		3
	
	c.	
	
		i
	
		i
	
		i
	
	d.
	
		i
	
		i
	
		i
	
		i
	
3.	What would be the output of the following code:

		numbers = [1, 1, 2, 3]
	
		for number in numbers:
	
			if number % 2 == 0:
		
				break
			
			print(number)
			
-	1
1
3
-	1
1
2
3
-	2
-	**1
1**
4.	What would be the output of the following code:
drink_choices = [“coffee”, “tea”, “water”, “juice”, “soda”]
for drink in drink_choices:
	print(drink)
-	drink
-	[“coffee”, “tea”, “water”, “juice”, “soda”]
-	**coffee
tea
water
juice
soda**
-	coffee
5.	What would be the output of the following code:
numbers = [1, 1, 2, 3]
for number in numbers:
	if number % 2 == 0:
		continue
	print(number)
-	2
-	1
1
-	**1
1
3**
-	1
1
2
6.	Fill in the blank with the appropriate while condition in order to print the numbers 1 through 10 in order:
i = 1
__blank__
	print(i)
	i += 1
-	while i == range (11):
-	while I < 10:
-	**while i <= 10:**
-	while I > 10:
7.	Which of these list comprehensions will create a list equal to desired_list?
my_list = [5, 10, -2, 8, 20]
desired_list = [10, 8, 20]
-	[i + 5 for i in my_list]
-	**[i for i in my_list if i > 5]**
-	[i for i in my_list]
-	[i for i in my_list if I > 10]
8.	What would be the output of the following code:
for i in range(3):
	print(5)
-	0
1
2
-	0
1
2
3
4
-	**5
5
5**
-	3
3
3
3
3
9.	Fill in the code to loop over the list grouped_topics and print every element in the list.
grouped_topics = [[“Algorithms”, “Data Structures”, “AI”], [“Linear Regression”, “SQL”]]

for sublist in _____ :
	for sublist_element in ______ :
		print( _____ )

-	**sublist**
-	for
-	**grouped_topics**
-	**sublist_element**
Click or drag and drop to fill in the blank
So, the answer is
for sublist in **grouped_topics**:
	for sublist_element in **sublist**:
		print (**sublist_element**)
10.	Which of these list comprehensions will create a list equal to desired_list?
desired_list = [-1, 0, 1, 2, 3]
-	desired_list = []
for i in range(5)
	desired_list = i -1
-	range(5)
-	**[i – 1 for i in range(5)]**
-	[i for i in range(5)]
