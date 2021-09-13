# State and Props

1. Based off the diagram, what happens first, the `‘render’` or the `‘componentDidMount’`?
*First the `render` then the `componentDidMount`*
2. What is the very first thing to happen in the lifecycle of React?
*Mounting When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. static getDerivedStateFromProps() The static getDerivedStateFromProps is the first React lifecycle method to be invoked during the updating phase, `render`, `componentDidMount`, and `UNSAFE_componentWillMount` all occur in this order during mounting.*
3. *Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`,`componentWillUnmount`, `React Updates`*

*1. constructor*
*2. render*
*3. componentDidMount*
*4. React Updates*
*5. componentWillUnmount*
4. What does componentDidMount do?
*This method allows you to clean up the DOM and netwrok requests/ subscriptions.The `componentDidMount()` method allows us to execute the React code when the component is already placed in the DOM (`Document Object Model`). This method is called during the `Mounting` phase of the `React Life-cycle` after the component is `rendered`.*

## React State Vs Props

1. What types of things can you pass in the props?
*pass a counter component its initial count inside of the props ,display something to the user that has a title and a subtitle you're going toalso store that in the props case our component is storing a title and a subtitle so we're passing those through the props*
2. What is the big difference between props and state?
*props you pass into acomponent and state is handled inside of that component and props are handledoutside of the component*
3. When do we re-render our application?
*when you change the state inside of your application it's going to re-render that section of your application*
4. What are some examples of things that we could store in state?
*have an input element check box select a box whatever it is that needs to be able to be updated by the user so we're going to actually use state to store*  

## Things I want to know more about

1. Handling Events
2. Conditional Rendering
3. forms.  
