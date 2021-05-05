# Read: 10 Error Handling & Debugging

## When writing a long script, nobody gets everything right in their first attempt. The error messages that a browser gives look cryptic at first, but they can help you determine what went wrong in your JavaScript and how to fix it. In this chapter you will learn about:
* ***THE CONSOLE & DEV TOOLS*** Tools built into the browser that help you hunt for errors.
* ***COMMON PROBLEMS*** Common sources of errors, and how to solve them.
* ***HANDLING ERRORS*** How code can deal with potential errors gra cefully.

## ORDER OF EXECUTION
### To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

![SA](https://www.oreilly.com/library/view/javascript-and-jquery/9781118531648/images/p452-001.jpg)
## EXECUT.ION CONTEXTS
### The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.


## 1- EXECUTION CONTEXT
 ### Every statement in a script lives in one of three execution contexts:
 *  GLOBAL CONTEXT
   * Code that is in the script, but not in a function. There is only one global context in any page.
* FUNCTION CONTEXT
  * Code that is being run within a function.
  * Each function has its own function context.
* EVAL CONTEXT 
  * Text is executed like code in an internal function called eva l {) (which is not covered in this book).

## 2- VARIABLE SCOPE
### The first two execution contexts correspond with the notion of scope (which you met on p98):
* GLOBAL SCOPE
  * If a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope.
* FUNCTION-LEVEL SCOPE
 * When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.

## EXECUTION CONTEXT & HOISTING
### Each time a script enters a new execution context, there are two phases of activity:
### 1- PREPARE
* The new scope is created
* Variables, functions, and arguments are created
* The value of the this keyword is determined


### 2- EXECUTE
* Now it can assign values to variables
* Reference functions and run their code
* Execute statements

## UNDERSTANDING SCOPE
### In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's v a ri ables object.

## UNDERSTANDING ERRORS
### If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.

##  ERROR OBJECTS cONTINUED
### some error you must know it :
* Syntax Error
* Ref erenceError
* EvalError
* URI Error
* Type Error
* RangeError
* NAN 

## HOW TO DEAL WITH ERRORS
### Now that you know what an error is and how the browser treats them, there are two things you can do with the errors.


## 1- DEBUG THE SCRIPT TO FIX ERRORS
* If you come across an error while writing a script (or when someone reports a bug), you will need to debug the code, track down the source of the error, and fix it.
## 2- HANDLE ERRORS GRACEFULLY
* You can handle errors gracefully using try, catch, throw, and f i na 1 ly statements.


## HOW TO LOOK AT ERRORS IN CHROME
### The console will show you when there is an error in your JavaScript. It also displays the line where it became a problem for the interpreter.
*  The Console option is selected.
* The type of error and the error message are shown in red.
* The file name and the line number are shown on the right-hand side of the console.

![ERE](https://i.stack.imgur.com/XsbFr.png)
# summary 
## 1-If you understand execution contexts (which have two stages) and stacks, yo are more likely to find the error in your code.
## 2-Debugging is the process of finding errors. It involves a process of deduction.
## 3-The console helps narrow down the area in which the error is located, so you can try to find the exact error.
## 4- JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.
## 5- If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements.
## 6-Use them to give your users helpful feedback.