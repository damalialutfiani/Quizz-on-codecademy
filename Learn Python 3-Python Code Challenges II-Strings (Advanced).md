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



