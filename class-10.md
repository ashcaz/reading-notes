## Duckett Ch. 10 Error Handling and Debugging

**Order of Execution**

- understanding the order in whoch things are processed

**Execution Context**

- Every statemnet in a script live in one of three places 
  1. Global context
  2. Function Context
  3. Eval Context

**Error Objects**

- Error : Generic error
- SyntaxError: Syntax has not been followed
- ReferenceError: Tried to reference a variable that is not declared/within scope
- TypeError: An unexpected data type that can not be coerced

**How to Deal With Errors**

1. Debug the script  to fix errors
  - use developer tools
2. Handle Errors Gracefully
  - using try, catch, throw  and finally statements

**Debugging Workflow**

- Where is the problem?
  1. Look at the error message, it tells you
  2. Check how far the script is running
  3. The type of error
- What exactly is the problem?
  1. When you have set breakpoints, you can see if the variables arround them have the values you would expect them to.
  2. Break down/break out  parts of the code to test
  3. Check the numbe of parameters for a function or the number of items for an array

**Summary**

- If you understand execution contexts (which have twostages) and stacks, you are more likely to find the error in your code.

- Debugging is the process of finding errors. It involves a process of deduction.

- The console helps narrow down the area in which the error is located, so you can try to find the exact error.

- JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.

- If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.


[Back to Homepage](https://ashcaz.github.io/reading-notes)