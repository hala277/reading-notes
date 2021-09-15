# React and Forms

## Forms

1. What is a ‘Controlled Component’?
*React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way*
2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
*No,mutable state is typically kept in the state property of components, and only updated with setState().*
3. How do we target what the user is entering if we have an event handler on an input field?
*add a name attribute to each element and let the handler function choose what to do based on the value of `event.target.name.`*

## The Conditional (Ternary) Operator Explained

Why would we use a ternary operator?

1.A ternary operator lets you assign one value to a variable if the condition is true, and another if the condition is false.
2.The assignment of a value to a variable is easier to read with a ternary operator since it is confined on a single line rather than an if else block.

Rewrite the following statement using a ternary statement:

``` javascript
 if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```

``` javascript
x===y ? console.log(true) : console.log(false)
```

## Things I want to know more about

* *React Bootstrap - Forms*

* *React Bootstrap - alert*

* *more about ternary statement*
