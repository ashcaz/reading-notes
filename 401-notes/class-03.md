# Reading/Writing Files and Exceptions

**LINKS**

- [Read & Write Files in Python](https://realpython.com/read-write-files-python/)
- [Exceptions in Python](https://realpython.com/python-exceptions/)
- [Video:Read & Write Files in Python - Companion Video](https://realpython.com/courses/reading-and-writing-files-python/)
- [Reading and Writing Files in Python Quiz](https://realpython.com/quizzes/read-write-files-python/)

Link Information I added in:

- [Big O Notation and Algorithm Analysis with Python Examples](https://stackabuse.com/big-o-notation-and-algorithm-analysis-with-python-examples/)
- [Big O Cheatsheet](https://www.bigocheatsheet.com/)

## Reading and Writing Files in Python (Guide)


### What is a file?

A file is a contiguous set of bytes used to store data. This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable. In the end, these byte files are then translated into binary 1 and 0 for easier processing by the computer.

Files are made up of three main parts:

1. **Header**: metadata about the contents of the file (file name, size, type, and so on)
2. **Data**:contents of the file as written by the creator or editor
3. **End of file (EOF)**:special character that indicates the end of the file

### File Paths

When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:

1. **Folder Path**: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
2. **File Name**: the actual name of the file
3. **Extension**: the end of the file path pre-pended with a period (.) used to indicate the file type

### Opening and Closing a File in Python

When you want to work with a file, the first thing to do is to open it. This is done by invoking the open() built-in function. open() has a single required argument that is the path to the file. open() has a single return, the file object:

```Python
file1 = open('dog_breeds.txt')

reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```
The with statement automatically takes care of closing the file once it leaves the with block, even in cases of error.

```Python
with open('dog_breeds.txt') as reader:
    # Further file processing goes here
```

This argument is a string that contains multiple characters to represent how you want to open the file. The default and most common is 'r', which represents opening the file in read-only mode as a text file:

```Python
with open('dog_breeds.txt', 'r') as reader:
    # Further file processing goes here
```
- 'r'	Open for reading (default)
- 'w'	Open for writing, truncating (overwriting) the file first
- 'rb' or 'wb'	Open in binary mode (read/write using byte data)

### Iterating Over Each Line in the File

Python .readline() method to perform that iteration:

```Python
>>> with open('dog_breeds.txt', 'r') as reader:
>>>     # Read and print the entire file line by line
>>>     line = reader.readline()
>>>     while line != '':  # The EOF char is an empty string
>>>         print(line, end='')
>>>         line = reader.readline()
Pug
Jack Russell Terrier
English Springer Spaniel
German Shepherd
Staffordshire Bull Terrier
Cavalier King Charles Spaniel
Golden Retriever
West Highland White Terrier
Boxer
Border Terrier
```
Another way you could iterate over each line in the file is to use the Python .readlines() method. Remember, .readlines() returns a list where each element in the list represents a line in the file:

```Python
>>> with open('dog_breeds.txt', 'r') as reader:
>>>     for line in reader.readlines():
>>>         print(line, end='')
```
## Python Exceptions: An Introduction

A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception.

### Exceptions versus Syntax Errors

An Exception error occurs whenever syntactically correct Python code results in an error.

Instead of showing the message exception error, Python details what type of exception error was encountered.

### Raising an Exception

```Python
x = 10
if x > 5:
    raise Exception('x should not exceed 5. The value of x was: {}'.format(x))
```

### The try and except Block: Handling Exceptions

The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

[Back to Homepage](https://ashcaz.github.io/reading-notes)

