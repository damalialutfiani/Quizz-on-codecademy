Lesson 9 – **Files**

1.	What does the with command do in Python?
-	Opens a file in read-mode.
-	Imports a new module for use by the writer of the code.
-	**Creates a context-manager, which performs cleanup after exiting the adjacent indented block.**

2.	Which of the following methods on a file object (called file_object) reads the contents of a file and returns it as a string?
-	file_contents = file_object.get()
-	file_contents = file_object.readlines()
-	**file_contents = file_object.read()**
-	file_contents = file_object.readline()

3.	What function would you use to render Python data to a JSON file?
-	**json.dump()**
-	json.write()
-	json.writelines()

4.	Which of the following opens a file in Python?
-	with file_obj = open('file.txt'):
pass
-	**with open('file1.txt') as file_obj:
Pass**
-	with open(file.txt) as file_obj:
pass

5.	What different modes, passed as arguments to the open() function, are there for opening a file in Python?
-	Read-mode (‘r’, the default mode), Write-mode (‘w’), and Update-mode (‘u’).
-	**Read-mode (‘r’, the default mode), Write-mode (‘w’), and Append-mode (‘a’).**
-	Read-mode (‘r’, the default mode), Delete-mode (‘d’), and Update-mode (‘u’).
