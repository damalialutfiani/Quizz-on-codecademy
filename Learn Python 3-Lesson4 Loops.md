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
			
	a.	
		
		1
	
		1
		
		3
	
	b.	
	
		1
	
		1
		
		2
		
		3
		
	c.	
		
		2
	
	d.	
	
	  **1**
	
	  **1**
		
4.	What would be the output of the following code:

		drink_choices = [“coffee”, “tea”, “water”, “juice”, “soda”]
	
		for drink in drink_choices:
	
			print(drink)
			
	a.	drink
	
	b.	[“coffee”, “tea”, “water”, “juice”, “soda”]
	
	c.	
	
	**coffee**
	
	**tea**
	
	**water**
	
	**juice**
	
	**soda**
	
	d.	coffee
	
5.	What would be the output of the following code:

		numbers = [1, 1, 2, 3]

		for number in numbers:
			
			if number % 2 == 0:
		
				continue
	
			print(number)
			
	a.	
	
		2
	
	b.	
	
		1
	
		1
		
	c.	
	
	**1**
	
	**1**
		
	**3**
		
	d.	
	
		1
	
		1
		
		2
		
6.	Fill in the blank with the appropriate while condition in order to print the numbers 1 through 10 in order:

		i = 1
		
		__blank__
		
			print(i)
		
			i += 1
		
	a.	while i == range (11):
	
	b.	while I < 10:
	
	c.	**while i <= 10:**
	
	d.	while I > 10:
	
7.	Which of these list comprehensions will create a list equal to desired_list?

		my_list = [5, 10, -2, 8, 20]

		desired_list = [10, 8, 20]
		
	a.	[i + 5 for i in my_list]
	
	b.	**[i for i in my_list if i > 5]**
	
	c.	[i for i in my_list]
	
	d.	[i for i in my_list if I > 10]
	
8.	What would be the output of the following code:

		for i in range(3):
	
			print(5)
			
	a.	
	
		0
		
		1
		
		2
		
	b.
	
		0
		
		1
		
		2
		
		3
		
		4
		
	c.	
	
	**5**
	
	**5**
	
	**5**
	
	d.
	
		3
		
		3
		
		3
		
		3
		
		3
		
9.	Fill in the code to loop over the list grouped_topics and print every element in the list.

		grouped_topics = [[“Algorithms”, “Data Structures”, “AI”], [“Linear Regression”, “SQL”]]

	
		for sublist in _____ :
		
			for sublist_element in ______ :
		
				print( _____ )

	a.	**sublist**
	
	b.	for
	
	c.	**grouped_topics**
	
	d.	**sublist_element**
	
	Click or drag and drop to fill in the blank.
	
	So, the answer is
	
		for sublist in **grouped_topics**:
		
   			for sublist_element in **sublist**:
			
        			print (**sublist_element**)
				
10.	Which of these list comprehensions will create a list equal to desired_list?

		desired_list = [-1, 0, 1, 2, 3]
		
	a.	
		
		desired_list = []
		
		for i in range(5)
		
			desired_list = i -1
			
	b.	range(5)
	
	c.	**[i – 1 for i in range(5)]**
	
	d.	[i for i in range(5)]
