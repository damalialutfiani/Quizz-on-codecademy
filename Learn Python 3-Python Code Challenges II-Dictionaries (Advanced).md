**Python Code Challenges II – Dictionaries (Advanced)**

1.  Word Length Dict

    Let’s start by writing a function that creates a new dictionary based on a list of strings. The keys of our dictionary will be every string in our list of strings, while the values will be the length of each of the words in the string list. Here are the steps:

        a.  Define the function to accept one parameter for our list of strings
        b.  Create a new empty dictionary
        c.  Loop through every string in the list of strings
        d.  Inside the loop, add the string as a key and the length of the string as the value to the dictionary
        e.  After the loop, return the new dictionary

    >   Coding question

        Write a function named word_length_dictionary that takes a list of strings named words as a parameter. The function should return a dictionary of key/value pairs where every key is a word in words and every value is the length of that word.

    >   Code    :

        # Write your word_length_dictionary function here:
        def word_length_dictionary(words):
          word_lengths = {}
          for word in words:
            word_lengths[word] = len(word)
          return word_lengths

        # Uncomment these function calls to test your  function:
        print(word_length_dictionary(["apple", "dog", "cat"]))
        # should print {"apple":5, "dog": 3, "cat":3}
        print(word_length_dictionary(["a", ""]))
        # should print {"a": 1, "": 0}

    >   Result  :

    ![python II - 4 1](https://user-images.githubusercontent.com/74751990/203868526-4d4581d3-5776-4477-bff1-3c0e3348dbc6.jpg)

2.  Frequency Count

    This next function is similar, but instead of counting the length of each string in the list of strings, we will be counting the frequency of each string. This function will also accept a list of strings as input and return a new dictionary. Here is what we need to do:

        a.  Define the function to accept one parameter for our list of strings
        b.  Create a new empty dictionary
        c.  Loop through every string in the list of strings
        d.  Inside the loop, if the string is not already in our dictionary, store the string as a key with a value of 0 in our dictionary. Then, increment the value by 1.
        e.  After the loop, return the new dictionary

    >   Coding question

        Write a function named frequency_dictionary that takes a list of elements named words as a parameter. The function should return a dictionary containing the frequency of each element in words.

    >   Code    :

        # Write your frequency_dictionary function here:
        def frequency_dictionary(words):
          freqs = {}
          for word in words:
            if word not in freqs:
              freqs[word] = 0
            freqs[word] += 1
          return freqs

        # Uncomment these function calls to test your  function:
        print(frequency_dictionary(["apple", "apple", "cat", 1]))
        # should print {"apple":2, "cat":1, 1:1}
        print(frequency_dictionary([0,0,0,0,0]))
        # should print {0:5}

    >   Result  :

    ![python II - 4 2](https://user-images.githubusercontent.com/74751990/203868897-bb83bbfe-d4fd-4e3e-ab5f-e0c24dcb0ab9.jpg)

3.  Unique Values

    Now let’s try reading a dictionary as input and finding how many values are unique. The function should return a number which is the count of all values from the dictionary without including duplicates. These are the steps:

        a.  Define the function to accept one parameter for our dictionary
        b.  Create a new empty list
        c.  Loop through every value in our dictionary
        d.  Inside the loop, if the value is not already in our list, append the value to our list
        e.  After the loop, return the length of our list

    >   Coding question

        Create a function named unique_values that takes a dictionary named my_dictionary as a parameter. The function should return the number of unique values in the dictionary.

    >   Code    :

        # Write your unique_values function here:
        def unique_values(my_dictionary):
          seen_values = []
          for value in my_dictionary.values():
            if value not in seen_values:
              seen_values.append(value)
          return len(seen_values)

        # Uncomment these function calls to test your  function:
        print(unique_values({0:3, 1:1, 4:1, 5:3}))
        # should print 2
        print(unique_values({0:3, 1:3, 4:3, 5:3}))
        # should print 1

    >   Result  :

    ![python II - 4 3](https://user-images.githubusercontent.com/74751990/204062922-b4cd40fb-b7ca-46c6-8be9-33e12e3d5bd1.jpg)



