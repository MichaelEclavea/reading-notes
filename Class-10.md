# Chapter 10: "Error Handling and Debugging"

If variables are created in a function, the variable is only known within that function. 
if A variable is created outside a function, it is called a global scope. It can be used and calley anytime globally. 

### Browser Errors:

-Object     Description
1. Error    Generic error. Causes all other errors because of this. 
2. Syntax Error - Coding syntax was not followed correctly.
3. Reference Error - Undeclared variable
4. Type Error - unexpedited data 
5. Range Error - unacceptable data Type

A great resource for debugging code is through web browsers. Each browser has developer tools to help locate tand to explain what errors were found.

There are three different ways to communicate with the browser.
1. Console.info() used for general information
2. Console.warn() used for warnings 
3. Console.error() used to hold errors

Console.assert() test if a condition is met, console write to conosle only if consdition is false.

### Breakpoints 

#### Steps: 
1. From browser go to developer tools and go to sources
2. Find file breakpoints at left menu
3. click on spot to stop running at that location on code.

### Debugger

Type debugger anywhere on your code. If developer tools are open, it will automatically create a breakpoint. 

### NAN is when you put a string in a mathematical operation. NaN (not a number).
