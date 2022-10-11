# Intro to OOP
## Object Oriented Programming.

## What is object-oriented programming?
### Object-oriented programming (OOP) is a computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.

### OOP focuses on the objects that developers want to manipulate rather than the logic required to manipulate them. This approach to programming is well-suited for programs that are large, complex and actively updated or maintained.

## Classes and Objects:
### Objects are an encapsulation of variables and functions into a single entity. 
### Objects get their variables and functions from classes.
### Classes are essentially a template to create your objects.

## Accessing Object Variables:
### To get to the value of an instance variable, you use dot notation, a form of addressing in which an instance or class variable name has two parts: a reference to an object or class on the left side of the dot and a variable on the right side of the dot.


## Accessing Object Functions
###  The data members and member functions of class can be accessed using the dot('.') operator with the object.

## What is init() used for in class? 
### The __init__() function, is a special function that is called when the class is being initiated. It's used for assigning values in a class.


# Thinking Recursively in Python:
### If the problem represents a simple case, solve it. If not, divide it into subproblems and apply the same strategy to them.


## Recursive Functions in Python:
###  A recursive function is a function defined in terms of itself via self-referential expressions.

### This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.

## Recursive Data Structures in Python
### A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure.


# Python Testing with pytest:
###  pytest, a library for testing Python code

### pytest has 2 features :
- fixtures
- code coverage

## 1- fixtures:
### Pytest fixtures are functions that can be used to manage our apps states and dependencies. Most importantly, they can provide data for testing and a wide range of value types when explicitly called by our testing software.

### We can tell pytest that a particular function is a fixture by decorating it with @pytest.fixture.

## 2-code coverage:
### a tool for measuring code coverage of Python programs. It monitors your program, noting which parts of the code have been executed, then analyzes the source to identify code that could have been executed but was not. Coverage measurement is typically .