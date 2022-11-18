**Python Code Challenges II - Strings (Advanced)**

1.  Check Name

    You are creating an app that allows users to interact and share their coding project ideas online. The first step is to provide your name in the application and a greeting for other people to see which contains your name. Let’s create a function that is able to check if a user’s name is located within their greeting. We need a function that accepts two parameters, a string for our sentence and a string for a name. The function should return True if the name exists within the string (ignoring any differences in capitalization). Here is what we need to do:

        a.  Define the function to accept two parameters, one string for the sentence and one string for the name
        b.  Convert all of the strings to the same case so we don’t have to worry about differences in capitalization
        c.  Check if the name is within the sentence. If so, then return True. Otherwise, return False

    >   Coding question

    1.  Write a function called check_for_name that takes two strings as parameters named sentence and name. The function should return True if name appears in sentence in all lowercase letters, all uppercase letters, or with any mix of uppercase and lowercase letters. The function should return False otherwise.

    2.  For example, the following three calls should all return True:
      
            check_for_name("My name is Jamie", "Jamie")
            check_for_name("My name is jamie", "Jamie")
            check_for_name("My name is JAMIE", "Jamie")

    >   Code    :

        # Write your check_for_name function here:
        def check_for_name(sentence, name):
          return name.lower() in sentence.lower()

        # Uncomment these function calls to test your  function:
        print(check_for_name("My name is Jamie", "Jamie"))
        # should print True
        print(check_for_name("My name is jamie", "Jamie"))
        # should print True
        print(check_for_name("My name is Samantha", "Jamie"))
        # should print False

    >   Result  :

    ![python II - 2 1](https://user-images.githubusercontent.com/74751990/202047790-a267fe21-2e0c-4b98-959e-a74a80110647.jpg)

2.  Every Other Letter

    For this next function, we are going to create a function that extract every other letter from a string and returns the resulting string. There are a few different ways you can solve this problem Here are the steps needed for one of the ways:

        a.  Define the function to accept one parameter for the string
        b.  Create a new empty string to hold every other letter from the input string
        c.  Loop through the input string while incrementing by two every time
        d.  Inside the loop, append the character at the current location to the new string we initialized earlier
        e.  Return the new string

    >   Coding question

        Create a function named every_other_letter that takes a string named word as a parameter. The function should return a string containing every other letter in word.

    >   Code    :

        # Write your every_other_letter function here:
        def every_other_letter(word):
          every_other = ""
          for i in range(0, len(word), 2):
            every_other += word[i]
          return every_other

        # Uncomment these function calls to test your function:
        print(every_other_letter("Codecademy"))
        # should print Cdcdm
        print(every_other_letter("Hello world!"))
        # should print Hlowrd
        print(every_other_letter(""))
        # should print 

    >   Result  :
    
    ![python II - 2 2](https://user-images.githubusercontent.com/74751990/202048434-b2f338e9-b764-469b-a24b-eae694e67d90.jpg)

3.  Reverse

    This one is similar to the last challenge. Instead of selecting every other letter, we want to reverse the entire string. This can be performed in a similar manner, but we will need to modify the range we are using. Here is what we need to do:

        a.  Define the function to accept one parameter for the string
        b.  Create a new empty string to hold the reversed string
        c.  Loop through the input string by starting at the end, and working towards the beginning
        d.  Inside the loop, append the character at the current location to the new string we initialized earlier
        e.  Return the result

    >   Coding question

        Write a function named reverse_string that has a string named word as a parameter. The function should return word in reverse.

    >   Code    :

        # Write your reverse_string function here:
        def reverse_string(word):
          reverse = ""
          for i in range(len(word)-1, -1, -1):
            reverse += word[i]
          return reverse

        # Uncomment these function calls to test your  function:
        print(reverse_string("Codecademy"))
        # should print ymedacedoC
        print(reverse_string("Hello world!"))
        # should print !dlrow olleH
        print(reverse_string(""))
        # should print

    >   Result  :

    ![python II - 2 3](https://user-images.githubusercontent.com/74751990/202478617-e971d98f-9c34-4b95-9c27-ba51d03a313f.jpg)

4.  Make Spoonerism

    A Spoonerism is an error in speech when the first syllables of two words are switched. For example, a Spoonerism is made when someone says “Belly Jeans” instead of “Jelly Beans”. We are going to make a function that is similar, but instead of using the first syllable, we are going to switch the first character of two words. Here is what we need to do:

        a.  Define the function to accept two parameters for our two words
        b.  Get the first character of the first word and the first character of the second word
        c.  Get the remaining characters of the first word and the remaining characters of the second word.
        d.  Append the first character of the second word to the remaining character of the first word
        e.  Append a space character
        f.  Append the first character of the first word to the remaining characters of the second word.
        g.  Return the result

    >   Coding question

        Write a function called make_spoonerism that takes two strings as parameters named word1 and word2. Finding the first syllable of a word is a difficult task, so for our function, we’re going to switch the first letters of each word. Return the two new words as a single string separated by a space.

    >   Code    :

        # Write your make_spoonerism function here:
        def make_spoonerism(word1, word2):
          return word2[0]+word1[1:]+" "+word1[0]+word2[1:]

        # Uncomment these function calls to test your function:
        print(make_spoonerism("Codecademy", "Learn"))
        # should print Lodecademy Cearn
        print(make_spoonerism("Hello", "world!"))
        # should print wello Horld!
        print(make_spoonerism("a", "b"))
        # should print b a

    >   Result  :

    ![python II - 2 4](https://user-images.githubusercontent.com/74751990/202726660-80622bab-6024-4cf5-a0ff-968e9707774c.jpg)


