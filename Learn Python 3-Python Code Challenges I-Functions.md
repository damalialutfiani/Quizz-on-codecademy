**Python Code Challenges I - Functions**

1. Tenth Power

    Let’s create some functions which can help us solve math problems! For this first function, we are going to take the tenth power of a number. In order to do this we need to do three things:

        a.  Set up the function header for tenth_power which accepts one parameter

        b.  Take the tenth power of the input value

        c.  Return the result
    
    >   Coding question
    
    1.  Write a function named tenth_power() that has one parameter named num.

    2.  The function should return num raised to the 10th power.
    
    >   Code :

        # Write your tenth_power function here:
        
        def tenth_power(num):

            return num ** 10

        # Uncomment these function calls to test your tenth_power function:

        print(tenth_power(1))

        # 1 to the 10th power is 1

        print(tenth_power(0))

        # 0 to the 10th power is 0

        print(tenth_power(2))

        # 2 to the 10th power is 1024

    >   Result  :

      ![python I - 7 1](https://user-images.githubusercontent.com/74751990/194049614-018943e3-5b04-40e8-8aa3-fd07de514354.jpg)

2. Square Root

    Another useful function for solving math problems is the square root function. We can create this using similar steps from the last problem. The code will look very similar. We need to:

        a.  Set up the function header for square_root which accepts one parameter

        b.  Take the square root of the input value

        c.  Return the result

    >   Coding question

    1.  Write a function named square_root() that has one parameter named num.

    2.  Use exponents (**) to return the square root of num.

    >   Code :

        # Write your square_root function here:

        def square_root(num):

            return num ** 0.5

        # Uncomment these function calls to test your square_root function:

        print(square_root(16))

        # should print 4

        print(square_root(100))

        # should print 10

    >   Result  :

      ![python I - 7 2](https://user-images.githubusercontent.com/74751990/194330948-e8014922-64eb-447a-a110-65ca6358b647.jpg)

3. Win Percentage

    Next, we will create a function which calculates the percentage of games won. In order to do this, we will need to know how many total games there were and divide the number of wins by the total number of games. For this function, there will be two input parameters, the number of wins and the number of losses. We also need to make sure that we return the result as a percentage (in the range of 0 to 100). In order to create this method we need the following steps:

        a.  Define the function header with two parameters, wins and losses

        b.  Calculate the total number of games using the number of wins and losses

        c.  Get the ratio of winning using the number of wins out of the total number of games.

        d.  Convert the ratio to a percentage

        e.  Return the percentage


    >   Coding question

    1.  Create a function called win_percentage() that takes two parameters named wins and losses.

    2.  This function should return out the total percentage of games won by a team based on these two numbers.

    >   Code :

        # Write your win_percentage function here:

        def win_percentage(wins, losses):

            return wins / (wins + losses) * 100

        # Uncomment these function calls to test your win_percentage function:

        print(win_percentage(5, 5))

        # should print 50

        print(win_percentage(10, 0))

        # should print 100

    >   Result  :

      ![python I - 7 3](https://user-images.githubusercontent.com/74751990/194445343-253dbd04-e80b-4ac5-a3ec-81d150f62c81.jpg)

4. Average

    Let’s create a function which takes the average of two numbers. These two numbers will be the input of the function and the output will be the average of the two. In order to do this, we need to do a few steps:

        a.  Define the function with two input parameters, num1 and num2

        b.  Calculate the sum of the two numbers

        c.  Divide the sum by the number of inputs to the function

        d.  Return the answer

    >   Coding question

    1.  Write a function named average() that has two parameters named num1 and num2.

    2.  The function should return the average of these two numbers.

    >   Code :

        # Write your average function here:

        def average(num1, num2):

            return (num1 + num2) / 2

        # Uncomment these function calls to test your average function:

        print(average(1, 100))

        # The average of 1 and 100 is 50.5

        print(average(1, -1))

        # The average of 1 and -1 is 0

    >   Result  :

      ![python I - 7 4](https://user-images.githubusercontent.com/74751990/194713127-9b88e5d3-3792-4bd3-9b1a-653596ed7a33.jpg)

5. Remainder

    For the final challenge in this group, we are going to take the remainder of two numbers while performing other mathematical operations on them. We are going to multiply the numerator by 2 and divide the denominator by 2. After the two values have been modified, we will divide them and return the remainder. In order to do this we will need to:

        a.  Define the function to accept two parameters

        b.  Multiply the first input value by 2

        c.  Divide the second input value by 2

        d.  Calculate the remainder of the modified first input value divided by the modified second input value (using modulus)

        e.  Return the answer























