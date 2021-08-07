# Problem Domain, Objects, and the DOM

## Understanding The Problem Domain Is The Hardest Part Of Programming

### Why problem domains are hard ?

*Writing code is a lot like putting together a jigsaw puzzle. We put together code with the purpose of building components that we have taken out of the «bigger picture» of the problem domain.The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all.The real world is a messy place. Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint.*

## Programming is easy if you understand the problem domain

 *the waterfall approach and the extreme amount of specification that was done before anything was built—it was very easy to write the code for a feature.writing a tab control for the user interface of a printer and having the complete pixel perfect specs handed  before  began to write any code. also given all the possible use cases and told exactly how it should function and what it should do under just about every circumstance.*

*how easy it was to write the code to produce this tab control? Super easy.*

*When you essentially given the entire problem domain in the form of a spec that was clear and unambiguous. you will be easily able to learn that problem domain and because of it, you will be able to write the code very easily .Perhaps you have had a similar experience, not necessarily working on a waterfall project where you were given the spec, but perhaps on an Agile project where you took the time to clearly understand the problem domain before writing any code.*

**You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.**

*What I mean by this is that it is often beneficial to take a part of the problem and fully understand that part before expanding the problem domain.Games are really good at this. Look at most games today and you’ll find that you start with a very small problem domain. The first level is usually a tutorial that has a basic set of things you can do so that you don’t get overwhelmed. But, as you advance through the levels, you usually find they get harder and introduce new concepts that build gradually on what you know, until you understand a pretty large problem domain.The other choice is to become better at understanding problem domains. As developers, we tend to think that sitting down and talking to customers or business people who know about the problem domain is a waste of time.*


## Object Literals
*Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object,  variables and functions take on new names.*

+ IN AN OBJECT: VARIABLES BECOME  KNOWN AS PROPERTIES :
*If a variable is part of an object, it's called a property. Properties tell us about the object, such as  the name of a hotel or the number of rooms it has.*

+ IN AN OBJECT: FUNCTIONS BECOME  KNOWN AS METHODS:
*If a function is part of an object, it is called a method. Methods represent tasks that are associated with the object.*

+ *Like variables and named functions, properties and methods have a name and a value. In an object, that name is called a* **key.** 

+ *An object **cannot have two keys with the same name**. This is because keys are used to access their corresponding values.*

+ *The value of a property can be a **string, number, Boolean, array, or even another object**. The value of a method is always a **function**.*

### Programmers use a lot of name/value pairs: 
+ HTML uses attribute names and values. 
+ CSS uses property names and values. 

### In JavaScript: 
+ Variables have a name and you can assign them a value of a string, number, or Boolean. 
+ Arrays have a name and a group of values. ( Each item in an array is a name/value pair because it has an index number and a value.) 
+ Named functions have a name and value that is a set of statements to run if the function is called. 
+ Objects consist of a set of name/value pairs (but the names are referred to as keys). 

### CREATING AN OBJECT: LITERAL NOTATION 
*Literal notation is the easiest and most popular way to create objects.* 

+ The object is the curly braces and their contents. The object is stored in a variable called hotel, so you would refer to it as the hotel object. 

+ Separate each key from its value using a colon. Separate each property and method with a comma (but not after the last value). 

### ACCESSING AN OBJECT AND DOT NOTATION 
*You access the properties or methods of an object using dot notation. You can also access properties using square brackets.*

+ To access a property or method Of an Object you use the name of the object, followed by a period, then the name of the property or method you want to access. This is known as dot notation. 

+ The period is known as the member operator. The property or method on its right is a member of the object on its left. Here, two variables are created to hold the hotel name and number of vacant rooms.

+ You can also access the properties of an object (but not its methods) using square bracket syntax. 


+ This time the object name is followed by square brackets, and the property name is inside them. 

`var hotelName = hotel [' name ']; `

**This notation is used most commonly when:** 
+ The name of the property is a number (technically allowed, but should generally be avoided) 
+  A variable is being used in place of the property name .

## Document Object Model
*The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.*

### CACHING DOM QUERIES 

*Methods that find elements in the DOM tree are called DOM queries. When you need to work with an element more than once, you should use a variable to store the result Of this query.When a script selects an element to access or update, the interpreter must find the elements in the DOM tree.Once it has found the node that represents the element(s), you can work with that node, its parent, or any children.*

![Dom tree](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/DOM-model.svg/1200px-DOM-model.svg.png)

*When people talk about storing elements in variables, they are really storing the location of the element(s) within the DOM tree in a variable. The properties and methods of that element node work on the variable.*

### METHODS THAT SELECT INDIVIDUAL ELEMENTS 
*`getE1ementById()` and `querySe1ector()` can both search an entire document and return individual elements. Both use a similar syntax.*

+ `getE1ementByld()` is the quickest and most efficient way to access an element because no two elements can share the same value for their id attribute.

+ `querySe1ector()` is a more recent addition to the DOM, so it is not supported in older browsers. But it is very flexible because its parameter is a CSS selector, which means it can be used to accurately target many more elements. 

### SELECTING AN ELEMENT FROM A NODELIST 
**There are two ways to select an element from a NodeList:** 
+ The item() method 
+ array syntax. 

**Both require the index number of the element you want.** 

1.  THE item() METHOD 
*NodeLists have a method called item() which will return an individual node from the NodeList. You specify the index number of the element you want as a parameter of the method (inside the parentheses).*

2. Array syntax
*Array syntax is preferred over the item() method because it is faster. Before selecting a node from a NodeList, check that it contains nodes. If you repeatedly use the NodeList, store it in a variable.*

### REPEATING ACTIONS FOR AN ENTIRE NODELIST 
*When you have a NodeList, you can loop through each node in the collection and apply the same statements to each.*

### ADDING OR REMOVING HTML CONTENT 
*There are two very different approaches to adding and removing content from a DOM tree: the innerHTML property and DOM manipulation.*

1. THE innerHTML PROPERTY
+ APPROACH 
*innerHTML can be used on any element node. It is used both to retrieve and replace content. To update an element, new content is provided as a string. It can contain markup for descendant elements.*

+ ADDING CONTENT 
To add new content: 
1. Store new content (including markup) as a string in a variable. 
2. Select the element whose content you want to replace. 
3. Set the element's innerHTML property to be the new String. 


+ REMOVING CONTENT 
*To remove all content from an element, you set innerHTML to an empty String. TO remove one element from a DOM fragment, one `<li>` from a `<ul>` you need to provide the entire fragment minus that element.*

2. DOM manipulation
*DOM manipulation easily targets individual nodes in the DOM tree, whereas innerHTML is better suited to updating entire fragments.* 


+ APPROACH 
*DOM manipulation refers to a set of DOM methods that allow you to create element and text nodes, and then attach them to the DOM tree or remove them from the DOM tree.*


+ ADDING CONTENT 
*To add content, you use a DOM method to create new content one node at a time and store it in a variable. Then another DOM method is used to attach it to the right place in the DOM tree.*


+ REMOVING CONTENT 
*You can remove an element (along with any contents and child elements it may contain) from the DOM tree using a single method.*

### Conclusion:
*The browser represents the page using a DOM tree. DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes. You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax. Whenever a DOM query can return more than one node, it will always return a NodeLi st. From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques. An element node can contain multiple text nodes and child elements that are siblings of each other. In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery). Browsers offer tools for viewing the DOM tree.* 



























