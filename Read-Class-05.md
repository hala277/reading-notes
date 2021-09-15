# Putting it all together

## Thinking in React

1. What is the single responsibility principle and how does it apply to components?
*One such technique is the single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.*
2. What does it mean to build a ‘static’ version of your application?
*Create a version that takes your data model and generates the UI, but doesn't allow you to interact with it. It's preferable to separate these processes since creating a static version necessitates a lot of typing but little thought, whereas adding interaction necessitates a lot of thinking but little type.Create components that reuse other components and utilize props to pass data. Props are a means for data to be sent from a parent to a child. If you're familiar with the idea of state, you shouldn't utilize it to create this static version. Only interactivity, or data that varies over time, is allowed to use state.*
3. Once you have a static application, what do you need to add?
*Identify The Minimal Representation Of UI State,Consider the bare minimum of changeable state that your program requires. Calculate anything else you need on-demand after determining the absolute minimum representation of the state your application requires.*
4. What are the three questions you can ask to determine if something is state?

``` text
1. Is it passed in from a parent via props? If so, it probably isn’t state.
2. Does it remain unchanged over time? If so, it probably isn’t state.
3. Can you compute it based on any other state or props in your component? If so, it isn’t state.
```

5.How can you identify where state needs to live?

```text
1. ProductTable needs to filter the product list based on state and SearchBar needs to display the search text and checked state.
2. The common owner component is `FilterableProductTable`.
3. It conceptually makes sense for the filter text and checked value to live in `FilterableProductTable`
```

## Higher-order functions

* What is a “higher-order function”?
*Functions that operate on other functions, either by taking them as arguments or by returning them, are called higher-order functions.*
* Explore the `greaterThan` function as defined in the reading. In your own words, what is line 2 of this function doing?
*this function is doing another function with it, its areturn to the value which in this case is n*
* Explain how either `map` or `reduce` operates, with regards to higher-order functions.
*Reduce is the higher-order operator that reflects this pattern (sometimes also called fold). It creates a value by mixing a single member from the array with the current value over and over again. When summing numbers, start with zero and add each element to the total.
Aside from the array, the arguments to reduce are a combining function and a start value. This function is a little more complicated than filtering and mapping.*

## Things I want to know more about

* more about react and other library
* know more about componants
