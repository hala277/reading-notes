# Error Handling & Debugging

## The stack

*The JavaScript interpreter processes one line of code at a time. When a statement needs data from another function, it stacks (or piles) the new function on top of the current task. When a statement has to call some other code in order to do its job. the new task goes to the top of the pile of things to do.* 
*Each time a new item is added to the stack, it creates a new execution context. Variables defined in a function (or execution context) are only available in that function. if a function gets called a second time, the variables can have different values.*

### EXECUTION CONTEXT & HOISTING 
*Each time a script enters a new execution context, there are two phases of activity:*
1. PREPARE 
+ The new scope is created 
+ Variables, functions, and arguments are created 
+ The value of the this keyword is determined

2. EXECUTE
+ Now it can assign values to variables 
+ Reference functions and run their code 
+ Execute statements 

### UNDERSTANDING SCOPE 
*In the interpreter, each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent'svariables object.* 
*Functions in JavaScript are said to have lexical scope.  They are linked to the object they were defined within. So,for each execution context, the scope is the current execution context's variables object, plus the variables object for each parent execution context.*

### UND ERSTANDING ERRORS 
![javascript error](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/08/JavaScript-Errors-1200x720.jpg)
*If a JavaScript statement generates an error, then it throws an exception . At that point, the interpreter stops and looks for exception-handling code.*
*If you are anticipating that something in your code may ca use an error, you ca n use a set of statements  to handle the error This is important because if the error is not handled, the script will just stop processing and the user will not know why. So exception-handling code should inform users when there is a problem.*

### ERROR OBJECTS 
Error objects can help you find where your mistakes are and browsers have tools to help you read them. 
When an Error object is created, it will contain the  following properties: 
PROPERTY |DESCRIPTION 
---------|----------------------------
name |Type of execution 
message |Description 
fileNumber |Name of the JavaScript file 
lineN umber| Line number of error 



*There are seven types of built-in error objects in JavaScript.* 
OBJECT| DESCRIPTION 
-----------|-------------------
Error| Generic error - the other errors are all based upon this error 
Syntax Error |Syntax has not been followed 
Reference Error| Tried to reference a variable that is not declared/within scope 
TypeError | An unexpected data type that cannot be coerced
Range Error |Numbers not in acceptable range
URI Error |`encodeURI(),decodeURI()`,and similar methods used incorrectly
EvalError |`eval()` function used incorrectly 

### HOW TO DEAL WITH  ERRORS 
*Now that you know what an error is and how the browser treats them,  there are two things you can do with the errors.* 
1: DEBUG THE SCRIPT TO FIX ERRORS 
*If you come across an error while writing a script (or when someone reports a bug), you will need to  debug the code, track down the source of the error, and fix it.* 
2: HANDLE ERRORS GRACEFULLY 
*You can handle errors gracefully using try, catch, throw, and finally statements.* 

### HANDLING EXCEPTIONS 
*If you know your code might fail, use try, catch, and finally. Each one is given its own code block.* 
```
try { 
// Try to execute this code 
}catch (exception) { 
// If there is an exception, run this code 
}finally { 
// This always gets executed 
}

```
+ TRY 
*First, you specify the code that you think might throw an exception within the try block.  If an exception occurs in this  section of code, control is  automatically passed to the  corresponding catch block. The try clause must be used in this type of error handling code, and it should always have either a catch, finally, or both. If you use a continue, break, or return keyword inside a try, it  will go to the finally option.* 

+ CATCH 
*If the try code block throws an  exception, catch steps in with an  alternative set of code. It has one parameter: the error  object. Although it is optional,  you are not handling the error if you do not catch an error. The ability to catch an error can  be very helpful if there is an issue  on a live website. It lets you tell users that something has gone wrong (rather than not informing them why the site stopped working).*

+ FINALLY 
*The contents of the finally code block will run either way - whether the try block  succeeded or failed. It even runs if a return keyword  is used in the try or catch block.  It is sometimes used to clean up  after the previous two clauses. These methods are similar to the `.done()` , `. fail()`, and `. always()` methods in jQuery.*


**conclusion**
*If you understand execution contexts (which have two  stages) and stacks, you are more likely to find the error  in your code. Debugging is the process of finding errors. It involves a  process of deduction. The console helps narrow down the area in which the  error is located, so you can try to find the exact error.  JavaScript has 7 different types of errors. Each creates  its own error object, which can tell you its line number  and gives a description of the error. If you know that you may get an error, you can handle  it gracefully using the try, catch, finally statements.  Use them to give your users helpful feedback.* 
