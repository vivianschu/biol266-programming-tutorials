# Tutorial 2 - Python
Python is a popular programming language used for many purposes ranging from building websites and software development to data analysis and automating tasks. Many people like Python over other programming languages becasue its syntax (language structure) is similar to the English language - after all, it was designed for readability!

## General Information
* Python files (modules) are stored using ".py" (e.g., HelloWorld.py).
* Indentation is used to group code blocks. This refers to the spaces at the beginning of a code line.
* If you're interested in learning more Python, consider enrolling in [CS 116 Introduction to Computer Science 2](https://cs.uwaterloo.ca/current/courses/course_descriptions/cDescr/CS116) at the University of Waterloo.

## Getting Started
### Downloading Python and Text Editor


### Your First Program
When we <i>print</i> text in a program, we're not literally talking about printing a piece of paper from a printer. <i>Print</i> means our computer is outputting some text.

Let's print our first message:
```
print("Hello world")
```
This line is called a <i>statement</i>.

`print` is the name of a <i>function</i>. <i>Functions</i> are codes that are used to accomplish a specific task. They can be blocks of code, or individual statements like `print`.

The text within the round parentheses are called <i>arguments</i>. Depending on the function, there can be one or more arguments. These tell our functions what exactly to do. In this case, our argument is telling our function `print` to output the text `Hello world`.

## Programming Basics

### Comments
<i>Comments</i> are short notes in code that help explain how your program works, or in-code documentation.
In Python, these start with a hash character '#' and continue until the end of the line. 
```
#This is a comment!
```
They can be placed at the end of a function.
```
print("Hello world") #This is a comment
```
Span more than one line
```
#This
#is a
#comment
```
And can prevent Python from executing your function.
```
print("Hello world")
#print("Goodbye world")
```
Comments are useful when you are showing your code to somebody else, but more importantly, they're extremely useful to reminding <b>you</b> how your code works. These can help you understand your own code. Let's write a comment for our first program:
```
# Print a greeting; say hello to the world.
print("Hello world")
```

### Variables
Variables store data - they can be:
* <i>strings</i> (text), defined using double quotations
* numbers (integer, float (number with decimals)

They're also case-sensitive. So, ACGT, acgt, acGT, AcGT are all separate variables.

```
courseName = "Introduction to Computational Biology"
myInteger = 9876
myFloat = 54.321

print(courseName)
print(myInteger)
print(myFloat)
```
The variable courseName is assigned to the string "Introduction to Computational Biology". Now, we can refer to the variable instead of the string itself, and use it in a print statement. Since the quotes are already part of the string in courseName, we don't need to include them because they are part of courseName.

We can also reassign the variable as many times as we need to.
```
courseName = "Introduction to Computational Biology"
print(courseName)
#Update Course Name
courseName = "Methods in Bioinformatics"
print(courseName)

luckyNumber = 7
print(luckyNumber)
#Reaassign number
unluckyNumber = 13
print(unluckyNumber)
```

It might seem like there's a relationship between our variable and its content, but we can name our variable anything we want. 
```
courseName = "Methods in Bioinfornatics"
print(courseName)
#Change variable name
ilovemarshmellows = "Methods in Bioinformatics"
print(ilovemarshmellows)

luckyNumber = 7
print(luckyNumber)
# Change variable name
unluckyNumber = 7
print(unluckyNumber)
```

### Lists
Lists are used to store multiple items (strings, numbers, etc.) in a single variable. Lists are one of Python's four built-in data types. The others are Tuple, Set and Dictionary, but we won't dive too deep into those in this tutorial. 

Square brackets define lists.
```
# Example of an empty list
emptyBasket = []
print(emptyBasket)

# Example of a list with items
myDNA = ["A", "C", "T", "G"]
print(myDNA)
```
We can access different items in the list by specifying its `index`. <b>The first index of a list in Python is 0</b>,not 1. For instance, in a list of 4 items, we have the indeces 0, 1, 2, 3.
```
myDNA = ["A", "C", "T", "G"]
```

### Operations

# Resources
* [W3Schools Python Tutorial](https://www.w3schools.com/python/default.asp)
