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

2. Over 9000

    We are constructing a device that is able to measure the power level of our coding abilities and according to the device, it will be impossible for our power levels to be over 9000. Because of this, as we iterate through a list of power values we will count up each of the numbers until our sum reaches a value greater than 9000. Once this happens, we should stop adding the numbers and return the value where we stopped. In order to do this, we will need the following steps:

        a.  Define the function to accept a list of numbers

        b.  Create a variable to keep track of our sum

        c.  Iterate through every element in our list of numbers

        d.  Within the loop, add the current number we are looking at to our sum

        e.  Still within the loop, check if the sum is greater than 9000. If it is, end the loop

        f.  Return the value of the sum when we ended our loop

    >   Coding question

    1.  Create a function named over_nine_thousand() that takes a list of numbers named lst as a parameter.

    2.  The function should sum the elements of the list until the sum is greater than 9000. When this happens, the function should return the sum. If the sum of all of the elements is never greater than 9000, the function should return total sum of all the elements. If the list is empty, the function should return 0.

    3.  For example, if lst was [8000, 900, 120, 5000], then the function should return 9020.

    >   Code :

        #Write your function here

        def over_nine_thousand(lst):

            sum = 0

            for number in lst:

                sum += number

                if (sum > 9000):

                    break

            return sum

        #Uncomment the line below when your function is done

        print(over_nine_thousand([8000, 900, 120, 5000]))

    >   Result  :

      ![python I - 6 2](https://user-images.githubusercontent.com/74751990/193464835-307a72e4-09ce-46ca-9f42-ce987174ae97.jpg)

3. Max Num

    Here is a more traditional coding problem for you. This function will be used to find the maximum number in a list of numbers. This can be accomplished using the max() function in python, but as a challenge, we are going to manually implement this function. Here is what we need to do:

        a.  Define the function to accept a list of numbers called nums

        b.  Set our default maximum value to be the first element in the list

        c.  Loop through every number in the list of numbers

        d.  Within the loop, if we find a number greater than our starting maximum, then replace the maximum with what we found.

        e.  Return the maximum number

    >   Coding question

    1.  Create a function named max_num() that takes a list of numbers named nums as a parameter.

    2.  The function should return the largest number in nums

    >   Code :



    >   Result  :







