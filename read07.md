## Control flow:
*The control flow is the sequence in which a script's statements are executed by the computer.
Unless the computer encounters (very common) structures that modify the control flow, such as conditionals and loops, code is executed in sequence from the first line in the file to the final line.
Consider a script that is used to verify user data from a website form. The script sends verified data, but if the user, for example, forgets to fill in a necessary field, the script encourages them to do so. The script accomplishes this by employing a conditional structure, often known as `if`,`else`, in which different code is executed based on whether the form is completed or not.*

>if (number==1) {
>
>   add();}
>
> else {
>
>   leave();}

## JavaScript Functions:
*A JavaScript function is a piece of code that performs a certain purpose.*

*When "something" calls a JavaScript function, it is executed (calls it).*

example:
>function myFunction(p1, p2) {
>
> return p1 * p2;
>   
>of p1 and p2
>}

### Syntax of javaScript Functions
*The function keyword is used to define a JavaScript function, which is then followed by a name and parenthesis ().Letters, numbers, underscores, and dollar signs can all be used in function names (same rules as variables).*
*Parameter names separated by commas may be included in the parentheses:
`(parameter 1, parameter 2, and so on...)`
The function's code to be run is enclosed in curly brackets:* `{}`

>function name(parameter1, parameter2, parameter3) {
>
>  // code to be executed
>}

+ In the function definition, function arguments are specified inside parentheses ().
+ The values passed to the function when it is called are known as function parameters.
+ The arguments (parameters) are treated as local variables within the function.

### Invoking a function
*When "something" invokes (calls) the function, the code within it will run:*

+ When something happens (when a user clicks a button)

+ When it is used in JavaScript code, it is invoked (called).

+ Conveniently (self invoked)

### Function Return
*The function will cease operating when it reaches a `return` statement in JavaScript.
If the function was called from a statement, JavaScript will execute the code after the statement that called it.
Return values are frequently computed by functions. The`caller` is `returned` the return value.*

### The () Operator is used to call a function.
*ToCelsius refers to the function object in the example above, and toCelsius() refers to the function result.
When you call a function without (), the function object is returned instead of the function result.*

### Variable Values Using Functions
*Functions can be utilized in all sorts of formulae, assignments, and computations in the same manner that variables can.*

### Local Variables  
*Variables defined within a JavaScript function are LOCAL to it.
Only within the function can you access local variables.*

## JavaScript Operators:
![JavaScript Operators](Javascript3.png)
