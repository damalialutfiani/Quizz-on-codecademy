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

        a.  Define the function to accept three parameters: the list, the first item, and the second item

        b.  Count the number of times item1 shows up in our list

        c.  Count the number of times item2 shows up in our list

        d.  If item1 shows up more, return item1. Otherwise, return item2

    >   Coding question

    1.  Create a function named more_frequent_item that has three parameters named lst, item1, and item2.

    2.  Return either item1 or item2 depending on which item appears more often in lst.

    3.  If the two items appear the same number of times, return item1.

    >   Code :

        #Write your function here

        def more_frequent_item(lst, item1, item2):
 
            if lst.count(item1) >= lst.count(item2):

                return item1

            else:

                return item2

        #Uncomment the line below when your function is done

        print(more_frequent_item([2, 3, 3, 2, 3, 2, 3, 2, 3], 2, 3))

    >   Result  :

      ![python I - 4 3](https://user-images.githubusercontent.com/74751990/191766378-2d8f60d2-e6ec-4fac-a88b-0ee4905c90f1.jpg)

4. Double Index

    Our next function will double a value at a given position. We will provide a list and an index to double. This will create a new list by replacing the value at the index provided with double the original value. If the index is invalid then we should return the original list. Here is what we need to do:

        a.  Define the function to accept two parameters, one for the list and another for the index of the value we are going to double

        b.  Test if the index is invalid. If its invalid then return the original list

        c.  If the list is valid then get all values up to the index and store it as a new list

        d.  Append the value at the index times 2 to the new list

        e.  Add the rest of the list from the index onto the new list

        f.  Return the new list

    >   Coding question

    1.  Create a function named double_index that has two parameters: a list named lst and a single number named index.

    2.  The function should return a new list where all elements are the same as in lst except for the element at index. The element at index should be double the value of the element at index of the original lst.

    3.  If index is not a valid index, the function should return the original list.

    4.  For example, the following code should return [1,2,6,4] because the element at index 2 has been doubled:

            double_index([1, 2, 3, 4], 2)

    5.  After writing your function, un-comment the call to the function that we’ve provided for you to test your results.

    >   Code :

        #Write your function here

        def double_index(lst, index):

        # Checks to see if index is too big

            if index >= len(lst):

                return lst

            else:

                # Gets the original list up to index

                new_lst = lst[0:index]

        # Adds double the value at index to the new list 

            new_lst.append(lst[index]*2)

            #  Adds the rest of the original list

            new_lst = new_lst + lst[index+1:]

            return new_lst

        #Uncomment the line below when your function is done

        print(double_index([3, 8, -10, 12], 2))

    >   Result  :

      ![python I - 4 4](https://user-images.githubusercontent.com/74751990/191827460-12072613-2c12-4524-9c81-e71255c537e5.jpg)

5. Middle Item

    For the final code challenge, we are going to create a function that finds the middle item from a list of values. This will be different depending on whether there are an odd or even number of values. In the case of an odd number of elements, we want this function to return the exact middle value. If there is an even number of elements, it returns the average of the middle two elements. Here is what we need to do:

        a.  Define the function to accept one parameter for our list of numbers

        b.  Determine if the length of the list is even or odd

        c.  If the length is even, then return the average of the middle two numbers

        d.  If the length is odd, then return the middle number

    >   Coding question

    1.  Create a function called middle_element that has one parameter named lst.

    2.  If there are an odd number of elements in lst, the function should return the middle element. If there are an even number of elements, the function should return the average of the middle two elements.

    >   Code :



    >   Result  :


