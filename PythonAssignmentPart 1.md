## Assignment Part-1
## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?
Ans: Python is called a general-purpose and high-level programming language for several reasons:

General-purpose: Python is a versatile language that can be used for a wide range of applications. It can be used for web development, scientific computing, data analysis, artificial intelligence, machine learning, and more. Python has a vast library of modules and packages, which makes it easy to develop different types of applications.

High-level: Python is a high-level language, which means that it is designed to be easy to read and write. It has a simple and clean syntax that allows developers to express concepts in fewer lines of code than other languages. Python also takes care of many low-level tasks, such as memory management, which makes it easier for developers to focus on solving problems rather than worrying about the details of how the code works.

Easy to learn: Python is an easy language to learn for beginners. It has a clear and concise syntax, and its code is easy to read and understand. The Python community is also very active, which means that there are plenty of resources and support available for new developers.

Cross-platform: Python can be used on different operating systems, including Windows, Linux, and macOS. This means that developers can write code once and run it on different platforms without having to worry about compatibility issues.

Interpreted: Python is an interpreted language, which means that the code is executed line by line, rather than being compiled before execution. This makes it easier to debug and test code, as changes can be made quickly and easily.

Overall, these features make Python a versatile and powerful language that can be used for a wide range of applications, from web development to scientific computing and machine learning.

Q2. Why is Python called a dynamically typed language?

Ans: Python is called a dynamically typed language because the type of a variable is determined at runtime rather than during compilation. In other words, the type of a variable can change dynamically based on the value assigned to it at runtime.

In a dynamically typed language like Python, the programmer does not need to declare the data type of a variable explicitly. Instead, Python automatically determines the type of a variable based on the value assigned to it. For example, if we assign an integer value to a variable, Python will automatically assign the type "int" to that variable. If we then assign a string value to the same variable, Python will automatically assign the type "string" to that variable.

This dynamic type checking allows for more flexibility in programming and makes it easier to write code quickly. However, it can also lead to errors if the programmer is not careful. For example, if we try to perform a mathematical operation on a string variable, Python will raise a type error because the two types are incompatible.

In summary, Python is called a dynamically typed language because its variables can change types dynamically at runtime, based on the values assigned to them.

Q3. List some pros and cons of Python programming language?

Ans: Pros:

Easy to learn and read: Python has a simple and easy-to-read syntax that makes it a great language for beginners to learn. The code is easy to understand, which makes it easy to maintain and update.

Large standard library: Python has a large standard library that includes modules for a wide range of tasks, such as web development, data analysis, and scientific computing. This makes it easier for developers to write code quickly and efficiently.

Cross-platform compatibility: Python code can run on different operating systems, including Windows, Linux, and macOS. This makes it easier to write code once and run it on different platforms without worrying about compatibility issues.

Interpreted language: Python is an interpreted language, which means that code is executed line by line. This makes it easier to test and debug code.

Community support: Python has a large and active community of developers who contribute to the language and create modules and packages for various applications. This community support makes it easier to find resources and help when needed.

Cons:

Slow performance: Python is an interpreted language, which can make it slower than compiled languages like C and C++. While Python has made improvements to its performance with just-in-time (JIT) compilation and other optimizations, it may not be suitable for applications that require high-performance computing.

Weak in mobile computing: Python has limited support for mobile computing, which means that it may not be the best choice for developing mobile applications.

Memory consumption: Python is not the most memory-efficient language, which can be a problem for applications that require a lot of memory.

Global Interpreter Lock (GIL): Python has a Global Interpreter Lock (GIL), which can limit the ability to run multiple threads in parallel. This can be a bottleneck for certain applications that require high-performance computing.

Design restrictions: Python's design philosophy is focused on readability and simplicity, which can limit the ability to write highly optimized code. This can be a disadvantage for applications that require high-performance computing or low-level access to hardware.

Overall, Python is a versatile and powerful language that is easy to learn and use. However, it may not be the best choice for all applications, and developers should consider the pros and cons before deciding to use Python for their project.

Q4. In what all domains can we use Python?

Ans: Python is a versatile language that can be used in a wide range of domains. Here are some examples:

Web Development: Python can be used to develop web applications and APIs using frameworks like Django, Flask, Pyramid, and more.

Data Science and Analytics: Python is widely used for data analysis, data visualization, and machine learning. Libraries like NumPy, Pandas, Matplotlib, and Scikit-learn make it easy to work with large datasets and perform complex analyses.

Scientific Computing: Python is used extensively in scientific computing and engineering applications. Libraries like SciPy, SymPy, and OpenCV provide tools for scientific computing, numerical analysis, and image processing.

Game Development: Python can be used to develop games using libraries like Pygame and PyOpenGL.

Desktop Applications: Python can be used to create desktop applications using frameworks like PyQt and wxPython.

Network Programming: Python provides support for network programming, making it a good choice for developing network-based applications.

DevOps and Automation: Python can be used for automation and scripting tasks, making it popular in the DevOps field.

Artificial Intelligence and Machine Learning: Python's simplicity, ease of use, and extensive libraries have made it a popular choice for artificial intelligence and machine learning applications.

