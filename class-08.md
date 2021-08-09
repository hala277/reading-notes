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
```

**containing Elements**
 
*If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element. It is common to group a number of elements together inside a `<div>` (or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The `<div>` element that contains this group of elements is then referred to as the containing element.*

*A box may be nested inside several other block-level elements. The containing element is always the direct parent of that element.*

**Controlling the  position of elements**
*CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute  positioning. You specify the positioning scheme using the position  property in CSS. You can also float elements using the float property.*

![position of elements](https://www.internetingishard.com/html-and-css/advanced-positioning/css-positioning-schemes-790d5b.png)
