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

        # Write your tip function here:

        def tip(total, percentage):

            return (total * percentage) / 100

        # Uncomment these function calls to test your tip function:

        print(tip(10, 25))

        # should print 2.5

        print(tip(0, 100))

        # should print 0.0

    >   Result  :

      ![python I - 8 2](https://user-images.githubusercontent.com/74751990/195116963-b55e7ec2-02cb-4325-81c0-2fdc7584002d.jpg)

3. Bond, James Bond

    It’s time to re-create a famous movie scene through code. Our function is going to concatenate strings together in order to replace James Bond’s name with whatever name we want. The input to our function will be two strings, one for a first name and another for a last name. The function will return a string consisting of the famous phrase but replaced with our inputs. To accomplish this, we need to:

        a.  Define the function to accept two parameters, first_name and last_name

        b.  Concatenate the string ', ' on to the last_name

        c.  Concatenate the first_name on to the result of the previous step

        d.  Concatenate a space on to the result

        e.  Concatenate the last_name again to the result

        f.  Return the final string

    >   Coding question

    1.  Write a function named introduction() that has two parameters named first_name and last_name.

    2.  The function should return the last_name, followed by a comma, a space, first_name another space, and finally last_name.

    >   Code : 

        # Write your introduction function here:

        def introduction(first_name, last_name):

            return (last_name + ", " + first_name + " " + last_name)

        # Uncomment these function calls to test your introduction function:

        print(introduction("James", "Bond"))

        # should print Bond, James Bond

        print(introduction("Maya", "Angelou"))

        # should print Angelou, Maya Angelou

    >   Result  :

      ![python I - 8 3](https://user-images.githubusercontent.com/74751990/195383375-d4dfe03f-c58d-4709-a8b4-8ec4032f4ded.jpg)

4. Dog Years

    Let’s create a function which calculates a dog’s age in dog years! This function will accept the name of the dog and the age in human years. It will calculate the age of the dog in dog years and return a string describing the dog’s age. This will require a few steps:

        a.  Define the function called dog_years to accept two parameters: name and age

        b.  Calculate the age of the dog in dog years

        c.  Concatenate the string with the dog’s name and age in dog years

        d.  Return the resulting string

    >   Coding question

    1.  Some say that every one year of a human’s life is equivalent to seven years of a dog’s life. Write a function named dog_years() that has two parameters named name and age.

    2.  The function should compute the age in dog years and return the following string:

            "{name}, you are {age} years old in dog years"

    3.  Test this function with your name and your age!

    >   Code : 

        # Write your dog_years function here:

        def dog_years(name, age):

            return (name + ", you are " + str(age * 7) + " years old in dog years")

        # Uncomment these function calls to test your dog_years function:

        print(dog_years("Lola", 16))

        # should print "Lola, you are 112 years old in dog years"

        print(dog_years("Baby", 0))

        # should print "Baby, you are 0 years old in dog years"

    >   Result  :

      ![python I - 8 4](https://user-images.githubusercontent.com/74751990/195519671-241f35ea-37e6-41f1-abcd-659a6d8ee3d0.jpg)

5. All Operations

    For the final code challenge, we are going to perform multiple mathematical operations on multiple inputs to the function. We will begin with adding the first two inputs, then we will subtract the third and fourth inputs. After that, we will multiply the first result and the second result. In the end, we will return the remainder of the previous result divided by the first input. We will also print each of the steps. The steps needed to complete this are:

        a.  Define the function to accept four inputs: a, b, c, and d

        b.  Print and store the result of a + b

        c.  Print and store the result of c - d

        d.  Print and store the first result times the second result

        e.  Return the previous result modulo a


















