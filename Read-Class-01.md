
# Introduction to React and Components

## What is a component?

*A component is a well-defined collection of modular, portable, replaceable, and reusable functionality that wraps and exports its implementation as a higher-level interface.*

*A component is a software object that encapsulates specific functionality or a collection of functions and is designed to interact with other components. It has a well defined interface and follows a suggested behavior that other components in an architecture should follow.*

*Only a software component with a contractually stated interface and explicit context dependencies may be defined as a unit of composition. In other words, a software component can be deployed independently and is subject to third-party composition.*

------------------

## What are the charactistics of a component?

1. **Reusability**
*Components are often built to be utilized in a variety of settings and applications. Some components, on the other hand, may be tailored to a specific purpose.*
2. **Replaceable**
*Components can be swapped out for others that are comparable.*
3. **Not context specific**
*Components are built to work in a variety of settings and scenarios.*
4. **Extensible**
*A component can be expanded from other components to add additional functionality.*
5. **Encapsulated**
*A A component shows the interfaces that allow the caller to access its functionality, but it does not reveal any underlying processes, variables, or state*
6. **Independent**
*Components are meant to have as few dependencies as possible.*

------------------

## What are the advantages of using component based architecture?

1. Ease of deployment As new compatible versions become available, it becomes easier to update older versions without affecting other components or the system as a whole.

2. Lower costs Using third-party components helps you to stretch the expense of development and maintenance over a longer period of time.

3. Ease of development Components use well-known interfaces to offer specified functionality, letting developers to work on them without affecting other areas of the system.

4. Reusable Using reusable components allows you to divide the expense of creation and maintenance over several apps or systems.

5. Modification of technical complexity Through the usage of a component container and its services, a component can change the technical complexity.

6. Reliability The entire system's reliability improves when the reliability of each individual component improves the overall system's reliability via reuse.

7. System upkeep and evolution It's simple to update and alter the implementation without impacting the rest of the system.

8. Components are self-contained and connected in a flexible manner. Different groups create components independently and in simultaneously. Productivity in software development, both now and in the future.

 ------------------

## What is Props and How to Use it in React

## What is props short for?

*Props is a special keyword in React, which stands for properties and is being used for passing data from one component to another.*

## How are props used in React?

1. define an attribute and its `value(data)`
2. Then pass it to child component(s) by using Props
3. render the Props Data

## What is the flow of props?

*data with props are being passed in a uni-directional flow **one way from parent to child***

### How Does React Work and What Is It?

*React is a JavaScript framework for creating contemporary apps that was released by Facebook in 2013. React is a view layer framework that can be used to create both online and mobile apps.*

## These are the features that make the React library so good and powerful to build modern applications and what also makes React stand out against other frameworks and libraries

### **Virtual DOM**

*The most essential element of an online application is the DOM (Document Object Model), which describes the structure of a document web page, which is primarily HTML.Because modern apps demand a lot of state changes, animations, and effects, DOM manipulation is frequently utilized nowadays.*

*React makes use of virtual DOM, which is a virtual version of the real DOM tree. It's basically a memory-synchronized tree data structure of ordinary JavaScript objects. Because the virtual DOM will never be shown to the user and will only exist in memory, rendering it is quicker.*

### JSX

*React makes use of JSX, a JavaScript syntactic extension. It's what we utilize to make React "elements."Preprocessors (such as Babel) utilize JSX to convert HTML-like content in JavaScript files into parsable JavaScript objects.Although React does not need the usage of JSX, most developers find that it makes it easier to deal with the UI within the JavaScript code.We utilize JSX to construct React components, thus it's an important element of the React ecosystem.*

### Components

*React components are what separate our UI into distinct parts and make our code reusable.React components function in the same way as JavaScript functions do. A React component can take any number of props and should always return a React element that describes what should be displayed to the user.*

## Things I want to know more about

1. React vs. Angular, Vue and Other Frameworks
2. What Is React Native?
3. React Libraries
