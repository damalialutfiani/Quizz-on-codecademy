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


