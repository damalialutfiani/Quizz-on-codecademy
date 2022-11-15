**Python Code Challenges II - Strings**

1.  Count Letters

    For the first code challenge, we are going to count the number of unique letters in a string. This means that when we are looking at the word, any new letters should be counted and any duplicates should not be counted. There are a few ways to solve this, but we can use the provided alphabet string to ensure that duplicates are not counted. Here is what we need to do:

        a.  Define the function to accept one parameter — the word whose letters we are counting
        b.  Create a counter to keep track of unique letters
        c.  Loop through every letter in our alphabet string. If the current letter was found in our word, increase our count
        d.  Return the count after looping through all letters.

    >   Coding question

    1.  Write a function called unique_english_letters that takes the string word as a parameter. The function should return the total number of unique letters in the string. Uppercase and lowercase letters should be counted as different letters.

    2.  We’ve given you a list of every uppercase and lower case letter in the English alphabet. It will be helpful to include that list in your function.

    >   Code    :

        letters = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz"
        
        # Write your unique_english_letters function here:
        def unique_english_letters(word):
          uniques = 0
          for letter in letters:
            if letter in word:
              uniques += 1
          return uniques

        # Uncomment these function calls to test your function:
        print(unique_english_letters("mississippi"))
        # should print 4
        print(unique_english_letters("Apple"))
        # should print 4

    >   Result  :

    ![python II - 1 1](https://user-images.githubusercontent.com/74751990/201520487-629fdf9d-f8b2-4f90-9240-9fddad6228f5.jpg)

2.  Count X

    Next, we are going to try something a bit different. This time we are going to count the number of occurrences of a certain letter within a string. Our function will accept a parameter for a string and another for the character which we are going to count. For example, providing the word "mississippi" and the character 's' would result in an answer of 4. These are the steps we need to take:

        a.  Define the function to accept two parameters. word for the input string and x for the single character
        b.  Create a counter to keep track of the occurrences
        c.  Loop through every letter in the string. If the current letter is equal to the input letter, increase our counter
        d.  Return the counter after looping through the entire string.

    >   Coding question

        Write a function named count_char_x that takes a string named word and a single character named x as parameters. The function should return the number of times x appears in word.
    
    >   Code    :

        # Write your count_char_x function here:
        def count_char_x(word, x):
          occurrences = 0
          for letter in word:
            if letter == x:
              occurrences += 1
          return occurrences

        # Uncomment these function calls to test your tip function:
        print(count_char_x("mississippi", "s"))
        # should print 4
        print(count_char_x("mississippi", "m"))
        # should print 1

    >   Result  :

    ![python II - 1 2](https://user-images.githubusercontent.com/74751990/201572796-2b3801ce-cd5d-43a3-a507-a29a45ac6044.jpg)

3.  Count Multi X

    Now let’s change our function to compare against an entire string instead of a single character. This function should accept a string and a substring to compare against. The number of occurrences of the second parameter within the first parameter string are returned. What this means is that we are checking the number of occurrences of the shorter string (second parameter) within the longer string (first parameter). One way to accomplish this is using the split function. Here is how to do that:

        a.  Define the function to accept two parameters. word for the input string and x for the second string we are searching for
        b.  Split the string into substrings based on the second input parameter
        c.  Count the number of instances the substring appeared in the first input string based on the split string
        d.  Return the result

    >   Coding question

    1.  Write a function named count_multi_char_x that takes a string named word and a string named x. This function should do the same thing as the count_char_x function you just wrote - it should return the number of times x appears in word. However, this time, make sure your function works when x is multiple characters long.

    2.  For example, count_multi_char_x("Mississippi", "iss") should return 2

    >   Code    :

        # Write your count_multi_char_x function here:
        def count_multi_char_x(word, x):
          splits = word.split(x)
          return(len(splits)-1)

        # Uncomment these function calls to test your function:
        print(count_multi_char_x("mississippi", "iss"))
        # should print 2
        print(count_multi_char_x("apple", "pp"))
        # should print 1

    >   Result  :

    ![python II - 1 3](https://user-images.githubusercontent.com/74751990/201574099-9777a5bb-9abf-4e9b-818f-2c282166b801.jpg)

4.  Substring Between

    Here is a challenging problem. We need a function that is able to extract a portion of a string between two characters. The function will take three parameters where the first parameter is the string we are going to extract the substring from, the second input is the starting character of our substring and the third character is the ending character of our substring. Here are the steps we can use:

        a.  Define the function to accept three parameters, one string and two characters
        b.  find the starting index of our substring using the second input parameter
        c.  find the ending index of our substring using the third input parameter
        d.  If neither of the indices are -1, return the portion of the first input parameter string between the starting and ending indices (not including the starting and ending index)
        e.  If either of the indices are -1, that means the start or end of the substring didn’t exist in our string. Return the original string in this case.

    >   Coding question

    1.  Write a function named substring_between_letters that takes a string named word, a single character named start, and another character named end. This function should return the substring between the first occurrence of start and end in word. If start or end are not in word, the function should return word.

    2.  For example, substring_between_letters("apple", "p", "e") should return "pl".

    >   Code    :

        # Write your substring_between_letters function here:
        def substring_between_letters(word, start, end):
            start_ind = word.find(start)
            end_ind = word.find(end)
            if start_ind > -1 and end_ind > -1:
                return(word[start_ind+1:end_ind])
            return word

        # Uncomment these function calls to test your function:
        print(substring_between_letters("apple", "p", "e"))
        # should print "pl"
        print(substring_between_letters("apple", "p", "c"))
        # should print "apple"

    >   Result  :

    ![python II - 1 4](https://user-images.githubusercontent.com/74751990/201964602-9a871a50-f4cd-4280-95bb-b400a11f78ac.jpg)

5.  X Length

    Let’s use the split method in a different way. We need a new function that is able to accept two inputs: one for a sentence and another for a number. The function returns True if every single word in the sentence has a length greater than or equal to the number provided. These are the steps:

        a.  Define the function to accept two parameters, one string, and one number
        b.  Split up the sentence into an array of words
        c.  Loop through the words. If the length of any of the words is less than the provided number return False
        d.  If we made it through the loop without returning False then return True

    >   Coding question

        Create a function called x_length_words that takes a string named sentence and an integer named x as parameters. This function should return True if every word in sentence has a length greater than or equal to x.

    >   Code    :



    >   Result  :


