Lesson 9 – **Python Files**

1.	What does the with command do in Python?

    a.  Opens a file in read-mode.

    b.  Imports a new module for use by the writer of the code.

    c.  **Creates a context-manager, which performs cleanup after exiting the adjacent indented block.**

2.	Which of the following methods on a file object (called file_object) reads the contents of a file and returns it as a string?

    a.	file_contents = file_object.get()

    b.  file_contents = file_object.readlines()

    c.  **file_contents = file_object.read()**

    d.  file_contents = file_object.readline()

3.	What function would you use to render Python data to a JSON file?

    a.	**json.dump()**

    b.  json.write()

    c.	json.writelines()

4.	Which of the following opens a file in Python?

    a.
        
        with file_obj = open('file.txt'):
        pass

    b.  
    
    **with open('file1.txt') as file_obj:**
        
    **Pass**

    c.	
    
        with open(file.txt) as file_obj:
        pass

5.	What different modes, passed as arguments to the open() function, are there for opening a file in Python?

    a.  Read-mode (‘r’, the default mode), Write-mode (‘w’), and Update-mode (‘u’).

    b.	**Read-mode (‘r’, the default mode), Write-mode (‘w’), and Append-mode (‘a’).**

    c.	Read-mode (‘r’, the default mode), Delete-mode (‘d’), and Update-mode (‘u’).
