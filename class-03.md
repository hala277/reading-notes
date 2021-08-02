# *HTML Lists, Control Flow with JS, and the CSS Box Model*

**Entry:** *we will talk about Lists in html and how to creat them then we will talk about boxes in css and how to creat them and how many way we can make a box throw it ,then we will get to know what is the array and how to declar in js ,and in the end we will get to know loops and see how many common types of it*


### *Lists*

#### *Html provides three different types of lists:*

1. **Ordered lists:** 
*These are lists in which each item is numbered. The list might be a collection of stages in a recipe that must be completed in a specific sequence, or a formal contract with each point marked by a section number.*

*we can creat order list throw `<ol>`, Each item in the list is placed  between an opening `<li>` tag  and a closing `</li>` tag. (The li  stands for list item.)*


2. **Unordered lists:** 
*these are lists that start with a bullet point (rather than characters that indicate order).*

*we creat Unordered lists with `<ul>`,Each item in the list is placed  between an opening `<li>` tag and a closing `</li>` tag. (The li  stands for list item.)*

3. **Definition lists:** 
*a collection of words with meanings for each of them.*

*The definition list is created with  the `<dl>` element and usually  consists of a series of terms and  their definitions.Inside the `<dl>` element usually see pairs of `<dt>`This is used to contain the term  being defined (the definition  term), `<dd>` is used to contain the  definition.*

#### *nested Lists*
*we can put a second list inside an <li> element to create a sublist or nested list.*

**Example**
>`<ul>`
>
>   `<li>` Home
>
>    `<ul>`
>
>    `<li>` profil `</li>`
>
>   `</ul>`
>
>    `</li>`
>
>`</ul>`  

#### *Conclusion*
 *here are three types of HTML lists: ordered,  unordered, and definition.Ordered lists use numbers.Unordered lists use bullets. Definition lists are used to define terminology. Lists can be nested inside one another.*

 ## *Boxes*
 **CSS treats each HTML  element as if it lives in its own box.**

 *we can set several properties that affect the appearance of  these boxes, like:*
* Control the dimensions of  boxes
*  Create borders around boxes
* Set margins and padding for boxes
* Show and hide boxes

#### Box Dimensions(width, height)
*By default a box is sized just big  enough to hold its contents. To  set your own dimensions for a  box you can use the height and width properties.The most popular ways to  specify the size of a box are to use pixels percentages, or  ems. Traditionally, pixels have  been the most popular method  because they allow designers to  accurately control their size.*

**Example**
```
 div.box {
height: 100px;
 width: 100px;
 background-color: #bbbbaa;}
p {
 height: 75%;
 width: 75%;
 background-color: #0088dd;}
```

#### limiting Width(min-width, max-width)
*Some page designs adapt to the size of the user's screen by expanding and contracting. When the browser window is narrow, the min-width property provides the smallest size a box may be displayed at, while the max-width property gives the greatest width a box can expand to when the browser window is broad.*

**Example**
```
td.description {
 min-width: 450px;
 max-width: 650px;
 text-align: left;
 padding: 5px;
 margin: 0px;}

```

#### limiting height(min-height, max-height)
*the way that you might  want to limit the width of a box  on a page, you may also want to limit the height of it. This is achieved using the min-height  and max-height properties.*

**Example**
```
h2, p {
 width: 400px;
 font-size: 90%;
 line-height: 1.2em;}
h2 {
 color: #0088dd;
 border-bottom: 1px solid #0088dd;}
p {
 min-height: 10px;
 max-height: 30px;}

```
#### overfloWing content(overflow)
*If the content contained within a box is bigger than the box itself, the overflow property informs the browser what to do. It can be one of two types of values:*
1. **hidden:**
*This property simply hides any additional information that does not fit within the box.*

2. **scroll:** 
*This property adds a scrollbar to the box, allowing users to scroll to view what's missing.*

**code Example**
```
p.one {
 overflow: hidden;}
p.two {
 overflow: scroll;}

```
### BorDer, mArgin  & PADDing
*Every box has three available properties that  can be adjusted to control its appearance:*
1. **Border**
*Every box has a border (even if it is not visible or is specified to  be 0 pixels wide).The border  separates the edge of one box  from another.*
2. **Margin**
*Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.*
3. **Padding**
*Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.*

### White sPAce & verticAl mArgin
*The padding and margin properties are very helpful in adding space  between various items on the page.*

