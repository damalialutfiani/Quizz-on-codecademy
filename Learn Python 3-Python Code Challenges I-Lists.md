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
   
   
   
   
