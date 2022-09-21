**Python Code Challenges I - Lists (Advanced)**

1. Every Three Numbers

    Let’s start our challenging problems with a function that creates a list of numbers up to 100 in increments of 3 starting from a number that is passed to the function as an input parameter. Here is what we need to do:

        a.  Define the function to accept one parameter for our starting number

        b.  Calculate the numbers between the starting number and 100 while incrementing by 3

        c.  Store the numbers in a list

        d.  Return the list

    >   Coding question

    1.  Create a function called every_three_nums that has one parameter named start.

    2.  The function should return a list of every third number between start and 100 (inclusive). For example, every_three_nums(91) should return the list [91, 94, 97, 100]. If start is greater than 100, the function should return an empty list.

    >   Code :

        #Write your function here

        def every_three_nums(start):

            return list(range(start, 101, 3))

        #Uncomment the line below when your function is done

        print(every_three_nums(91))

    >   Result  :

      ![python I - 4 1](https://user-images.githubusercontent.com/74751990/191417206-68ec8efd-d01e-4877-9c74-0ede35fc3104.jpg)

2. Remove Middle

    Our next function will remove all elements from a list with an index within a certain range. The function will accept a list, a starting index, and an ending index. All elements with an index between the starting and ending index should be removed from the list. Here are the steps:

        a.  Define the function to accept three parameters: the list, the starting index, and the ending index

        b.  Get all elements before the starting index

        c.  Get all elements after the ending index

        d.  Combine the two partial lists into the result

        e.  Return the result