Overall, Python's versatility and ease of use make it a popular choice in many domains, from web development to scientific computing, automation to AI and machine learning.



Q5. What are variable and how can we declare them?

A variable in programming is a named memory location that stores a value or data. In Python, we can declare a variable by assigning a value to a variable name. For example: p=10

In this example, we have declared a variable named "p" and assigned it the value 10. Python automatically determines the data type of the variable based on the value assigned to it. In this case, "p" is an integer.

We can also declare multiple variables in a single line using comma-separated values:

x, y, z = 5, 10, 15
In this example, we have declared three variables named "x", "y", and "z" and assigned them the values 5, 10, and 15 respectively.

Python supports multiple data types for variables, including integers, floating-point numbers, strings, boolean values, and more. We can also change the value of a variable by reassigning it to a new value:

x = 5
x = "Hello, world!"

In this example, we have initially declared "x" as an integer with the value 5. We then reassign "x" to a string value "Hello, world!".

When declaring variables, it's important to follow Python's naming conventions. Variable names should start with a letter or underscore, and should not start with a number. Variable names can contain letters, numbers, and underscores, but cannot contain spaces or special characters.

In summary, variables in Python are named memory locations that store data. We can declare variables by assigning a value to a variable name, and Python automatically determines the data type of the variable.

Q6. How can we take an input from the user in Python?

Ans: We can take input from the user in Python using the input() function. The input() function waits for the user to type something and press enter, and then returns the input as a string.

For example:
name = input("What is your name? ")
print("Hello, " + name + "!")

In this example, we use the input() function to ask the user for their name. The text "What is your name?" is displayed as a prompt to the user. The input from the user is stored in the variable name. We then use the print() function to display a greeting message to the user, using the value of the name variable.

We can also convert the input to a different data type, such as an integer or a float, using the appropriate type casting function. 

For example: 
age = int(input("What is your age? "))
print("You will be " + str(age + 1) + " next year.")

In this example, we use the int() function to convert the input from the user to an integer. We then perform some calculations on the input value and use the str() function to convert the result back to a string for display.

It's important to note that the input() function returns a string, so we need to use type casting functions to convert the input to the desired data type before performing any operations or calculations on it.





Q7. What is the default datatype of the value that has been taken as an input using input() function?

Ans: The input() function in Python always returns a string, regardless of the type of value that the user enters. This means that if the user enters a number, the input() function will return a string representation of that number, not an actual number data type like integer or float.

For example, consider the following code:

x = input("Enter a number: ")
print(type(x))

If the user enters the number 42 as input, the output of this code will be:

<class 'str'>

This shows that the input() function returns a string, even if the user enters a number.

To perform numerical operations on the input value, we need to convert it to a numeric data type using type casting functions like int() or float(). 

For example: 
x = input("Enter a number: ")
y = int(x)
z = y * 2
print(z)

In this example, we convert the input value x to an integer using the int() function and store it in the variable y. We then perform a calculation on y and store the result in z. This code will correctly output the result of multiplying the user's input value by 2.


Q8. What is type casting?

Type casting is the process of converting a value from one data type to another data type. In Python, we can use built-in functions like int(), float(), str(), bool(), and others to cast a value to a different data type.

For example, we can cast a string value to an integer using the int() function:

x = "42"
y = int(x)
print(y)

In this example, we cast the string value "42" to an integer using the int() function and store the result in the variable y. The output of this code will be the integer value 42.

We can also cast a numeric value to a string using the str() function:

x = 42
y = str(x)
print(y)

In this example, we cast the integer value 42 to a string using the str() function and store the result in the variable y. The output of this code will be the string value "42".

Type casting is useful when we need to perform operations or comparisons on values of different data types. For example, if we have a string value that represents a number, we can cast it to an integer or float before performing mathematical operations on it. Or if we have a numeric value that we want to display as part of a message, we can cast it to a string before concatenating it with other strings.

It's important to note that not all data types can be cast to each other, and some casts may result in loss of information or unexpected behavior. Care should be taken when performing type casting to ensure that the resulting value is correct and suitable for the intended use.

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

ANs: Yes, we can take multiple inputs from the user using a single input() function in Python. To do this, we can separate the inputs with commas and then use the split() function to split the input string into separate values.

For example:
name, age = input("Enter your name and age, separated by a comma: ").split(",")
print("Hello, " + name + "! You are " + age + " years old.")

In this example, we use the input() function to prompt the user to enter their name and age, separated by a comma. We then use the split() function to split the input string into two separate values, which we assign to the variables name and age. We then use these variables to display a personalized message to the user.

Note that when using this method, we need to make sure that the user enters the inputs in the correct format (in this case, separated by a comma), otherwise the split() function may not work as expected and we may encounter errors.

Alternatively, we can take multiple inputs from the user using separate input() statements for each value:

name = input("Enter your name: ")
age = input("Enter your age: ")
print("Hello, " + name + "! You are " + age + " years old.")

This method is more straightforward and may be easier to use in cases where we don't need to prompt the user to enter multiple values in a specific format.


Q10. What are keywords?

