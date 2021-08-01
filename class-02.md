# *Readings : Basics of HTML, CSS & JS*

## *Text*

### *we will start with the most use tags in the text in HTML*

1. #### *Headings*
*HTML have six "levels" of  headings:*

> `<h1>` is used for main headings
> `<h2>` is used for subheadings

`<h1>`
`<h2>`
`<h3>`
`<h4>`
`<h5>`
`<h6>`

> `<h1>` the most important,`<h6>` the least important

2. #### *Paragraphs*
`<p>` *To build a paragraph, use an initial `<p>` tag and a closing `</p>` tag to enclose the words that make up the paragraph. A browser will display each paragraph on a separate line with some space between it and any future paragraphs by default.*

3. #### *Bold & italic*
`<b>`*We may make characters look bold by surrounding words in the tags `<b>` and `</b>`. Although the usage of the `<b>` element does not suggest any additional meaning, it does signify a portion of text that would be presented in a visually distinct fashion (for example, crucial words in a paragraph).*

`<i>` *We may make characters look italic by surrounding words in the tags `<i>` and `</i>`. The `<i>`element also denotes a portion of text that is stated differently than the surrounding information, such as technical terminology, ship names, foreign language, thoughts, or other terms that are normally italicized.*

4. #### *superscript & article subscript*
`<sup>` *The `<sup>` element is used to include letters that should be superscripted, such as date suffixes or mathematical ideas like increasing a number to a power of 22, for example.*

`<sub>` *Characters that should be subscripted are placed in the `<sub>` element. It is commonly used with foot notes or chemical  formulas such as H2O.*

5. #### *line Breaks & article Horizontal rules*
`<br/>` *Each new paragraph or header will be displayed on a new line by the browser. However, you may use the line break tag `<br/>` to insert a line break in the midst of a paragraph.*

`<hr/>` *The `<hr/>` element can be used to add a horizontal rule between sections to make a break between topics, such as a change of topic in a book or a new scene in a play.*


**Visual editors often resemble  word processors. Although  each editor will differ slightly,  there are some features that  are common to most editors  that allow you to control the  presentation of text.**

* Headings are created by highlighting text then using  a drop-down box to select a  heading.
* Bold and italic text are created by highlighting some  text and pressing a b or i  button.
* New paragraphs are created using the return or the enter  key.
* Line breaks are created by pressing the shift key and the  return key at the same time.
* Horizontal rules are created using a button with a straight  line on it.


6. #### *semantic markup*
*Semantic markup refers to text components that aren't meant to change the structure of your web pages but do provide more information to them.*

