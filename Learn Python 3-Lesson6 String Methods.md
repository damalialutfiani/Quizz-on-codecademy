Lesson 6 – **String Methods**

1.	Given the poem (When You Are Old, by W. B. Yeats) saved as multiline string as shown in the code block, what code could we use to create a list that contains a string of each line in the poem?

		when_you_are_old = \
		“””When you are old and grey and full of sleep,
		And nodding by the fire, take down this book,
		And slowly read, and dream of the soft look
		Your eyes had once, and of their shadows deep;

		How many loved your moments of glad grace,
		And loved your beauty with love false or true,
		But one man loved the pilgrim soul in you,
		And loved the sorrows of your changing face;

		And bending down beside the glowing bars,
		Murmur, a little sadly, how Love fled
		And paced upon the mountains overhead
		And hid his face amid a crowd of stars.”””
	
	a.	list_of_lines = when_you_are_old.strip()
	
	b.	
		
		list_of_lines = []
		for line in when_you_are_old:
			list_of_lines.append(line)
	
	c.	list_of_lines = “\n”.join(when_you_are_old)
	
	d.	**list_of_lines = when_you_are_old.split("\n")**

2.	Consider the string user_name = "::::::::Eloise :::::::::::". What line of code would clean this string and produce the string user_name_fixed = "Eloise"?

	a.	user_name_fixed = user_name.strip(":")

	b.	user_name_fixed = user_name.strip()

	c.	**user_name_fixed = user_name.strip(":").strip()**

	d.	user_name_fixed = user_name.strip().strip(":")

3.	Given the list greeting = ["Hello", "my", "name", "is", "Earl"] what line of code would produce a string that contains “Hello_my_name_is_Earl”.

	a.	" ".join(greeting, “_”)
	
	b.	greeting.join(“_”)
	
	c.	**"_".join(greeting)**

	d.	greeting.join()

4.	Which of the following answer choices best describes the function of the string method .find()?

	a.	Find searches a string for its argument and replaces it with its second argument.

	b.	Find searches a string for its argument returns a string of all the characters that come before the argument.

	c.	Find searches a string for its argument and True or False.

	d.	**Find searches a string for its argument returns the index location of that argument.**

5.	Given the following block of code, what is stored in the string split_hairs?

		dirty_harry = "Go ahead, make my day."
		split_hairs = dirty_harry.split("a")
	
	a.	["Go a", "head, ma", "ke my da", "y."]

	b.	**["Go ", "he", "d, m", "ke my d", "y."]**

	c.	["Go", "ahead,", "make”, “my", "day."]

	d.	["Go head, mke my dy”, “a”]

6.	Given the string hello_jerry = "Hi, my name is Jerry", which of the following lines of code will produce the string "Hi, My Name Is Jerry"?

	a.	hello_jerry.upper()

	b.	hello_jerry.lower()

	c.	**hello_jerry.title()**

	d.	hello_jerry.namecase()

7.	Which of the following is a benefit of using .format() to include variables in your strings?

	a.	They let you update variales while printing a string.

	b.	They are able to catch and process errors if a variable does not exist.

	c.	**It makes your code more legible.**

	d.	They let you define variables within a string.