Ans: In Python, keywords are reserved words that have a specific meaning and purpose within the language. These words are used to define the syntax and structure of the code, and they cannot be used as variable names or other identifiers.

Examples of Python keywords include if, else, while, for, in, def, return, class, try, except, finally, True, False, None, and and, among others.

Here are some important features of Python keywords:

Keywords are case-sensitive and must be written in lowercase letters.
Since keywords have predefined meanings in the language, we cannot use them as variable names, function names, or any other identifiers in our code.
Using keywords in an unintended way may cause syntax errors or unexpected behavior in the code.
We can use the keyword module in Python to get a list of all keywords in the language.
For example, we can use the keyword module to print a list of all Python keywords:

import keyword

print(keyword.kwlist)

This code will output a list of all Python keywords:

['False', 'None', 'True', 'and', 'as', 'assert', 'async', 'await', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']



Q11. Can we use keywords as a variable? Support your answer with reason.

Ans: No, we cannot use keywords as variable names in Python. Keywords are reserved words that have a specific meaning and purpose within the language, and they cannot be used as variable names or other identifiers.

If we try to use a keyword as a variable name, Python will raise a SyntaxError and report that the keyword is an invalid syntax. For example, if we try to define a variable with the name if, we will get an error like this:

>>> if = 10
  File "<stdin>", line 1
    if = 10
       ^
SyntaxError: invalid syntax

To avoid this error, we should choose a different name for our variable that does not conflict with any Python keywords.


Q12. What is indentation? What's the use of indentaion in Python?

Ans: In Python, indentation refers to the number of spaces or tabs used at the beginning of a line of code to indicate its level of nesting within a block of code. Indentation is used to define the structure and organization of the code, and it is a key feature of Python's syntax.

The use of indentation in Python is important because it replaces the use of curly braces or other block delimiters that are used in other programming languages to define the structure of the code. Instead, Python uses whitespace to delimit code blocks, which makes the code more readable and easier to understand.

For example, consider the following code that uses indentation to define a for loop that iterates over a list of numbers and prints each number:

numbers = [1, 2, 3, 4, 5]

for num in numbers:
    if num % 2 == 0:
        print(num, "is even")
    else:
        print(num, "is odd")

In this code, the for loop and the conditional statements (if and else) are defined by the level of indentation used for each line of code. The lines of code that are indented under the for loop are executed once for each item in the numbers list, while the lines of code that are indented under the if and else statements are executed conditionally based on the value of each number.

Using indentation in this way makes the code more readable and easier to understand, since the structure of the code is more clearly defined and organized.



Q13. How can we throw some output in Python?

Ans: In Python, we can use the print() function to display output on the console or command line. The print() function can take one or more arguments, separated by commas, and it will display the values of those arguments on the console. Here's an example:

print("Hello, world!")

This code will display the string "Hello, world!" on the console.

We can also use the format() method to format the output of the print() function. The format() method allows us to insert variables or values into a string and format them in a specific way. Here's an example:

name = "Alice"
age = 30

print("My name is {} and I am {} years old.".format(name, age))

This code will display the string "My name is Alice and I am 30 years old." on the console, with the values of the name and age variables inserted into the string using the {} placeholders.

Additionally, we can also use formatted string literals, or f-strings, to insert variables or values directly into a string. Here's an example:

name = "Bob"
age = 25

print(f"My name is {name} and I am {age} years old.")

This code will display the same string "My name is Bob and I am 25 years old." on the console, using an f-string to insert the values of the name and age variables into the string.


Q14. What are operators in Python?

Ans:  In Python, operators are special symbols or keywords that are used to perform operations on values or variables. There are several types of operators in Python, including:

Arithmetic operators: used to perform mathematical operations, such as addition (+), subtraction (-), multiplication (*), division (/), and modulus (%).

Assignment operators: used to assign a value to a variable, such as = or +=.

Comparison operators: used to compare two values or variables, such as == (equality), != (inequality), > (greater than), < (less than), >= (greater than or equal to), and <= (less than or equal to).

Logical operators: used to perform logical operations on boolean values or expressions, such as and, or, and not.

Identity operators: used to compare the identity of two objects, such as is (returns True if two objects are the same) and is not (returns True if two objects are not the same).

Membership operators: used to test if a value or variable is a member of a sequence, such as in (returns True if a value is in a sequence) and not in (returns True if a value is not in a sequence).

Bitwise operators: used to perform bitwise operations on binary values, such as & (bitwise AND), | (bitwise OR), ^ (bitwise XOR), << (left shift), and >> (right shift).

These operators are used extensively in Python to perform various operations on values and variables, and they are an essential part of the language.

Q15. What is difference between / and // operators?

In Python, the / operator performs floating-point division, while the // operator performs integer division (also known as floor division).

When the / operator is used to divide two numbers, it returns a floating-point result, even if the result is a whole number. For example:

>>> 5 / 2
2.5

In contrast, the // operator performs integer division, which returns the largest integer that is less than or equal to the result of the division. For example:

>>> 5 // 2
2

Note that if both the dividend and divisor are integers, then the result of the // operator will also be an integer. If either the dividend or divisor is a float, then the result will be a float.

Additionally, when using negative numbers with the // operator, the result is rounded towards negative infinity, rather than towards zero. For example:

>>> -5 // 2
-3

This is because the // operator returns the largest integer that is less than or equal to the result of the division, and in this case, the largest integer that is less than or equal to -2.5 is -3.


Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```
Sol:  Code: print("iNeuron" * 4 + "Neuron")

o/p: iNeuroniNeuroniNeuroniNeuron

In this code, we use the string concatenation operator (+) to concatenate the string "Neuron" to the end of the string "iNeuron" repeated four times using the string repetition operator (*). This results in the desired output string.

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

Sol: num = int(input("Enter a number: "))

if num % 2 == 0:
    print(num, "is even")
else:
    print(num, "is odd")

In this code, we first use the input() function to take a number as input from the user and convert it to an integer using the int() function. We then use an if statement to check if the number is even or odd. If the remainder of the number divided by 2 is 0, then the number is even, and we print a message saying so. Otherwise, the number is odd, and we print a message indicating that.

Q18. What are boolean operator?

Boolean operators are used to combine or modify the logical values of operands (i.e., True or False) in a logical expression. In Python, there are three boolean operators: and, or, and not. Here is a brief description of each of them:

and: The and operator returns True if both operands are True, and False otherwise. It evaluates the left operand first and only evaluates the right operand if the left operand is True.

or: The or operator returns True if at least one of the operands is True, and False otherwise. It evaluates the left operand first and only evaluates the right operand if the left operand is False.

not: The not operator returns the opposite boolean value of its operand. If the operand is True, then not returns False, and if the operand is False, then not returns True.

Boolean operators are often used in control structures (such as if statements and loops) to make decisions based on multiple conditions.

Q19. What will the output of the following?
```
1 or 0

0 and 0

True and False and True

1 or 0 or 0
```
Ans: The output of the following boolean expressions would be:

1 or 0: This expression will evaluate to 1 because the or operator returns the first True value it encounters, and 1 is considered True in Python. So the expression will short-circuit and return 1.

0 and 0: This expression will evaluate to 0 because the and operator returns the first False value it encounters, and 0 is considered False in Python. So the expression will short-circuit and return 0.

True and False and True: This expression will evaluate to False because the and operator returns the first False value it encounters. In this case, it will evaluate True and False, which is False, and short-circuit without evaluating the third operand.

1 or 0 or 0: This expression will evaluate to 1 because the or operator returns the first True value it encounters. In this case, it will evaluate 1 or 0, which is 1, and short-circuit without evaluating the third operand.

Q20. What are conditional statements in Python?

ANs: Conditional statements in Python are used to execute certain code if a certain condition is met. The most commonly used conditional statements in Python are if, elif, and else.

The syntax of the if statement is as follows:
if condition:
    statement(s)

Here, condition is an expression that returns a boolean value (True or False), and statement(s) is a block of code that is executed only if the condition is true.

The elif statement is used to check for additional conditions if the previous if or elif statement(s) are not true. The syntax is:

if condition1:
    statement(s)
elif condition2:
    statement(s)
else:
    statement(s)

Here, condition1 is checked first, and if it is true, statement(s) is executed and the program skips to the end of the block. If condition1 is false, then condition2 is checked, and if it is true, statement(s) is executed, and the program skips to the end of the block. If neither condition1 nor condition2 are true, then statement(s) in the else block is executed.

The else statement is used to execute a block of code if none of the if or elif conditions are true. The syntax is:

if condition1:
    statement(s)
elif condition2:
    statement(s)
else:
    statement(s)

Here, statement(s) in the else block is executed only if neither condition1 nor condition2 are true.



Q21. What is use of 'if', 'elif' and 'else' keywords?
Ans: if, elif, and else are keywords in Python that are used for conditional execution of code.

The if statement is used to execute a block of code if a certain condition is true. It has the following syntax:

if condition:
    statement(s)

Here, condition is an expression that returns a boolean value (True or False), and statement(s) is a block of code that is executed only if the condition is true.

The elif statement is used to check for additional conditions if the previous if or elif statement(s) are not true. It has the following syntax:

if condition1:
    statement(s)
elif condition2:
    statement(s)

Here, condition1 is checked first, and if it is true, statement(s) is executed and the program skips to the end of the block. If condition1 is false, then condition2 is checked, and if it is true, statement(s) is executed, and the program skips to the end of the block. If neither condition1 nor condition2 are true, then the program continues executing the code outside the block.

The else statement is used to execute a block of code if none of the if or elif conditions are true. It has the following syntax:

if condition1:
    statement(s)
elif condition2:
    statement(s)
else:
    statement(s)

Here, statement(s) in the else block is executed only if neither condition1 nor condition2 are true. If either condition1 or condition2 are true, then the program skips to the end of the block and does not execute the else statement.


Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

Ans: Here is the code to take the age of a person as an input and display "I can vote" if age >= 18, and "I can't vote" if age is < 18:

age = int(input("Enter your age: "))

if age >= 18:
    print("I can vote")
else:
    print("I can't vote")

In this code, we first use the input() function to take the age of the person as an input from the user. We then convert the input to an integer using the int() function and store it in the variable age.

Next, we use an if statement to check if age is greater than or equal to 18. If it is, we print "I can vote" using the print() function. If age is less than 18, the else block is executed and we print "I can't vote".

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

Ans: Here's the code to take 3 numbers as input from the user and display the greatest number as output:

num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))
num3 = float(input("Enter the third number: "))

if num1 >= num2 and num1 >= num3:
    print(num1, "is the greatest number")
elif num2 >= num1 and num2 >= num3:
    print(num2, "is the greatest number")
else:
    print(num3, "is the greatest number")

In this code, we first use the input() function to take three numbers as input from the user. We then convert them to floating-point numbers using the float() function and store them in the variables num1, num2, and num3.

Next, we use a series of if-elif-else statements to compare the three numbers and determine which one is the greatest.

In the first if statement, we check if num1 is greater than or equal to num2 and num3. If it is, we print num1 as the greatest number.

If num1 is not the greatest number, we move on to the second elif statement, where we check if num2 is greater than or equal to num1 and num3. If it is, we print num2 as the greatest number.

If neither of the first two conditions are met, then num3 must be the greatest number, so we print num3 as the output.

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

Code :
numbers = [12, 75, 150, 180, 145, 525, 50]

for num in numbers:
    if num > 500:
        break  # stop the loop if number is greater than 500
    if num % 5 == 0:
        if num > 150:
            continue  # skip the number if it's greater than 150
        print(num)
In this code, we have a list of numbers stored in the numbers variable. We use a for loop to iterate over each number in the list.

Within the loop, we use an if statement to check if the number is greater than 500. If the number is greater than 500, we break out of the loop using the break statement.

If the number is not greater than 500, we continue with the loop and check if the number is divisible by 5 using the modulo operator %. If the number is divisible by 5, we use another if statement to check if the number is greater than 150. If the number is greater than 150, we skip it using the continue statement and move on to the next number.

If the number is not greater than 150, we print it using the print() function.

When we run this program, the output will be:
75
50
These are the only numbers from the list that satisfy the conditions in the if statements.




```
Q26. What is a string? How can we declare string in Python?

Ans26. In Python, Strings are arrays of bytes representing Unicode characters.

Q27. How can we access the string using its index?

Ans27. Sqaure brackets can used to access the elements of the string.

Q28. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "iNeuron"
```
Ans28. 
```python
string[9:16]
```
Q29. Write a code to get the desired output of the following
```
string = "Big Data iNeuron"
desired_output = "norueNi"
```
Ans29. 
```python
string[15:8:-1]
```

Q30. Resverse the string given in the above question.
Ans30. 
```python
string[::-1]
```

Q31. How can you delete entire string at once?

Ans31. We can delete the entire string at once by using del keyword.
```python
str1 = "Hello"
del(str1)
```

Q32. What is escape sequence?

Ans32. The "backslash (\)" character as an escape character. In other words, it has a special meaning when we use it inside the strings. As the name suggests, the escape character escapes the characters in a string for a brief moment to introduce unique inclusion.

Q33. How can you print the below string?
```
'iNeuron's Big Data Course'
```
Ans33. 'iNeuron\'s Big Data Course'

Q34. What is a list in Python?

Ans34. Python list are dynamically sized array, declared in languages like C++ and Java. A list is a collection of things, enclosed in [ ] and separated by commas. 

Q35. How can you create a list in Python?

Ans35. You can create a list by opening and closing the square brackets.

Q36. How can we access the elements in a list?

Ans36. We can access the elements in a list by indexing.

Q37. Write a code to access the word "iNeuron" from the given list.
```
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
``` 
Ans37.
```python
lst = [1,2,3,"Hi",[45,54, "iNeuron"], "Big Data"]
lst[4][2]
```
Q38. Take a list as an input from the user and find the length of the list.

Ans38. 
```python
n = input("Enter number of elements seprated by space: ").split(" ")
print(len(n))
```

Q39. Add the word "Big" in the 3rd index of the given list.
```
lst = ["Welcome", "to", "Data", "course"]
```
Ans39. 
```python
lst = ["Welcome", "to", "Data", "course"]
lst.insert(2, "Big")
```

Q40. What is a tuple? How is it different from list?

Ans40. Tuple is a collection of Python objects much like a list. The sequence of values stored in a tuple can be of any type, and they are indexed by integers. 
Tuples are immutable where as list are mutable. We can also faster through the tuples than the list.

Q41. How can you create a tuple in Python?

Ans41. We can create tuple using round brackets ().

Q42. Create a tuple and try to add your name in the tuple. Are you able to do it? Support your answer with reason.

Ans42. No, I can't as tuples are immutable. The work around is it typecast tuple to list and then append.
```python
tup = ()
tup = list(tup)
tup.append("Vishal")
tup = tuple(tup)
tup
```

Q43. Can two tuple be appended. If yes, write a code for it. If not, why?

Ans43.Yes, we can.
```python
tup1 = ("Vishal ")
tup2 = ("Singh")
tup1+tup2
```

Q44. Take a tuple as an input and print the count of elements in it.

Ans44. 
```python
x = input("Enter the values separeted by space: ").split(" ")
x = tuple(x)
print(len(x))
```

Q45. What are sets in Python?

Ans45. A set is an unordered collection of data types that is iterable, mutable and has no duplicate elements. The order of elements in a set is undefined though it may consist of various elements.

Q46. How can you create a set?

Ans46. We can create set using curly brackets {}. Keep in mind empty {} will result in dictionary hence there must be some value in the brackets.

Q47. Create a set and add "iNeuron" in your set.

Ans47. 
```python
set1 = {"iNeuron"}
set1
```

Q48. Try to add multiple values using add() function.

Ans48. 
```python
set1.add("Big")
set1.add("Data")
set1
```

Q49. How is update() different from add()?

Ans49. We can add more than one element in a single go using update(), but using add() it's not possible.

Q50. What is clear() in sets?

Ans50. To remove all the elements from the set, clear() function is used.

Q51. What is frozen set?

Ans51. Frozen sets in Python are immutable objects that only support methods and operators that produce a result without affecting the frozen set or sets to which they are applied. While elements of a set can be modified at any time, elements of the frozen set remain the same after creation. 

Q52. How is frozen set different from set?

Ans52.
- Frozen sets are immutable where as sets are mutable.
- Sets can't be used as keys in dictionary where as frozen sets can be used.

Q53. What is union() in sets? Explain via code.


Ans53. Python set Union() Method returns a new set which contains all the items from the original set.
```python
set1 = {2, 4, 5, 6}
set2 = {4, 6, 7, 8}
set3 = {7, 8, 9, 10}

print("set1 U set2 : ", set1 | set2)

print("set1 U set2 U set3 :", set1 |set2 | set3)
```

Q54. What is intersection() in sets? Explain via code.

Ans54. Python set intersection() method returns a new set with an element that is common to all set
```python
set1 = {2, 4, 5, 6}
set2 = {4, 6, 7, 8}
set3 = {4, 6, 8}

print("set1 intersection set2 : ", set1.intersection(set2))

print("set1 intersection set2 intersection set3 :", set1.intersection(set2, set3))
```

Q55. What is dictionary ibn Python?

Ans55. Dictionary in Python is a collection of keys values, used to store data values like a map, which, unlike other data types which hold only a single value as an element.

Q56. How is dictionary different from all other data structures.

Ans56. Dictionary is having key and value pair where as all other data structures have only values in them.

Q57. How can we delare a dictionary in Python?

Ans57. We can create dictionary using curly brackets {}.

Q58. What will the output of the following?
```
var = {}
print(type(var))
```
Ans58. dict

Q59. How can we add an element in a dictionary?

Ans59. 
```python
Dict = {}
Dict[0] = "Hello"
Dict[1] = "Course: ["Data Science", "Big Data"]"
```

Q60. Create a dictionary and access all the values in that dictionary.

Ans60. 
```python
Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
for i, j in Dict.items():
  print(f"Key is {i} and value is {j}")
```

Q61. Create a nested dictionary and access all the element in the inner dictionary.

Ans61.
```python
Dict = {"Name": {"f_name":"Vishal", "l_name":"Singh"}, "Experience": 3, "Organisation":"iNeuron"}
for i, j in Dict["Name"].items():
  print(f"Key is {i} and value is {j}")
```
Q62. What is the use of get() function?

Ans62. get() is also to access the elements in dictionary.
```python
Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.get("Name"))
```
Q63. What is the use of items() function?

Ans63. items() method is used to return the list with all dictionary keys with values.
```python
Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.items())
```
Q64. What is the use of pop() function?

Ans64.
```python
Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.pop("Name"))
```
Q65. What is the use of popitems() function?

Ans65. popitem() method removes the last inserted key-value pair from the dictionary and returns it as a tuple.
```python
Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.popitem())
```
Q66. What is the use of keys() function?

Ans66.  keys() method returns a view object that displays a list of all the keys in the dictionary.
```python
Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.keys())
```
Q67. What is the use of values() function?


Ans67. values() is an inbuilt method in Python programming language that returns a view object. The view object contains the values of the dictionary, as a list.
```python
Dict = {"Name": "Vishal", "Experience": 3, "Organisation":"iNeuron"}
print(Dict.values())
```

Q68. What are loops in Python?

Ans68. Loops are used the iterate over a block of statement multiple times.

Q69. How many type of loop are there in Python?

Ans69. There is for and while loop in Python

Q70. What is the difference between for and while loops?

Ans70. When we know the exact number of iterations, we can use for loop. When we want the to run till a certain condition is true we can use while loop.

Q71. What is the use of continue statement?

Ans71. Continue Statement skips the execution of the program block from after the continue statement and forces the control to start the next iteration.

Q72. What is the use of break statement?

Ans72. break statement in Python is used to bring the control out of the loop when some external condition is triggered. break statement is put inside the loop body

Q73. What is the use of pass statement?

Ans73. The pass statement is a null statement. But the difference between pass and comment is that comment is ignored by the interpreter whereas pass is not ignored. 

Q74. What is the use of range() function?

Ans74. range() function returns a sequence of numbers, in a given range. The most common use of it is to iterate sequence on a sequence of numbers

Q75. How can you loop over a dictionary?

Ans75. 
```python
statesAndCapitals = {
	'Gujarat': 'Gandhinagar',
	'Maharashtra': 'Mumbai',
	'Rajasthan': 'Jaipur',
	'Bihar': 'Patna'
}

