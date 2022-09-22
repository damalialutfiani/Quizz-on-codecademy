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

    >   Coding question

    1.  Create a function named remove_middle which has three parameters named lst, start, and end.

    2.  The function should return a list where all elements in lst with an index between start and end (inclusive) have been removed.

    3.  For example, the following code should return [4, 23, 42] because elements at indices 1, 2, and 3 have been removed:

            remove_middle([4, 8 , 15, 16, 23, 42], 1, 3)

    >   Code :

        #Write your function here
    
        def remove_middle(lst, start, end):
    
            return lst[:start] + lst[end+1:]

        #Uncomment the line below when your function is done

        print(remove_middle([4, 8, 15, 16, 23, 42], 1, 3))

    >   Result  :

      ![python I - 4 2](https://user-images.githubusercontent.com/74751990/191763362-8257f144-8929-4b40-93c9-a8075f80c488.jpg)

3. More Frequent Item

    Let’s go back to our factory example. We have a conveyor belt of items where each item is represented by a different number. We want to know, out of two items, which one shows up more on our belt. To solve this, we can use a function with three parameters. One parameter for the list of items, another for the first item we are comparing, and another for the second item. Here are the steps:

        1.  Define the function to accept three parameters: the list, the first item, and the second item

        2.  Count the number of times item1 shows up in our list

        3.  Count the number of times item2 shows up in our list

        4.  If item1 shows up more, return item1. Otherwise, return item2











