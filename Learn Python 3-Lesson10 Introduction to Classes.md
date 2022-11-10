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
-	The context in which the object is created. We usually name the parameter this.
-	**The instance of the object itself. We usually refer to it as self.**
-	The class itself. We usually refer to it as self.