for state in statesAndCapitals:
	print(state)
```

### Coding problems
Q76. Write a Python program to find the factorial of a given number.

Ans76.
```python
def factorial(n):
  if n < 0:
    return 0
  elif n == 0 or n == 1:
    return 1
  else:
    fact = 1
    while(n>1):
      fact *= n
      n -= 1
    return fact

n=6
print(f"Factorial of {n} is {factorial(n)}")
```
Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (P*R*T)/100

Ans77.
```python
def SI(p,r,t):
  si = (p*r*t)/100
  print(f"Simple interest is {si}")
  return si

SI(8, 8, 6)
```      
Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.

Ans78.
```python
def CI(p, r, t):
  amount = p*(1+r/100)**t
  ci = amount - p
  print(f"Compound intrest is {ci}")
  return ci

CI(10000, 10.25, 5)
```
Q79. Write a Python program to check if a number is prime or not.

Ans79.
```python
from math import sqrt

def is_prime(n):
  prime_flag = 0

  if(n > 1):
    for i in range(2, int(sqrt(n)) + 1):
      if (n % i == 0):
        prime_flag = 1
        break
    if (prime_flag == 0):
      print(f"{n} is a prime number.")
    else:
      print(f"{n} is not a prime number.")
  else:
    print(f"{n} is not a prime number.")

