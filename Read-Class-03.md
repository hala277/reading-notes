# Passing Functions as Props

## React Docs - lists and keys

1. What does .map() return?
*array, We assign the new array returned by map()*
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
*we loop through the numbers array using the JavaScript `map()` function. We return a `<li>` element for each item. Finally, we assign the resulting array of elements to `listItems`,We include the entire `listItems` array inside a `<ul>` element, and render it to the `DOM`*
[codeExample](https://codepen.io/gaearon/pen/GjPyQr?editors=0011)
3. Each list item needs a unique __keys__.
4. What is the purpose of a key?
*Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity*  

----------------

## The Spread Operator

**1. What is the spread operator?**
*JavaScript, spread syntax refers to the use of an ellipsis of three dots `(…)` to expand an iterable object into the list of arguments.*

**2.List 4 things that the spread operator can do.**

- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments

**3.Give an example of using the spread operator to combine two arrays.**
*the spread operator can quickly combine two arrays, an operation known as array concatenation*

``` javascript

const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
```

[code refrence](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

**4. Give an example of using the spread operator to add a new item to an array.**

``` javascript
const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]
```

[code refrence](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

**5.Give an example of using the spread operator to combine two objects into one.**

``` javascript
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂
```

[code refrence](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

## How to Pass Functions Between Components

1. In the video, what is the first step that the developer does to pass functions between components?
*create the function wherever the state is that we're going to change `increment`*
2. In your own words, what does the increment function do?
*its a function that locks to find a match on the name and if it found the name it will increment and add it to the count*
3. How can you pass a method from a parent component into a child component?
*when the person clicks the button that's inside of person we call the increment method using props*
4. How does the child component invoke a method that was passed to it from a parent component?
*through this.props*

## Things I want to know more about

1. *`map()`*
2. *props*
3. *more about lists and keys*
