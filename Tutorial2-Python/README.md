# Tutorial 2 - Python
Python is a popular programming language used for many purposes ranging from building websites and software development to data analysis and automating tasks. Many people like Python over other programming languages becasue its syntax (language structure) is similar to the English language - after all, it was designed for readability!

## General Information
* Python files (modules) are stored using ".py" (e.g., HelloWorld.py).
* Indentation is used to group code blocks. This refers to the spaces at the beginning of a code line. Standard indents are 4 spaces.
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
<i>Variables</i> store data to be referenced and can be changed using a computer program.

They can be:
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
We can access different items in the list by specifying its `index` using square brackets. <b>The first index of a list in Python is 0</b>,not 1. For instance, in a list of 4 items, we have the indices 0, 1, 2, 3. You can also use negative indices to access items with respect to the right-end of the list.
```
myDNA = ["A", "C", "T", "G"]

# Access adenine from myDNA
print(myDNA[0])

# Assign adenine its own variable
adenine = myDNA[0]
print(adenine)
```

### Operations
Operations are special symbols that carry out arithmetic or logical computation, like adding, subtracting, dividing, multipling, comparing numbers and more.
```
myInteger = 9876
myFloat = 54.321

# Add myInteger and myFloat
mySum = myInteger + myFoloat
print(mySum)
```

Other operations are included below:
```
x = 42
y = 241

# Addition
z = x + y
print(z)

# Subtraction
z = x - y
print(z)

# Multiplication
z = x * y
print(z)

# Division
z = x / y
print(z)

# Exponents
z = x ** y
print(z)
```

We can also use operations on strings.
```
# Concatenate Sentence
courseCode = "BIOL 266"
courseName = "Introduction to Computational Biology"

course = "Welcome to " + courseCode + " " + courseName
# notice we included two quotation marks with an empty space - this is a string!
print(course)

# Repeat Strings
minion = banana * 100
print(minion)

# Slice a string (substrings)
print(course[0:6])                      # should output "Welcome"

# Compute the length of the string
len(course)
print(len(course))

# Identify the index of a character
i = course.index("B")                   # should return 11, since the first occurence of 'B' is at index 11

# Counting the number of 'B' characters in the string
i = course.index("B")
print(i)                                # should return 2
```

### Conditional Statements (If/Else)
<i>If statements</i> or <i>conditions</i> are commonly used to evaluate if conditions are true or false given a set of rules using `if`.

Logical conditions include:
* equals: `a == b`
* not equals: `a != b`
* greater than: `a > b`
* less than: `a < b`
* greater than or equal to `a >= b`
* less than or equal to `a <= b`
* `and`
* `or`
* `not`

```
DNAsequence1 = "ATAGCGCATCGATCAGCTATGCGA"
DNAsequence2 = "ATGATCGACCGCTATAGCTAGCTA"

if DNAsequence1 == DNAsequence2:
    print ("The two DNA sequences are identical")
else:
    print ("The DNA sequences are different")
```
Python relies on indentation (standard indentation is 4 spaces) at the beginning of a line to specify a code block.
The `else` function directs the code to another result if the preceding conditions aren't met.

We can also put an if statement in an if statement. This is refered to as a <i>nested</i> if statement.
```
DNAsequence1 = "ATAGCGCATCGATCAGCTATGCGA"
DNAsequence2 = "ATGATCGACCGCTATAGCTAGCTA"

if DNAsequence1 == DNAsequence2:
    print ("The two DNA sequences are identical")
else:
    print ("The DNA sequences are different")
    if len(DNAsequence1) == len(DNAsequence2):
        print ("but they have the same length")
    else:
        print ("and they are different in length")
```
In this example, we first compare if DNAsequence1 is equal to DNAsequence2. If they are identical, we print a sentence stating that they are identical. If they're not identical, we move to the `else` portion of the statement and print a sentence stating that the sequences are different. We also move to the next `if` block which compares the string lengths of our DNA seuqeqnces. If they are identical, we print a sentence stating that they have the same length. If they are not identical lengths, we print a statement stating that our sequences are different in length.

The `in` operator is also useful to see if a variable mathes an element of a list.
```
DNAsequence1 = "ATAGCGCATCGATCAGCTATGCGA"

if DNAsequence1[1] in ["A","C","G","T"]:
    print ("The first character is a nucleotide")
else:
    print ("The first character is not a nucleotide")
```

### For and while Loops
To repeat code, you can use `for` and `while` loops
```
nucleotides = ["A", "C", "G", "T"]
for nucleotide in nucleotides:
    print (nucleotide)

#or a numeric example

for i in range(1,10):
    print (i)
```


# Resources
* [W3Schools Python Tutorial](https://www.w3schools.com/python/default.asp)
* [Codecademy](https://www.codecademy.com/catalog)
* [LearnPython.org](https://www.learnpython.org/)
* [Python for Biologists](http://userpages.fu-berlin.de/digga/p4b.pdf)
