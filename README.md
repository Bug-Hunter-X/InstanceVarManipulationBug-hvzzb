# Unexpected Behavior with Instance Variable Manipulation in Ruby

This repository demonstrates a subtle bug related to directly modifying instance variables in Ruby using `instance_variable_set`. While it's not a syntax error, it can lead to unexpected behavior and is generally considered bad practice.

## The Bug
The `bug.rb` file contains a simple class and then directly changes the instance variable with `instance_variable_set`. While this works, it bypasses any potential getter/setter methods and can make code harder to maintain and debug.

## The Solution
The `bugSolution.rb` file provides a better way to handle this. It uses a setter method, which provides more control, encapsulation, and readability.  This approach allows for data validation and other actions without altering the core functionality of the class.

This example highlights a common pitfall when working with instance variables and advocates for best practices by utilizing methods to interact with object data.