is_prime(134)
```
Q80. Write a Python program to check Armstrong Number.

Ans80.
```python
def check_armstrong(n):
  s = n
  b = len(str(n))
  sum1 = 0
  while n != 0:
      r = n % 10
      sum1 = sum1+(r**b)
      n = n//10
  if s == sum1:
      print(f"The given number {s} is armstrong number")
  else:
      print(f"The given number {s} is not armstrong number")

check_armstrong(153)
```
Q81. Write a Python program to find the n-th Fibonacci Number.

Ans81.
```python
def Fibonacci(n):
	if n<= 0:
		print("Incorrect input")
	elif n == 1:
		return 0
	elif n == 2:
		return 1
	else:
		return Fibonacci(n-1)+Fibonacci(n-2)

print(Fibonacci(7))
```
Q82. Write a Python program to interchange the first and last element in a list.

Ans82.
```python
def swap_list(newList):
	size = len(newList)
	temp = newList[0]
	newList[0] = newList[size - 1]
	newList[size - 1] = temp
	
	return newList

newList = [15, 12, 35, 17, 9, 56, 29]

print(swap_list(newList))
```
```python
def swap_list(newList):
     
    newList[0], newList[-1] = newList[-1], newList[0]
 
    return newList
     
newList = [15, 12, 35, 17, 9, 56, 29]
print(swap_list(newList))
```
Q83. Write a Python program to swap two elements in a list.

Ans83.
```python
def swapPositions(list, pos1, pos2):
	
	list[pos1], list[pos2] = list[pos2], list[pos1]
	return list