### Border Width
*The border-width property is used to control the width of a border. The value of this  property can either be given in pixels or using one of the  following values:*
`thin` `medium` `thick`
**You cannot use percentages  with this property.**
*You can control the individual  size of borders using four separate properties:*
* `border-top-width`
* `border-right-width`
* `border-bottom-width`
* `border-left-width`
*You can also specify different widths for the four border values in one property, like so:*
`border-width: 2px 1px 1px  2px;`

### Border style(border-style)
*You can control the style of a border using the `border-style`property. This property can take the following values:*

* `solid` *a single solid line*

* `dotted` *a series of square dots(if your border is 2px wide, then the dots are 2px squared with a 2px gap between each dot)*

* `dashed` *a series of short lines*

* `double` *two solid lines (the value of the border-width 
property creates the sum of the two lines)*

* `groove` *appears to be carved into the page*

* `ridge` *appears to stick out from the page*

* `inset` *appears embedded into the page*

* `outset` *looks like it is coming out of the screen*

* `hidden` / `none` *no border is shown*

**we can individually change the  styles of different borders using:**
* `border-top-style`
* `border-left-style` 
* `border-right-style`
* `border-bottom-style`

**conclusion:**
*CSS treats each HTML element as if it has its own box.You can use CSS to control the dimensions of a box.You can also control the borders, margin and padding for each box with CSS.It is possible to hide elements using the display and visibility properties.Block-level boxes can be made into inline boxes,and inline boxes made into block-level boxes.Legibility can be improved by controlling the width of boxes containing text and the leading.SS3 has introduced the ability to create image  borders and rounded borders*

## Basic JavaScript Instructions
### Arrays:
*An array is a special type of variable. It doesn't just store one value; it stores a list of values .*

#### when we can use the array?
*we use an array whenever we are working with a list or a set of values that are related to each other,Its also helpful when we do not know how many items a list will contain because, when we create the array, we do not need to specify how many values it will hold.*

### CREATING AN ARRAY
*create an array and give it a name just like other variable(using the `var` keyword followed by the name of the array).*

**array literal** *It is usually the preferred  method for creating an array. we can also write each value on a separate line:* 
```
colors= ['white', 'black', 'custom']; 
```
**array constructor** *This uses the new keyword followed by `Array();`The values are then specified in parentheses (not square brackets), and each value is separated by a comma. You can also use a method called `item()` to retrieve data from the array.*

### VALUES IN ARRAYS 
*Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).*

**Example how its start from zero not one**
INDEX |  Value
------|--------
0  | 'A'
1  | 'B'
2  | 'C'

 ## Decisions and Loops

 ### SWITCH STATEMENTS
*A switch statement tarts with a variable called the switch value.  Each case indicates a possible  value for this variable and the code that should run if the variable matches that value.*

**IF else vs. switch

if else | switch
--------|--------
*There is no need to provide an el se option. (You can just use an if statement.)| You have a default option that is run if none of the cases match. 
With a series of if statements, they are all checked even if a match has been found (so it performs more slowly than switch).|If a match is found, that code is run; then the break statement stops the rest of  the switch statement running (providing  better performance than multiple if statements). 
-------------------------------------------------------

### loops
*Loops check a condition. If it returns true, a code block will run. Then the condition will be checked again and if it still returns true, the code block will run again. It repeats until the condition returns false. There are three common types of loops:*

 * **For**
 *If you need to run code a specific number of times, use a for loop. (It is the most common loop.) In a for loop, the condition is usually a counter which is used to tell how many times the loop should run.*

 * **WHILE**
*If you do not know how many times the code should run, you can use a whi le loop. Here the condition can be something other than a counter, and the code will continue to loop for as long as the condition is true.*

* **DO WHILE** 
*The do...while loop is very similar to the while loop, but has one key difference: it will always run the statements inside the curly braces at least once, even if the condition evaluates to false*

### loop counters
```
`for`(var i =0; i<5; i++)
`document.write(i);`
```
**conclusion** *Conditional statements allow your code to make  decisions about what to do next. Comparison operators `(===, ! ==, ==, ! =, <, >, <=, =>)`  are used to compare two operands. Logical operators allow you to combine more than one  set of comparison operators. if ... else statements allow you to run one set of code  if a condition is true, and another if it is false. switch statements allow you to compare a value  against possible outcomes (and also provides a default  option if none match). Data types can be coerced from one type to another.  All values evaluate to either truthy or false. There are three types of loop: for, while, and do ... while. Each repeats a set of statements.* 



