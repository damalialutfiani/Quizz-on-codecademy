Lesson 10 – **Introduction to Classes**

1.    What does the hasattr() function call in the last line here evaluate to?

                class HoldsFive:
                        five = 5

                five_holder = HoldsFive()
                hasattr(five_holder, 'five')

      a.      **True**
      
      b.      False
      
      c.	5

2.    What function, defined within a class, provides instructions on what to assign to a new instance when it is created?

      a.      **__ init __**

      b.        __ create __
       
      c.	init

      d.	__ new __

3.    What is the first argument of a method?

      a.      The context in which the object is created. We usually name the parameter this.

      b.      **The instance of the object itself. We usually refer to it as self.**

      c.      The class itself. We usually refer to it as self.

4.    What would be printed from the following code?

                class User:
 		        def __init__(self, name):
    			        self.name = name
    	 		
                        def __repr__(self):
   			        return "Hiya {}!".format(self.name)
  	
                devorah = User("Devorah")
                print(devorah)

      a.	**Hiya Devorah!**

      b.	Devorah

      c.	Hiya devorah!

      d.	Devorah

5.	What keyword is used to indicate the start of a class definition?

    a.  __init__
  
    b.  Def

    c.  **Class**

    d.  Type

6.	What does the type() function do in Python?

    a.  Returns a type object that contains some metadata about the class.

    b.  **Returns the class that an object implements.**

    c.  Returns a string that’s the name of the class.

    d.  Returns an implementation of a class.

7.	How would we create an instance of the following class?
class NiceClass:
 		neat_attribute = "neat"
-	**nice_instance = NiceClass()**
-	nice_instance = new NiceClass
-	nice_instance = NiceClass
