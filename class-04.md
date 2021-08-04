# HTML Links, JS Functions, and Intro to CSS Layout

**intro:** *we will talk about links in html and then we will get to know layout and the layout of a page: normal flow, relative positioning, and absolute  positioning.after that we will get to know What Is a Function and how to Declaring  and at the end we will discuse what are the 6 Reasons for Pair Programming*

## links
*Links are the defining feature of the web  because they allow you to move from  one web page to another enabling the  very idea of browsing or surfing.*

  **links types:**
1.  Links from one website to another.
2.  Links from one page to another on the same website.
3. Links from one part of a web page to another part of the same page.
4.  Links that open in a new browser window.
5. Links that start up your email program and address a new email to someone.

**Writing Links:**
*links are created using the `<a>` element. Users can click on anything  between the opening `<a>` tag and the closing `</a>` tag. You specify  which page you want to link to using the `href` attribute.The text between the opening `<a>` tag and closing `</a>` tag  is known as link text. Where  possible, your link text should  explain where visitors will be  taken if they click on it.*

+ **Linking to other sites code example:**
```
<p> Movie Reviews:
 <ul>
  <li><a href="http://www.empireonli.co">
    Empire</a></li>
  <li><a href="http://www.metacrit.co">
    Metacritic</a></li>
  <li><a href="http://www.rottentomato.co">
    Rotten Tomatoes</a></li>
  <li><a href="http://www.varie.c">
    Variety</a></li>  </ul>
</p>
```
+ **Linking to other Pages on the same site code example:**

```
<p>
 <ul>
  <li><a href="index.html">Home</a></li>
  <li><a href="about-us.html">About</a></li>
  <li><a href="movies.html">Movies</a></li>
  <li><a href="contact.html">Contact</a></li>
 </ul>
</p>

```
**email Links:**
*To create a link that starts up  the user's email program and  addresses an email to a specified  email address, you use the `<a>`  element. However, this time the  value of the `href` attribute starts  with mailto: and is followed by  the email address you want the  email to be sent to.*

**Code example:**

```
<a href="mailto:hala@example.org">Email hala</a>
```

**opening Links in a new Window:**

*`target` If you want a link to open in a new window, you can use the target attribute on the opening `<a>` tag. The value of this attribute should be _blank.* 

Code example:
```
<a href="http://www..imdb.co" target="_blank">Internet Movie Database</a> (opens in new window)

```
*To link specific  Part of the same Page do  this using the id attribute (which  can be used on every HTML  element). The value of the id attribute  should start with a letter or an  underscore (not a number or  any other character) and, on a  single page, no two id attributes  should have the same value.*

**Conclusion:**
*links are created using the `<a>` element. The `<a>` element uses the` href` attribute to indicate  the page you are linking to. If you are linking to a page within your own site, it is  best to use relative links rather than qualified URLs. You can create links to open email programs with an email address in the "to" field. You can use the id attribute to target elements within  a page that can be linked to.*

## Layout
**Key Concepts in  positioning elements**

**Building Blocks:**
*CSS treats each HTML element as if it is in its  own box. This box will either be a block-level  box or an inline box.*

*Block-level boxes start on a new line and act as the main building blocks  of any layout, while inline boxes flow between surrounding text. You can  control how much space each box takes up by setting the width of the  boxes (and sometimes the height, too). To separate boxes, you can use  borders, margins, padding, and background colors.*

+ *Block-level elements start on a new line*

**Examples code:**
```
<h1> <p> <ul> <li>
```

+ *inline elements flow in Between surrounding text*


**Examples code:**
```
<img> <b> <i>
````
**containing Elements**
 
*If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element. It is common to group a number of elements together inside a `<div>` (or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The `<div>` element that contains this group of elements is then referred to as the containing element.*

*A box may be nested inside several other block-level elements. The containing element is always the direct parent of that element.*

**Controlling the  position of elements**
*CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute  positioning. You specify the positioning scheme using the position  property in CSS. You can also float elements using the float property.*

![position of elements](https://www.internetingishard.com/html-and-css/advanced-positioning/css-positioning-schemes-790d5b.png)


## js Functions, Methods, and Objects
**WHAT IS A FUNCTION?**

*Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).*

**HOW TO DECLARING A FUNCTION**

*To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces. This is known as a function declaration.* 

```
function sayHello() { 
document . write( Hello); 
```

**HOW TO CALLING A FUNCTION**

*Having declared the function, you can then execute all of the statements between its curly braces with just one line of code. This is known as calling the function.*

```
sayHello();
```

**HOW TO DECLARING FUNCTIONS THAT NEED INFORMATION**

*Sometimes a function needs specific information to perform its task. In such cases, when you declare the function you give it parameters. Inside the function, the parameters act like variables.*
```
function getArea(width, height) { 
return width * height; 
}

```
**HOW TO CALL FUNCTIONS THAT NEED INFORMATION**

*When you call a function that has parameters, you specify the values it should use in the parentheses that follow its name. The values are called arguments, and they can be provided as values or as variables.* 


+  **ARGUMENTS AS VALUES**
*When the function below is called, the number 7 will be used for the width of the wall, and 7 will be used for its height.* 
```
getArea(7, 7); 
```

+ **ARGUMENTS AS VARIABLES** 
*You do not have to specify actual values when calling a function ,you can use variables in their place. So the following does the same thing.*

```
wallWidth = 7; 
wallHeight = 7;
getArea (wallWidth , wallHeight); 
```
**HOW TO GET A SINGLE VALUE OUT OF A FUNCTION**

*Some functions return information to the code that called them. For example, when they perform a calculation, they return the result.*

```
function calculateArea(width, height) { 
var area = width * height; 
return area; 
}
var wallOne = calculateArea(3,7); 
var wallTwo = calculateArea(8,7);
```
**HOW TO GET MULTIPLE VALUES OUT OF A FUNCTION**

*Functions can return more than one value using an array. For example, this function calculates the area and volume of a box.*

```
function getSize(width, height, depth) { 
var area = width * height; 
var volume = width * height * depth; 
var sizes = [area, volume] ; 
return sizes; 
}

var area0ne = getSize(3, 2, 3) [0]
var volume0ne = getSize(3, 2, 3) [1]
```
## 6 Reasons for Pair Programming
**How does pair programming work?**

*The Driver is the programmer who is typing and the only one whose hands are on the keyboard. While learning to code, developers likely study several programming languages.*

**Why pair program?**

*While learning to code, developers likely study several programming languages.Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.*

**Greater efficiency**

*When coming up with ideas and discussing solutions out loud, two programmers may come to a solution faster than one programmer on their own. Also, when the pair is stuck, both programmers can research the problem and reach a solution faster. Researches also identified pairing enhances technical skills, team communication, and even enjoyability of coding in the workplace.*

**Engaged collaboration**

*When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. We advise our students to spend no more than fifteen minutes stuck on a problem before asking a teaching assistant or instructor for help. When developers pair program, they rely more on each other and can often find a solution together without needing to ask for additional help.*

**Learning from fellow students**

*If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution. Often times, the developers in a pairing have different skill sets.*

**Social skills**

*Pair programming is great for improving social skills. Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills. As much as employers want strong programmers, they know it’s essential to hire people who can work well with others.*

**Job interview readiness**

*A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen.*








