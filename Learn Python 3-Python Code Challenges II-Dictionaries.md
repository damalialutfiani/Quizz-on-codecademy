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

3.  Add Ten

    Let’s loop through the keys again, but this time let’s modify the values within the dictionary. Our function should add 10 to every value in the dictionary and return the modified dictionary. Here is what we need to do:

        a.  Define the function to accept one parameter for our dictionary
        b.  Loop through every key in the dictionary
        c.  Retrieve the value using the key and add 10 to it. Make sure to re-save the new value to the original key.
        d.  After the loop, return the modified dictionary

    >   Coding question

        Create a function named add_ten that takes a dictionary with integer values named my_dictionary as a parameter. The function should add 10 to every value in my_dictionary and return my_dictionary

    >   Code    :

        # Write your add_ten function here:
        def add_ten(my_dictionary):
          for key in my_dictionary.keys():
            my_dictionary[key] += 10
          return my_dictionary

        # Uncomment these function calls to test your  function:
        print(add_ten({1:5, 2:2, 3:3}))
        # should print {1:15, 2:12, 3:13}
        print(add_ten({10:1, 100:2, 1000:3}))
        # should print {10:11, 100:12, 1000:13}

    >   Result  :

    ![python II - 3 3](https://user-images.githubusercontent.com/74751990/202928555-01368bb1-c4bd-46df-9e64-3c0d8c0cc27b.jpg)

4.  Values That Are Keys

    We are making a program that will create a family tree. Using a dictionary, we want to return a list of all the children who are also parents of other children. Using dictionaries we can consider those people to be values which are also keys in our dictionary of family data. Here is what we need to do:

        a.  Define the function to accept one parameter for our dictionary
        b.  Create an empty list to hold the values we find
        c.  Loop through every value in the dictionary
        d.  Inside the loop, test if the current value is a key in the dictionary. If it is then append it to the list of values we found
        e.  After the loop, return the list of values which are also keys

    >   Coding question

        Create a function named values_that_are_keys that takes a dictionary named my_dictionary as a parameter. This function should return a list of all values in the dictionary that are also keys.

    >   Code    :

        # Write your values_that_are_keys function here:
        def values_that_are_keys(my_dictionary):
          value_keys = []
          for value in my_dictionary.values():
            if value in my_dictionary:
              value_keys.append(value)
          return value_keys

        # Uncomment these function calls to test your  function:
        print(values_that_are_keys({1:100, 2:1, 3:4, 4:10}))
        # should print [1, 4]
        print(values_that_are_keys({"a":"apple", "b":"a", "c":100}))
        # should print ["a"]

    >   Result  :

    ![python II - 3 4](https://user-images.githubusercontent.com/74751990/203692688-4e45317c-6413-42c7-9764-75974159be81.jpg)

5.  Largest Value

    For the last challenge, we are going to create a function that is able to find the maximum value in the dictionary and return the associated key. This is a twist on the max algorithm since it is using a dictionary rather than a list. These are the steps:

        a.  Define the function to accept one parameter for our dictionary
        b.  Initialize the starting key to a very low number
        c.  Initialize the starting value to a very low number
        d.  Iterate through the dictionary’s key/value pairs.
        e.  Inside the loop, if the current value is larger than the current largest value, replace the largest key and largest value with the current ones you are looking at
        f.  Once you are done iterating through all key/value pairs, return the key which has the largest value