**Why using semantic markup is important :**
![img of semantic markup](http://brevity.temp927.kinsta.cloud/wp-content/uploads/2017/08/semantic-fb.jpg)

7. #### *strong & emphasis*
`<strong>` *The usage of the `<strong>` element denotes that the material is extremely important. The words in this portion, for example, might be stated with a lot of emphasis. Browsers display the contents of a `<strong>` element as bold by default.*

`<em>` *The `<em>` element denotes emphasis, which modifies the meaning of a text subtly. The contents of an `<em>` element are italicized by default in browsers.*

8. #### *Quotations*
**There are two elements commonly used for marking up  quotations:**

`<blockquote>` *For larger quotations that take up a full paragraph, the `<blockquote>` element is utilized. It's worth noting that the `<p>` element is still utilized within the `<blockquote>` element. The contents of the `<blockquote>` element are indented by default in browsers; however, you should not use this element to indent a piece of text; instead, you should use CSS.*

`<q>` *For shorter quotations that fit within a paragraph, the `<q>` element is used. Although browsers are meant to place quotations around the `<q>` element, Internet Explorer does not, and as a result, many users avoid using it. The citation property may be used on both components to identify the source of the quote. Its value should be a URL that contains further information about the quotation's source.*

9. #### *abbreviations &  acronyms*

`<abbr>`
If you use an abbreviation or an acronym, then the <abbr>  element can be used. A title  attribute on the opening tag is  used to specify the full term.

10. #### *citations &definitions*
`<cite>`
When you are referencing a piece of work such as a book, film or research paper, the  
<cite> element can be used to indicate where the citation is from.

`<dfn>`
The first time you explain some new terminology (perhaps an  academic concept or some 
jargon) in a document, it is known as the defining instance of it.

11. #### *author details*
`<address>`
The <address> element has  quite a specific use: to contain  contact details for the author of  the page. It can contain a physical address,  but it does not have to. For  example, it may also contain a  phone number or email address. Browsers often display the  content of the <address>  element in italics.

12. #### *changes To content*
`<ins>` `<del>`
The <ins> element can be used to show content that has been  inserted into a document, while 
the <del> element can show text  that has been deleted from it. The content of a <ins> element 
is usually underlined, while the  content of a <del> element usually has a line through it.

`<s>`
The <s> element indicates  something that is no longer accurate or relevant (but that 
should not be deleted).Visually the content of an <s>  element will usually be displayed  with a line through the center.

### *As a conclusion :*

#### *What is the use of HTML elements ?*
*HTML elements are used to describe the structure of  the page ( headings, subheadings, paragraphs).They also provide semantic information ( where  emphasis should be placed, the definition of any  acronyms used, when given text is a quotation).*


## *Introducing CSS:*
**You will use CSS to establish rules that control how each individual box (and the contents of that box) is displayed.**

### *Style rules are associated with htML elements in CSS:*
*CSS associates rules with HTML elements to make it function. The content of specified elements is displayed according to these criteria. A selector and a declaration are the two pieces of a CSS rule.*

**Example:**
![style examle](https://slidetodoc.com/presentation_image_h2/717065bd9017f07b3ab23f9891865ee8/image-6.jpg)

### *The following CSS attributes have an impact on how items are displayed:*
*CSS declarations are contained within curly brackets and consist of two parts: a property and a value separated by a colon. Several properties can be specified in a single declaration, each separated by a semi-colon.*

**Example:**
![css example](https://slideplayer.com/slide/13771255/85/images/9/CSS+PROPERTIES+AFFECT+HOW+ELEMENTS+ARE+DISPLAYED.jpg)

### *using external CSS*
`<link>` *In an HTML document, the `<link>` element can be used to notify the browser where to find the CSS file that will be used to design the page. It sits within the `<head>` element and is an empty element (meaning it doesn't need a closing tag). It should have three characteristics:*

* `href`
*The path to the CSS file is specified here (which is often placed in a folder called css or styles).*

* `type`
*The type of document being linked to is specified by this property. Text/css should be the value.*

* `rel`
*This describes the connection between the HTML page and the file to which it is linked. When connecting to a CSS file, the value should be stylesheet.*

### *using Internal CSS*
`<style>`
*CSS rules may also be included in an HTML page by putting them in the `<style>` element, which is generally found in the page's `<head>` element. The type property should be used on the `<style>` element to indicate that the styles are defined in CSS. `Text/css` should be the value.*

#### *Why You should utilize an external CSS style sheet when creating a site with more than one page?* 

1. Enables the usage of the same style standards across all pages (rather than repeating them in each page).
2. Separates the information from the appearance of the page.
3. It means you may modify the styles used on all pages by changing only one file (rather than each one separately).

### *As a conclusion :*
*CSS handles each HTML element as though it were contained within its own box, and utilizes rules to specify how it should appear. Selectors (which describe which items the rule applies to) and declarations make up rules (that indicate what these elements should look like). You may target your rules to various components using different sorts of selectors. The properties of the element you intend to alter, as well as the values of those properties, make up declarations. The font-family attribute, for example, defines the font to be used, while the value arial provides Arial as the preferred typeface. CSS rules are generally found in a distinct document, however they can also be included within a document.*

## *Basic JavaScript Instructions*
### *VARIABLES: HOW TO DECLARE THEM*
*Before  use a variable, we need to announce that you want to use it. This involves creating the variable and giving it a name. Programmers say that you declare the variable.*

**Example**
>`var name ;`

### *VARIABLES: HOW TO ASSIGN THEM A VALUE*
*Once you have created a variable you can tell it what information you would like it to store for you. Programmers say that you assign a value to the variable.*

**Example**
>`var name = "hala";`


### *As a conclusion :*
*A script consists of a set of statements. Each statement functions similarly to a step in a recipe. The directions in scripts are quite specific. You might, for example, require that a value be remembered  before doing a computation with it. Variables are used to store data that is utilized in the script on a temporary basis. Arrays are a particular sort of variable that may hold many pieces of linked data.Numbers (0-9) are distinguished from strings (text) and Boolean values in JavaScript (true or false). Expressions return a single value when evaluated.To compute a value, expressions use operators.*

## *Decisions and Loops*
### *DECISION MAKING*
*There are often several places in a script where decisions are made that determine which lines Of code should be run next. Flowcharts can help you plan for these occasions.*

![DECISION MAKING](https://static.javatpoint.com/tutorial/es6/images/es6-decision-making.png)

### *EVALUATING CONDITIONS & CONDITIONAL STATEMENTS*
**There are two components to a decision:**
1.  An expression is evaluated, which returns a value 
2.  A conditional statement says what to do in a given situation 

![CONDITIONAL STATEMENTS](https://www.tutorialspoint.com/perl/images/decision_making.jpg)

### *COMPARISON OPERATORS: EVALUATING CONDITIONS*
![EVALUATING CONDITIONS](https://i.ytimg.com/vi/wFB-ywsNPwg/maxresdefault.jpg)

### *LOGICAL OPERATORS*
![LOGICAL OPERATORS ](https://www.devopsschool.com/blog/wp-content/uploads/2020/07/JavaScript-Logical-Operator.png)

### *IF STATEMENTS*
![IF STATEMENTS ](https://cdn.programiz.com/sites/tutorial2program/files/js-if-statement_0.png)

### *IF ELSE STATEMENTS*
![IF ELSE STATEMENTS](https://cdn.programiz.com/sites/tutorial2program/files/js-if-else-statement.png)

### *SWITCH STATEMENTS*
![SWITCH STATEMENTS](https://images.slideplayer.com/19/5803798/slides/slide_2.jpg)

![SWITCH STATEMENTS2](https://cdn.programiz.com/sites/tutorial2program/files/javascript-switch-statement.png)








