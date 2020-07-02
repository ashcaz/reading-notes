# The Call Stack and Debugging

Links:

- [The call stack defined on MDN](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)
- [Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)
- [JavaScript Error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)



## Call Stack (article 1)

A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.


- When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
- Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
- When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
- If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.

```JavaScript
function greeting() {
   // [1] Some codes here
   sayHi();
   // [2] Some codes here
}
function sayHi() {
   return "Hi!";
}

// Invoke the `greeting` function
greeting();

// [3] Some codes here
```

## The JavaScript Call Stack (article 2)

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.


The understanding of the call stack is vital to Asynchronous programming


**LIFO (Last In, First Out)**: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

![LIFO pic](../img/LIFO-image.png)


**What is a stack Overflow**

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

```JavaScript
function callMyself(){
  callMyself();
}

callMyself();
```

## JavaScript error messages && debugging (article 3)

- soooo many errors. READ THIS

[Back to Homepage](https://ashcaz.github.io/reading-notes)