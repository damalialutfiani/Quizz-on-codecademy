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




