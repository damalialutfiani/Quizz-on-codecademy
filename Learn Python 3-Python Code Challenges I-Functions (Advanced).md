**Python Code Challenges I-Functions (Advanced)**

1. First Three Multiples

    Let’s start by creating a function which both prints and returns values. For this function, we are going to print out the first three multiples of a number and return the third multiple. This means that we are going to print 1, 2, and 3 times the input number and then return the value of 3 times the input number. For this, we are going to need a few steps:

        a.  Define the function header to accept one input parameter called num

        b.  Print out 1 times num
      
        c.  Print out 2 times num
      
        d.  Print out 3 times num
      
        e.  Return the value of 3 times num
        
    >   Coding question
        
    1.  Write a function named first_three_multiples() that has one parameter named num.

    2.  This function should print the first three multiples of num. Then, it should return the third multiple.

    3.  For example, first_three_multiples(7) should print 7, 14, and 21 on three different lines, and return 21.    
        
    >   Code :      
        
        # Write your first_three_multiples function here

        def first_three_multiples(num):

            list = num * 1, num * 2, num * 3

            print(list)
 
            return list[-1]

        # Uncomment these function calls to test your first_three_multiples function:

        first_three_multiples(10)

        # should print 10, 20, 30, and return 30

        first_three_multiples(0)

        # should print 0, 0, 0, and return 0        
        
    >   Result  :

      ![python I - 8 1](https://user-images.githubusercontent.com/74751990/194825115-9b25edde-c82f-4b5c-83e3-4a6a70306612.jpg)

2. Tip

    Let’s say we are going to a restaurant and we decide to leave a tip. We can create a function to easily calculate the amount to tip based on the total cost of the food and a percentage. This function will accept both of those values as inputs and return the amount of money to tip. In order to do this, we will need a few steps:

        a.  Define the function to accept the total cost of the food called total and the percentage to tip as percentage

        b.  Calculate the tip amount by multiplying the total and percentage and dividing by 100

        c.  Return the tip amount

    >   Coding question

    1.  Create a function called tip() that has two parameters named total and percentage.

    2.  This function should return the amount you should tip given a total and the percentage you want to tip.

    >   Code : 



    >   Result  :










