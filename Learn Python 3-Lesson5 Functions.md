Lesson 5 – **Functions**

1.	What line of code can be used to return a variable inner_var from a function back to the piece of code that called the function?

	a.	inner_var = None
	
	b.	print(inner_var)
	
	c.	**return inner_var**
	
	d.	def inner_var
	
2.	Which variables can be called in the blank spot in this code:

		counter = 0

		def update():
		
			new_counter = counter + 1
			
			return new_counter
			
		_____

	a.	**Just counter**
	
	b.	Neither counter nor new_counter
	
	c.	counter and new_counter
	
	d.	Just new_counter
	
3.	How do you call a function called setup with no arguments?

	a.	def setup():
	
	b.	**setup()**
	
	c.	setup
	
	d.	setup(None)
	
4.	What line of code will call force with a value of 10 for mass and a value of 9.81 for acceleration?

		def force(mass, acceleration):
		
			force_val = mass*acceleration
			
			return force_val


      a.	**force(10, 9.81)**

      b.	force(mass=10, 9.81)
	
      c.	force(10, mass=9.81)
	
      d.	force(9.81, 10)
	
5.	How do you call update with a new_value of 20?

		def update(new_value = 10):
	
			old_value = new_value

	a.	update()
	
	b.	def update()
	
	c.	update
	
	d.	**update(20)**

6.	Given the following function, what will produce the output “There is no greater agony than bearing an untold story inside you.”?

		def quote(x):
			print(“There is no greater agony than bearing “ + x + “ inside you.”)

	a.	def quote(“an untold story”)
	
	b.	quote(an untold story)
	
	c.	**quote(“an untold story”)**
	
	d.	quote()

7.	What happens when you call report()?

		time = “3pm”
		
		mood = “good”
		
		
		def report():
		
			print(“The current time is “ + time)
			
			print(“The mood is “ + mood)
			
		
		print(“Beginning of report”)
		
		report()

	a.	One String is printed: “The current time is 3pm”
	
	b.	**Two Strings are printed: “The current time is 3pm” and “The mood is good”**
	
	c.	Three Strings are printed: “Beginning of report”, “The current time is 3pm”, “The mood is good”
	
	d.	Two Strings are printed: “The current time is ” and “The mood is ”
