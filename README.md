# Exception Handling in C++
# Aim
To study and implement the concept of Exception Handling in C++.

Software
Visual Studio Code (VS Code)
Objectives
Understand what exceptions are and why they occur.
Learn how to use try, throw, and catch in C++.
Explore how exception handling improves program reliability.
Differentiate between normal program termination and exception-based termination.
Implement exception handling for common errors such as division by zero and underage voting.
Theory
What is Exception Handling?
Exceptions are runtime anomalies that interrupt the normal flow of a program.
In C++, exception handling provides a structured way to detect, throw, and handle errors so that programs can fail gracefully instead of crashing.
Keywords in C++
try
A block of code that might generate an exception.
throw
Used to raise an exception when an error condition occurs.
catch
A block of code that handles the exception if thrown.
How it Works
Program execution enters a try block.
If an error is detected, a throw statement is executed.
Control jumps to the nearest matching catch block.
If no handler is found, the program terminates abnormally.
Example Situations
Division by zero.
Invalid input formats.
Underage validation for voting.
File handling errors (file not found, permission denied).
Stack Unwinding
When an exception is thrown, the program unwinds the call stack.
Destructors of local objects are automatically called during this process, ensuring resource cleanup.
This is why C++ exception handling works well with RAII (Resource Acquisition Is Initialization).
Advantages
Separates error handling from normal logic.
Prevents abnormal program termination.
Provides flexible handling using multiple catch blocks for different exception types.
Enhances maintainability and readability.
# Conclusion
Exception handling in C++ is a powerful mechanism to deal with runtime errors effectively.
It ensures that errors such as invalid input, division by zero, or underage voting do not cause the program to crash abruptly.
By using try, throw, and catch, programmers can separate error-handling logic from normal program logic, making applications more robust and user-friendly.
Properly structured exception handling improves the reliability, maintainability, and clarity of C++ programs.
In real-world development, exceptions should be used for exceptional conditions only, not for routine checks, to balance performance with safety.
