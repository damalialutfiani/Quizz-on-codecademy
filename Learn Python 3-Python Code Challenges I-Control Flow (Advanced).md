**Python Code Challenges I - Control Flow (Advanced)**

1. In Range

    Let’s start the advanced challenge problems by testing if a number falls within a certain range. We will accept three parameters where the first parameter is the number we are testing, the second parameter is the lower bound and the third parameter is the upper bound of our range. These are the steps required:

        a.  Define the function to accept three numbers as parameters.
  
        b.  Test if the number is greater than or equal to the lower bound and less than or equal to the upper bound.
  
        c.  If this is true, return True, otherwise, return False

      >   Coding question

    1.  Create a function named in_range() that has three parameters named num, lower, and upper.
    
    2.  The function should return True if num is greater than or equal to lower and less than or equal to upper. Otherwise, return False.
  
    >   Code :

        # Write your in_range function here:

        def in_range(num, lower, upper):
  
          if num >= lower and num <= upper:
    
            return True
  
          else:
    
            return False

        # Uncomment these function calls to test your in_range function:

        print(in_range(10, 10, 10))

        # should print True

        print(in_range(5, 10, 20))

        # should print False

    >   Result :
  
      ![python I - 2 1](https://user-images.githubusercontent.com/74751990/189597019-01fee086-bb99-4312-8dfd-f4bf2584db7f.jpg)

2. Same Name
  
    We need to write a program that checks different names and determines if they are equal. We need to accept two strings and compare them. Here are the steps:

        a.  Define the function to accept two strings, your_name and my_name
        
        b.  Test if the two strings are equal
        
        c.  Return True if they are equal, otherwise return False

      >   Coding question
  
Create a function named same_name() that has two parameters named your_name and my_name.

If our names are identical, return True. Otherwise, return False.
  
  
      >   Code :
      
      
      # Write your same_name function here:
def same_name(your_name, my_name):
  if your_name == my_name:
    return True
  else:
    return False

# Uncomment these function calls to test your same_name function:
print(same_name("Colby", "Colby"))
# should print True
print(same_name("Tina", "Amber"))
# should print False

    >   Result :

      
      
      
      
