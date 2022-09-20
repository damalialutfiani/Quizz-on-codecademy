**Python Code Challenges I - Lists**

1. Append Size

    For the first code challenge, we are going to calculate the length of a list and then append the value to the end of the list. Here is what we need to do:

        a.  Define the function to accept one parameter for our list
      
        b.  Get the length of the list
      
        c.  Append the length of the list to the end of the list
      
        d.  Return the modified list
      
    >   Coding question
    
    1.  Create a function called append_size that has one parameter named lst.

    2.  The function should append the size of lst (inclusive) to the end of lst. The function should then return this new list.

    3.  For example, if lst was [23, 42, 108], the function should return [23, 42, 108, 3] because the size of lst was originally 3.
    
    >   Code :
    
        #Write your function here

        def append_size(lst):
  
            lst.append(len(lst))
  
            return lst

        #Uncomment the line below when your function is done

        print(append_size([23, 42, 108]))
    
    >   Result  :
      
      ![python I - 3 1](https://user-images.githubusercontent.com/74751990/190638363-936fd924-cc95-46bc-a7ef-40088abe3fa2.jpg)
      
2. Append Sum

    Let’s create a function that calculates the sum of the last two elements of a list and appends it to the end. After doing so, it will repeat this process two more times and return the resulting list. You can choose to use a loop or manually use three lines. Here are the steps we need:

        a.  Define the function to accept one parameter for our list of numbers

        b.  Add the last and second to last elements from our list together

        c.  Append the calculated value to the end of our list.

        d.  Repeat steps 2 and 3 two more times

        e.  Return the modified list

    >   Coding question

    1.  Write a function named append_sum that has one parameter — a list named named lst.

    2.  The function should add the last two elements of lst together and append the result to lst. It should do this process three times and then return lst.

    3.  For example, if lst started as [1, 1, 2], the final result should be [1, 1, 2, 3, 5, 8].

    >   Code :

        #Write your function here

            def append_sum(lst):

            lst.append(lst[-1]+lst[-2])

            lst.append(lst[-1]+lst[-2])

            lst.append(lst[-1]+lst[-2])

            return lst

        #Uncomment the line below when your function is done
    
        print(append_sum([1, 1, 2]))

    >   Result  :   
   
      ![python I - 3 2](https://user-images.githubusercontent.com/74751990/190858912-7a290c29-dc48-40d3-bf05-5398857c2968.jpg)
   
3. Larger List

    Let’s say we are working with two conveyor belts that contain items represented by a numerical ID. If one conveyor belt contains more items than the other, then we need to return the ID of the last item on that belt. In the case where they have the same number of items, return the last item from the first conveyor belt. In our code, we can represent the belts using lists. Here are the steps:

        a.  Define the function to accept two parameters for our two lists of numbers

        b.  Check if the length of the first list is greater than or equal to the length of the second list

        c.  If true, then return the last element from the first list. Otherwise, return the last element from the second list   
   
    >   Coding question

    1.  Write a function named larger_list that has two parameters named lst1 and lst2.

    2.  The function should return the last element of the list that contains more elements. If both lists are the same size, then return the last element of lst1.

    >   Code :

        #Write your function here

        def larger_list(lst1, lst2):

            if len(lst1) >= len(lst2):

                return lst1[-1]

            else:

                return lst2[-1]

        #Uncomment the line below when your function is done

        print(larger_list([4, 10, 2, 5], [-10, 2, 5, 10]))

    >   Result  :  

      ![python I - 3 3](https://user-images.githubusercontent.com/74751990/190869886-0f87eb03-33f8-4241-aaab-a370facf990b.jpg)

4. More Than N

    Our factory produces a variety of different flavored snacks and we want to check the number of instances of a certain type. We have a conveyor belt full of different types of snacks represented by different numbers. Our function will accept a list of numbers (representing the type of snack), a number for the second parameter (the type of snack we are looking for), and another number as the third parameter (the maximum number of that type of snack on the conveyor belt). The function will return True if the snack we are searching for appears more times than we provided as our third parameter. These are the steps we need:

        a.  Define the function to accept three parameters, a list of numbers, a number to look for, and a number for the number of instances

        b.  Count the number of occurrences of item (the second parameter) in lst (the first parameter)

        c.  If the number of occurrences is greater than n (the third parameter), return True. Otherwise, return False

    >   Coding question

    1.  Create a function named more_than_n that has three parameters named lst, item, and n.

    2.  The function should return True if item appears in the list more than n times. The function should return False otherwise.

    >   Code :

        #Write your function here

        def more_than_n(lst, item, n):

            if lst.count(item) > n :

                return True

            else:

                return False

        #Uncomment the line below when your function is done

        print(more_than_n([2, 4, 6, 2, 3, 2, 1, 2], 2, 3))

    >   Result  :  

      ![python I - 3 4](https://user-images.githubusercontent.com/74751990/190928460-b4edc51f-9a4d-4218-b937-3ddee4f9980e.jpg)

5. Combine Sort

    Finally, let’s create a function that combines two different lists together and then sorts them. To do this we can combine the lists with an operation and then sort using a function call. Here are the steps we need to use:

        a.  Define the function to accept two parameters, one for each list.

        b.  Combine the two lists together

        c.  Sort the result

        d.  Return the sorted and combined list

    >   Coding question

    1.  Write a function named combine_sort that has two parameters named lst1 and lst2.

    2.  The function should combine these two lists into one new list and sort the result. Return the new sorted list.

    >   Code :

        #Write your function here

        def combine_sort(lst1, lst2):

            newlist = sorted(lst1 + lst2)

            return newlist

        #Uncomment the line below when your function is done

        print(combine_sort([4, 10, 2, 5], [-10, 2, 5, 10]))

    >   Result  :  