List = [15, 12, 35, 17, 9, 56, 29]
pos1, pos2 = 1, 3

print(f"Original list: {List}")
print(f"Swapped list: {swapPositions(List, pos1, pos2)}")
```
Q84. Write a Python program to find N largest element from a list.

Ans84.
```python
def n_max_elements(list1, N):
	final_list = []

	for i in range(0, N):
		max1 = 0
		
		for j in range(len(list1)):	
			if list1[j] > max1:
				max1 = list1[j];
				
		list1.remove(max1);
		final_list.append(max1)
		
	print(final_list)

list1 = [2, 6, 41, 85, 0, 3, 7, 6, 10]
N = 3

n_max_elements(list1, N)
```
Q85. Write a Python program to find cumulative sum of a list.

Ans85.
```python
def cumulative_sum(lists):
	cu_list = []
	length = len(lists)
	cu_list = [sum(lists[0:x:1]) for x in range(0, length+1)]
	return cu_list[1:]

lists = [10, 20, 30, 40, 50]
print(f"Cumulative sum of the list is {cumulative_sum(lists)}")
```
Q86. Write a Python program to check if a string is palindrome or not.

Ans86.
```python
def isPalindrome(s):
  if s == s[::-1]:
	  return f"{s} is palindrome"
  return f"{s} is not palindrome"

