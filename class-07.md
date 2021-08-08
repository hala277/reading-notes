# Object-Oriented Programming, HTML Tables
## Domain Modeling

*Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the variousentities,their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as anobject-oriented model.As a communication tool,it defines a vocabulary that can be used within and between both technical and business teams.*

## Create a constructor and set up the properties.
*You'll want to use a constructor function to declare the same attributes across several instances.*

**example on how to initialize a costructor :**
```
let functionName = function(a,b){
    this.a=a;
    this.b=b;
}

let callA=new functionName(a,b);
let callB=new functionName(a,b);

console.log(callA);
console.log(callB);

```
**This is the most basic level of object-oriented programming in JavaScript.**

1. The new keyword creates (or instantiates) an object.
2. The constructor function uses the this variable to initialize variables within the object.
3. The item is saved in a variable and will be used later.

*The process of developing a conceptual model for a given topic is known as domain modeling. And a well-articulated domain model can confirm and validate your knowledge of the problem.*

 **some pointers while creating domain models:**

1. Build self-contained objects with the same properties and behaviors when modeling a single entity that will have multiple instances.
2. A constructor function that specifies and initializes properties is used to model its characteristics.
3. Model its actions using simple methods that concentrate on a single task.
4. Use the new keyword followed by a call to a constructor function to create instances.
5. Save the newly formed object in a variable so that its attributes and methods may be accessed from the outside.
6. Use the this variable to access the object's attributes and methods from within methods.

## Tables
### What's  a Table?
*A table represents information in a grid format.  Examples of tables include financial reports, TV  schedules, and sports results.*

**basic Table structure**
`<table>`
*The `<table>` element is used to create a table. The contents  of the table are written out row  by row.*

`<tr>`
*You indicate the start of each  row using the opening `<tr>` tag.(The tr stands for table row.) It is followed by one or more `<td>` elements (one for each cell  in that row).*

`<td>`
*Each cell of a table is  represented using a `<td>`  element. (The td stands for  table data.)*

**Table headings**

`<th>`
*The `<th>` element is used just like the  `<td>` element but its  purpose is to represent the heading for either a column or a row. (The `th` stands for table  heading.) Even if a cell has no content, you should still use a `<td>` or `<th>` element to represent the presence of an empty cell  otherwise the table will not render correctly.*

**spanning columns**
*Sometimes you may need the  entries in a table to stretch  across more than one column. The `colspan` attribute can be  used on a `<th>` or `<td>` element  and indicates how many columns  that cell should run across.* 

**spanning rows**
*You may also need entries in a table to stretch down across more than one row. The `rowspan` attribute can be used on a `<th>` or `<td>` element to indicate how many rows a cell  should span down the table.*

### long Tables
*There are three elements that  help distinguish between the  main content of the table and  the first and last rows (which can  contain different content). These elements help people  who use screen readers and also  allow you to style these sections  in a different manner than the  rest of the table*

`<thead>`
*The headings of the table should  sit inside the `<thead>` element.* 

`<tbody>`
*The body should sit inside the `<tbody>` element.*

`<tfoot>`
*The footer belongs inside the `<tfoot>` element.*

## Functions, Methods, and Objects

### CREATING AN OBJECT: CONSTRUCTOR NOTATION 
*The new keyword and the object constructor create a blank object. You can then add properties and methods to the object.*
 

+ *First, you create a new object using a combination of the new keyword and the Object (constructor function, (This function is part of the JavaScript language and is used to create objects.)* 

+ *Next, having created the blank object, you can add properties and methods to it using dot notation. Each statement that adds a property or method should end with a semicolon.* 


### UPDATING AN OBJECT 
*To update the value of properties, use dot notation or square brackets. They work on objects created using literal or constructor notation. To delete a property, use the delete keyword.*


### CREATING MANY OBJECTS: CONSTRUCTOR NOTATION 
*Sometimes you will want several objects to represent similar things. Object constructors can use a function as a template for creating objects.* 
```
Function functionName(a,b,c){
Properties and method
}
```
*You create instances of the object using the constructor function. The new keyword followed by a call to the function creates a new object. The properties of each object are given as arguments to the function.*


### ARRAYS ARE OBJECTS 
*Arrays are actually a special type of object. They hold a related set of key/value pairs (like all objects), but the key for each value is its index number.* 


### ARRAYS OF OBJECTS & OBJECTS IN ARRAYS 
*You can combine arrays and objects to create complex data structures: Arrays can store a series of objects (and remember their order). Objects can also hold arrays (as values of their properties). In an object. the order in which the properties appear is not important. In an array, the index numbers dictate the order of the properties.* 


### THREE GROUPS OF BUILT-IN OBJECTS 

**USING BUILT-IN OBJECTS: **
*The three sets Of built-in objects each offer a different range Of tools that help you write scripts 
For web pages.* 


### BROWSER OBJECT MODEL 
*The Browser Object Model creates a model of the browser tab or window. The topmost Object is the Window object, which represents current browser window or tab. Its child objects represent other browser features.* 


### DOCUMENT OBJECT MODEL 
*The Document Object Model (DOM) creates a model of the current web page. The topmost Object is the document Object, which represents the page as a whole. Its child objects represent other items on the page.* 


### GLOBAL JAVASCRIPT OBJECTS 
*The global Objects do not form a single model. They are a group of individual objects that relate to different parts of the JavaScript language. The names of the global objects usually start with a capital letter, e.g., the String and Date objects.* 



### CREATING AN INSTANCE OF THE DATE OBJECT 
*In order to work with dates, you create an instance of the Date object. You can then specify the time and date that you want it to represent. To create a Date object, use the Date() object constructor. The syntax is the same for creating any object with a constructor function .By default, when you create a Date object it will hold today's date and the current time. If you want it to store another date, you must explicitly specify the date and time you want it to hold.*


**Conclusion :**

*Functions allow you to group a set of related statements together that represent a single task.Functions can take parameters (information required to do their job) and may return a value. An object is a series of variables and functions that represent something from the world around you. In an object, variables are known as properties of the object; functions are known as methods of the object, Web browsers implement objects that represent both the browser window and the document loaded into the browser window. JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts. Arrays and objects can be used to create complex data sets (and both can contain the other).*



