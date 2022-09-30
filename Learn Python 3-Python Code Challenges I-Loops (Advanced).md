**Python Code Challenges I - Loops (Advanced)**

1. Larger Sum

    We are going to start our advanced challenge problems by calculating which list of two inputs has the larger sum. We will iterate through each of the list and calculate the sums, afterwards we will compare the two and return which one has a greater sum. Here are the steps we need:

        a.  Define the function to accept two input parameters: lst1 and lst2

        b.  Create two variables to record the two sums

        c.  Loop through the first list and add up all of the numbers

        d.  Loop through the second list and add up all of the numbers

        e.  Compare the first and second sum and return the list with the greater sum

    >   Coding question

    1.  Create a function named larger_sum() that takes two lists of numbers as parameters named lst1 and lst2.

    2.  The function should return the list whose elements sum to the greater number. If the sum of the elements of each list are equal, return lst1.

    >   Code :

        #Write your function here

        def larger_sum(lst1, lst2):

            sum1 = 0

            sum2 = 0

            for num in lst1:

                sum1 += num

            for num in lst2:

                sum2 += num

            if sum1 >= sum2:
 
                return lst1

            else:

                return lst2

        #Uncomment the line below when your function is done

        print(larger_sum([1, 9, 5], [2, 3, 7]))

    >   Result  :

      ![python I - 6 1](https://user-images.githubusercontent.com/74751990/193361567-839c8c01-7174-4fb2-9af4-5d24ce7e02b4.jpg)