s = "dad"
isPalindrome(s)
```
Q87. Write a Python program to remove i'th element from a string.

Ans87.
```python
def remove_ith_element(i):
  str1 = "Big Data Bootcamp"
  str2 = ""

  for n in range(len(str1)):
    if n == i:
      continue
    else:
      str2 = str2 + str1[n]

  return str2

remove_ith_element(5)
```
Q88. Write a Python program to check if a substring is present in a given string.

Ans88.
```python
def check_substring(s2, s1):
	if (s2.count(s1) > 0):
		print(f'"{s1}" is a substring of "{s2}"')
	else:
		print(f'"{s1}" is not a substring of "{s2}"')


s2 = "Welcome to iNeuron Big Data Bootcamp"
s1 = "iNeuron"
check_substring(s2, s1)
```
Q89. Write a Python program to find words which are greater than given length k.

Ans89.
```python
def string_greater_than_k(k, str):
	
	string = []

	text = str.split(" ")

	for x in text:

		if len(x) > k:

			string.append(x)

	return string

k = 3
str ="Big Data Bootcamp"
print(string_greater_than_k(k, str))
```
Q90. Write a Python program to extract unquire dictionary values.

Ans90.
```python
test_dict = {'iNeuron': [5, 6, 7, 8],
			'is': [10, 11, 7, 5],
			'best': [6, 12, 10, 8],
			'for': [1, 2, 5],
      'big data': [2, 7, 12, 9]
      }

