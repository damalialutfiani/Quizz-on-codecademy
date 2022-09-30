**Python Code Challenges I - Loops**

1. Divisible By Ten

    Let’s start our code challenges with a function that counts how many numbers are divisible by ten from a list of numbers. This function will accept a list of numbers as an input parameter and use a loop to check each of the numbers in the list. Every time a number is divisible by 10, a counter will be incremented and the final count will be returned. These are the steps we need to complete this:

        a.  Define the function to accept one input parameter called nums

        b.  Initialize a counter to 0

        c.  Loop through every number in nums

        d.  Within the loop, if any of the numbers are divisible by 10, increment our counter

        e.  Return the final counter value

    >   Coding question

    1.  Create a function named divisible_by_ten() that takes a list of numbers named nums as a parameter.

    2.  Return the count of how many numbers in the list are divisible by 10.

    >   Code :

        #Write your function here

        def divisible_by_ten(nums):

            count = 0

            for number in nums:

                if (number % 10 == 0):

                    count += 1

            return count

        #Uncomment the line below when your function is done

        print(divisible_by_ten([20, 25, 30, 35, 40]))

    >   Result  :

      ![python I - 5 1](https://user-images.githubusercontent.com/74751990/192553691-31638ae1-9d76-4154-94ff-aa9ac9c9ab1e.jpg)

2. Greetings

    You are invited to a social gathering, but you are tired of greeting everyone there. Luckily we can create a function to accomplish this task for us. In this challenge, we will take a list of names and prepend the string 'Hello, ' before each name. This will require a few steps:

        a.  Define the function to accept a list of strings as a single parameter called names

        b.  Create a new list of strings

        c.  Loop through each name in names

        d.  Within the loop, concatenate 'Hello, ' and the current name together and append this new string to the new list of strings

        e.  Afterwards, return the new list of strings

    >   Coding question

    1.  Create a function named add_greetings() which takes a list of strings named names as a parameter.

    2.  In the function, create an empty list that will contain each greeting. Add the string 'Hello, ' in front of each name in names and append the greeting to the list.

    3.  Return the new list containing the greetings.

    >   Code :

        #Write your function here
    
        def add_greetings(names):
    
            new_list = []
    
            for name in names:
        
                new_list.append("Hello, " + name)
    
            return new_list

        #Uncomment the line below when your function is done
    
        print(add_greetings(["Owen", "Max", "Sophie"]))

    >   Result  :

      ![python I - 5 2](https://user-images.githubusercontent.com/74751990/192597088-df91bfab-a9ea-4947-9043-2f2cc29c70c6.jpg)

3. Delete Starting Even Numbers

    Let’s try a tricky challenge involving removing elements from a list. This function will repeatedly remove the first element of a list until it finds an odd number or runs out of elements. It will accept a list of numbers as an input parameter and return the modified list where any even numbers at the beginning of the list are removed. To do this, we will need the following steps:

        a.  Define our function to accept a single input parameter lst which is a list of numbers

        b.  Loop through every number in the list if there are still numbers in the list and if we haven’t hit an odd number yet

        c.  Within the loop, if the first number in the list is even, then remove the first number of the list

        d.  Once we hit an odd number or we run out of numbers, return the modified list

    >   Coding question

    1.  Write a function called delete_starting_evens() that has a parameter named lst.

    2.  The function should remove elements from the front of lst until the front of the list is not even. The function should then return lst.

    3.  For example if lst started as [4, 8, 10, 11, 12, 15], then delete_starting_evens(lst) should return [11, 12, 15].

    4.  Make sure your function works even if every element in the list is even!

    >   Code :

        #Write your function here

        def delete_starting_evens(lst):

            while (len(lst) > 0 and lst[0] % 2 == 0):

                lst = lst[1:]

            return lst

        #Uncomment the lines below when your function is done

        print(delete_starting_evens([4, 8, 10, 11, 12, 15]))

        print(delete_starting_evens([4, 8, 10]))

    >   Result  :

      ![python I - 5 3](https://user-images.githubusercontent.com/74751990/192845855-94a65473-a5e8-421b-be57-fe8b0b333fff.jpg)

4. Odd Indices

    This next function will give us the values from a list at every odd index. We will need to accept a list of numbers as an input parameter and loop through the odd indices instead of the elements. Here are the steps needed:

        a.  Define the function header to accept one input which will be our list of numbers

        b.  Create a new list which will hold our values to return

        c.  Iterate through every odd index until the end of the list

        d.  Within the loop, get the element at the current odd index and append it to our new list

        e.  Return the list of elements which we got from the odd indices.

    >   Coding question

    1.  Create a function named odd_indices() that has one parameter named lst.

    2.  The function should create a new empty list and add every element from lst that has an odd index. The function should then return this new list.

    3.  For example, odd_indices([4, 3, 7, 10, 11, -2]) should return the list [3, 10, -2].

    >   Code :

        #Write your function here

        def odd_indices(lst):
  
            new_list = []
  
            for index in range(1, len(lst), 2):
 
                new_list.append(lst[index])

            return new_list

        #Uncomment the line below when your function is done

        print(odd_indices([4, 3, 7, 10, 11, -2]))

    >   Result  :

      ![python I - 5 4](https://user-images.githubusercontent.com/74751990/192846813-e21a57dd-3133-451f-975b-c7e676f14383.jpg)

5. Exponents

    In this challenge, we will be using nested loops in order to raise a list of numbers to the power of a list of other numbers. What this means is that for every number in the first list, we will raise that number to the power of every number in the second list. If you provide the first list with 2 elements and the second list with 3 numbers, then there will be 6 final answers. Let’s look at the steps we need:

        a.  Define the function to accept two lists of numbers, bases and powers

        b.  Create a new list that will contain our answers

        c.  Create a loop that iterates through every base in bases

        d.  Within that loop, create another loop that iterates through every power in power

        e.  Within that nested loop, append the result of the current base raised to the current power.

        f.  After all iterations of both loops are complete, return the list of answers

    >   Coding question

    1.  Create a function named exponents() that takes two lists as parameters named bases and powers. Return a new list containing every number in bases raised to every number in powers.

    2.  For example, consider the following code.

        exponents([2, 3, 4], [1, 2, 3])

        the result would be the list [2, 4, 8, 3, 9, 27, 4, 16, 64]. It would first add two to the first. Then two to the second. Then two to the third, and so on.

    >   Code :

        #Write your function here

        def  exponents(bases, powers):

            new_list = []

            for base in bases:

                for power in powers:

                    new_list.append(base ** power)

            return new_list

        #Uncomment the line below when your function is done

        print(exponents([2, 3, 4], [1, 2, 3]))

    >   Result  :

      ![python I - 5 5](https://user-images.githubusercontent.com/74751990/193165345-0cebe45c-bee9-423b-bdab-f24311012c7a.jpg)
