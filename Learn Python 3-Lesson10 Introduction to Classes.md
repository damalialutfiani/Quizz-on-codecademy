Lesson 10 – **Introduction to Classes**

1.	What does the hasattr() function call in the last line here evaluate to?

        class HoldsFive:
          five = 5

        five_holder = HoldsFive()
        hasattr(five_holder, 'five')

      a.      **True**
      
      b.      False
      
      c.	5

2.	What function, defined within a class, provides instructions on what to assign to a new instance when it is created?

      a.      **__ init __**

      b.        __ create __
       
      c.	init

      d.	__ new __

3.	What is the first argument of a method?

      a.      The context in which the object is created. We usually name the parameter this.

      b.      **The instance of the object itself. We usually refer to it as self.**

      c.      The class itself. We usually refer to it as self.

4.	What would be printed from the following code?

                class User:
 		        def __init__(self, name):
    			        self.name = name
    	 		
                        def __repr__(self):
   			        return "Hiya {}!".format(self.name)
  	
                devorah = User("Devorah")
                print(devorah)

-	**Hiya Devorah!**
-	Devorah
-	Hiya devorah!
-	Devorah