print("The original dictionary is : " + str(test_dict))

res = list(sorted({ele for val in test_dict.values() for ele in val}))

print("The unique values list is : " + str(res))
```
Q91. Write a Python program to merge two dictionary.

Ans91.
```python
def Merge(dict1, dict2):
	return(dict2.update(dict1))

dict1 = {'a': 10, 'b': 8}
dict2 = {'d': 6, 'c': 4}

print(Merge(dict1, dict2))

print(dict2)

```
Q92. Write a Python program to convert a list of tuples into dictionary.
```python
Input : [('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]
Output : {'Sachin': 10, 'MSD': 7, 'Kohli': 18, 'Rohit': 45}
```
Ans92.
```python
print (dict([('Sachin', 10), ('MSD', 7), ('Kohli', 18), ('Rohit', 45)]))
```

Q93. Write a Python program to create a list of tuples from given list having number and its cube in each tuple.
```python
Input: list = [9, 5, 6]
Output: [(9, 729), (5, 125), (6, 216)]
```
Ans93.
```python

list1 = [9, 5, 6]

res = [(val, pow(val, 3)) for val in list1]

print(res)

```
Q94. Write a Python program to get all combinations of 2 tuples.
```python
Input : test_tuple1 = (7, 2), test_tuple2 = (7, 8)
Output : [(7, 7), (7, 8), (2, 7), (2, 8), (7, 7), (7, 2), (8, 7), (8, 2)]
```
Ans94.
```python
test_tuple1 = (7, 2)
test_tuple2 = (7, 8)

res = [(a, b) for a in test_tuple1 for b in test_tuple2]
res = res + [(a, b) for a in test_tuple2 for b in test_tuple1]

print("The filtered tuple : ", str(res))
```
Q95. Write a Python program to sort a list of tuples by second item.
```python
Input : [('452', 10), ('256', 5), ('100', 20), ('135', 15)]
Output : [('256', 5), ('452', 10), ('135', 15), ('100', 20)]
```
Ans95.
```python
def Sort_Tuple(tup):
     
    lst = len(tup)
    for i in range(0, lst):
         
        for j in range(0, lst-i-1):
            if (tup[j][1] > tup[j + 1][1]):
                temp = tup[j]
                tup[j]= tup[j + 1]
                tup[j + 1]= temp
    return tup
 
tup =[('452', 10), ('256', 5), ('100', 20), ('135', 15)]
       
print(Sort_Tuple(tup))
```
Q96. Write a python program to print below pattern.
```
* 
* * 
* * * 
* * * * 
* * * * * 
```
Ans96.
```python
def pypart(n):
	
	for i in range(0, n):
	
		for j in range(0, i+1):
		
			print("* ",end="")
	
		print("\r")

n = 5
pypart(n)

```
Q97. Write a python program to print below pattern.
```
    *
   **
  ***
 ****
*****
```
Ans97.
```python
def inverse_pattern():
  n=5;i=0
  while(i<=n):
    print(" " * (n - i) +"*" * i)
    i+=1

inverse_pattern()
```
Q98. Write a python program to print below pattern.
```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```
Ans98.
```python

def triangle(n):
	
	k = n - 1

	for i in range(0, n):

		for j in range(0, k):
			print(end=" ")
	
		k = k - 1
	
		for j in range(0, i+1):

			print("* ", end="")
	
		print("\r")

n = 5
triangle(n)

```
Q99. Write a python program to print below pattern.
```
1 
1 2 
1 2 3 
1 2 3 4 
1 2 3 4 5
```
Ans99.
```python

def numpat(n):

	num = 1

	for i in range(0, n):

		num = 1

		for j in range(0, i+1):

			print(num, end=" ")

			num = num + 1

		print("\r")

n = 5
numpat(n)

```
Q100. Write a python program to print below pattern.
```
A 
B B 
C C C 
D D D D 
E E E E E 
```
Ans100.
```python

def alphapat(n):

	num = 65

	for i in range(0, n):
	
		for j in range(0, i+1):

			ch = chr(num)
		
			print(ch, end=" ")
	
		num = num + 1
	
		print("\r")

n = 5
alphapat(n)

```
