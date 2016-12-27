# Table of Contents
- [Introduction](#Introduction)
  - [Python installation](#Python-installation)
  - [My first program](#My-first-program)

# Introduction
Python is an open source, object-oriented  interpreted language which was originally created in the late 1980s, but only became widely used in the 2000s after the release of version 2.0. 
It is known for its clear, simple syntax and its dynamic typing – the same variables in Python can be reused to store values of different types; something which would not be allowed in a statically-typed language like C or Java. 
Everything in Python is an object, but Python can be used to write code in multiple styles – procedural, object-oriented or even functional.

## Python installation
Follow instruction at https://www.python.org/downloads/

## Invoke python
There are three different ways we can work with ruby.
- The First is going to be a single command.
- The Second will be using a python file, actually saving a file that has Ruby code in it. 
- The Third will be using the interactive interpreter

### Example of first one
```python
$> python -c 'print "hello world"'
$> python -c 'print("hello world\n") # puts add a new line
```
> **Note** : small bracket are optional 

### Example of second one
write the content in a file `hello_world.py` 
```python
#! /usr/bin/env python
print ("hello world\n")
```
Compile/Test for syntax  using
``` 
$>  python -m py_compile hello_world.py
```
Execute it using
```
$> python  hello_world.py
or
$> ./hello_world.py
```
### Example of third one
Using the interactive interpreter
- Allow us to interact with code in realtime
- work like a calc
- great testing tool

To get a interactive interpreter just type python which shows python shell as  `>>>`

```python
>>> print "hello world\n"
hello world
```
Few other  example 
```python
>>> 4 + 5
9
>>> print 4 + 5
9
>>> print "4 + 5"
4 + 5
```
## Tools for my first program

### Comments
In python comments start with hash or pound character (#), or """
```python
# I am single line comment , ignore me
print "my name is santosh" # I am comment in the same line as code, code will be executed and I will be ignored
"""
multiline comment started with three quotes
keep saying bla bla 
bla bla bla bla
comment end with three quotes
"""
```

### variable name
variable is a label for a location in memory. It can be used to hold a value. In statically typed languages, variables have predetermined types, and a variable can only be used to hold values of that type. 
In Python, we may reuse the same variable to store values of any type. Variables in ruby are lowercase letter with _  in it.
- Example includes
  - name = "santosh yadav"
  - age = 34
  - float_age = 34.0
  - arr = [1,2,3,4]
  - count, result, total = 0, 0, 0  # Define three variables at once
- Variable doesn't have data type . A variable can hold any data type.

### Get user input
In python we use input to get user input. In python 2 raw_input is used. For example
- name = input('Enter your name: ')
- age = input('Enter your age: ')
- name = raw_input("Please enter your name: ") # for python 2x

### Display string with string evaluation
print is used to display content to stdout
```python
print('Hello')
print('Hello', name)
print "Hi my name is ",name, "and age is", age
print "Hi my name is " + name + "and age is " + str(age) # we need to convert age to string
print ("Hi my name is %s and age is %d" %(name,age)) # note that there is no comma after string and variables names
# More fancier and new output format
print "Hi my name is {} and half age is {}".format(name, age) 
```

## My first program
Get name and age and return half of the age entered.
```python
#! /usr/bin/env python
name = input('Enter your name: ')  # Enter your name with quotes "Santosh yadav" . Use raw_input if quotes not to be forced
age = input('Enter your age : ')
half_age = age//2   # // forces division for two integer
print "Hi , My name is ", name ," and half age is ", half_age  # string manipulation using #{variable}
```
Output
```bash
./a.python
Enter your name : "Santosh Yadav"
Enter your age : 34
Hi , My name is  Santosh Yadav  and half age is  17

Next run shows python is very typed language as compaired to ruby
./a.rb
Enter your name : santosh
Enter your name: santosh
Traceback (most recent call last):
  File "a.py", line 2, in <module>
    name = input('Enter your name: ')  # Enter your name with quotes "Santosh yadav"
  File "<string>", line 1, in <module>
NameError: name 'santosh' is not defined
Enter your age : san
Enter your age : san
Traceback (most recent call last):
  File "a.py", line 3, in <module>
    age = input('Enter your age : ')
  File "<string>", line 1, in <module>
NameError: name 'san' is not defined
```

# Integer
An Integer (int type) is a whole number such as 1, 5. 
Python can display an integer with the print function, but only if it is the only argument:
```python
print(3) # print 3
# We can add two numbers together
print(1 + 2) # print 3
```
## Integer operation 
|Operation |	Symbol |	Example |	Result|
| --- | --- | --- | --- | 
|Addition 	|+ |	25 + 10 |	35|
|Subtraction | 	- |	25 - 10 |	15|
|Multiplication |	* |	25 * 10 |	250|
|Division |	// 	|25 //10 |	2|
|Modulus (remainder) | 	% |	25 % 10 |	5|
|Exponent (power) |	** |	25**2 |	625|

> **Note** : In Python 2, the operator / performed integer division if both the dividend and the divisor were integers, and floating-point division if at least one of them was a float. In Python 3, / always performs floating-point division and // always performs integer division – even if the dividend and divisor are floats!


# Float
The Float class is for floating-point numbers. 


# String

Example
- name = "santosh yadav"
- strvar = str("new world")

# File handle

# My second program

