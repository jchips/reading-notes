# Class 2

## What are the key principles of Test-Driven Development (TDD) in Python, and how do they contribute to the overall quality of code?

1. Write failing tests first
2. Write minimum code to pass test
3. Refactor the code to improve it

This strategy improves reliability.

Source: [code.likeagirl.io](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

## Explain the purpose of the if __name__ == '__main__': statement in Python scripts. What are some use cases for including this conditional in your code?

The purpose is to check if the code is coming from its own module instead of being imported. "`if __name__ == “__main__”:` is used to execute some code only if the file was run directly, and not imported." This will make certain executions only happen when running the `__main__` module.

Note: "Python files can act as either reusable modules, or as standalone programs."

Source: [geeksforgeeks.org](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)

## Describe the concept of recursion in Python

Recursion is when a function calls itself. It needs a base case so, when the base case is met, the function will stop recursing.

Source: [geeksforgeeks.org](https://www.geeksforgeeks.org/introduction-to-recursion-2/)

## What is the difference between Python modules and packages? Explain how to create, import, and use them in your Python programs

A Python module is a single file that has the extension `.py`. It contains Python code such as functions, classes, or variables.

A Python package is a collection of modules in a directory that has an `__init.py__` file. The presence of an `__init.py__` file represents that the directory is a package (even if the `__init.py__` nothing has nothing in it). TLDR: A Python package contains multiple modules.
To create a module: Put legitimate Python code in a file and give the file a name with the py extension. EX: `file_name.py`.
To import: A module's contents are accessed using import statements. EX: `import file_name` (imports file_name.py).
To use a module: `file_name.fun()` calls a function named `fun()` from the file_name.py module. `print(file_name.s)` prints out a variable named `s` from the file_name.py module.

Source: [realpython.com](https://realpython.com/python-modules-packages/)
