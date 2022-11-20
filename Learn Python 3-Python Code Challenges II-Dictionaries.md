**Python Code Challenges II – Dictionaries**

1.  Sum Values

    For the first code challenge, we are going to look at only the values in a dictionary. This function should sum up all of the values from the key-value pairs in the dictionary. Here are the steps we need:

        a.  Define the function to accept one parameter for our dictionary
        b.  Create a variable to keep track of our sum
        c.  Loop through every value in the dictionary
        d.  Inside the loop, add each value to the sum
        e.  Return the sum

    >   Coding question

        Write a function named sum_values that takes a dictionary named my_dictionary as a parameter. The function should return the sum of the values of the dictionary

    >   Code    :

        # Write your sum_values function here:
        def sum_values(my_dictionary):
          total = 0
          for value in my_dictionary.values():
            total += value
          return total

        # Uncomment these function calls to test your sum_values function:
        print(sum_values({"milk":5, "eggs":2, "flour": 3}))
        # should print 10
        print(sum_values({10:1, 100:2, 1000:3}))
        # should print 6

    >   Result  :

    ![python II - 3 1](https://user-images.githubusercontent.com/74751990/202850797-80fff0c8-d82e-4e01-9e3b-b4649b5cfcaf.jpg)

2.  Even Keys

    Next, we are going to do something similar, but we are going to use the keys in order to retrieve the values. Additionally, we are going to only look at every even key within the dictionary. Here are the steps:

        a.  Define the function to accept one parameter for our dictionary
        b.  Create a variable to keep track of our sum
        c.  Loop through every key in the dictionary
        d.  Inside the loop, if the key is even, add the value from the even key
        e.  After the loop, return the sum

    >   Coding question

        Create a function called sum_even_keys that takes a dictionary named my_dictionary, with all integer keys and values, as a parameter. This function should return the sum of the values of all even keys.

    >   Code    :

        # Write your sum_even_keys function here:
        def sum_even_keys(my_dictionary):
          total = 0
          for key in my_dictionary.keys():
            if key%2 == 0:
              total += my_dictionary[key]
          return total

        # Uncomment these function calls to test your  function:
        print(sum_even_keys({1:5, 2:2, 3:3}))
        # should print 2
        print(sum_even_keys({10:1, 100:2, 1000:3}))
        # should print 6

    >   Result  :

    ![python II - 3 2](https://user-images.githubusercontent.com/74751990/202913392-4907d03d-acfc-436d-be41-bf7cd9e22942.jpg)

3. Add Ten
Let’s loop through the keys again, but this time let’s modify the values within the dictionary. Our function should add 10 to every value in the dictionary and return the modified dictionary. Here is what we need to do:

Define the function to accept one parameter for our dictionary
Loop through every key in the dictionary
Retrieve the value using the key and add 10 to it. Make sure to re-save the new value to the original key.
After the loop, return the modified dictionary







