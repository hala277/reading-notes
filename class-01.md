# *How the Web Works*

*The web server that hosts a website might be located anywhere in the world when you view it. Your browser will initially connect to a Domain Name System (DNS) server to determine the location of the web server.The browser in Cambridge first communicates with a DNS server in London. The DNS server then informs the browser of the location of the web server in Paris that is hosting the site.*

* You connect to the internet through an Internet Service Provider (ISP) (ISP). To access a website, you input the domain name or web address into your browser, such as google.com or facebook.com.

* Domain Name System (DNS) servers are a network of servers that your computer communicates with. These are similar to phone books in that they provide the IP address linked with the desired domain name to your computer. An IP address is a string of numbers separated by periods or full stops that can be up to 12 digits long. Every computer linked to the internet has a unique IP address, which functions similarly to a phone number.

* Your browser can contact the web server that hosts the webpage you requested using the unique number returned by the DNS server to your machine. A web server is a computer that is always connected to the internet and is configured to serve web pages to users.

* The web server then returns to your browser the page you requested.

## *How Pages use  Structure*

*Consider the stories you read in the newspaper: each one will have a title, some text, and sometimes some graphics. If the article is lengthy, there may be subheadings or quotations from individuals involved to break up the tale into sections. The newspaper's structure aids readers in comprehending the articles.When reading a news piece online, the format is fairly similar (although it may also feature audio or video). On the right, a copy of a newspaper is displayed with the equivalent item on the newspaper's website.*

## *Structuring word  documents*

*Word document structure In any text, the choice of headings and subheadings frequently indicates a hierarchy of information. A document may, for example, begin with a big header and then proceed to an introduction or the most significant content. This may be expanded upon in the subheadings farther down the page. When creating a document with a word processor, we divide the text to give it structure. Each part may have a title that describes what it covers, and each topic could have its own paragraph.*

### what is  HTML ?
* HTML pages are text documents.
* HTML uses tags (characters that sit inside angled  brackets) to give the information they surround special  meaning.
* Tags are often referred to as elements.
*  Tags are often sold in pairs. The opening tag marks the beginning of a piece of content, while the closing tag marks the conclusion. 
*  Opening tags can have characteristics that provide more information about the element's content. 
* A name and a value are required for attributes. 
* To study HTML, you must first understand what tags are available, what they perform, and where they may be used.

## *Extra Markup*
### So what we mean when we say Escape Characters?
*There are some characters that are used in  and reserved by HTML code. (For example, the  left and right angled brackets.)*

#### *When employing escape characters, double-check the website in your browser to make sure the proper symbol appears. This is because certain fonts may not support all of these characters, and you may need to specify a separate font in your CSS code for these characters.*


### *How do we Know what is the Html version?*
* Throw DOCTYPES tell browsers which version of HTML you use.*
	
### *How to add comments to the code?*
* wecan add comments to the code between the  `<!-- and --> `markers.
	
### *What does id and class attributes do for us?*
* The id and class attributes allow you to identify particular elements.
	
### *What does <div> and <span>  do ?*
* The <div> and <span> elements allow to group  block-level and inline elements together.

### *what can  <iframes> help us with?*
* <iframes> cut windows into your web pages through  which other pages can be displayed.
	
### *What doer  <meta> tag do ?*
* The <meta> tag allows you to supply all kinds of  information about your web page.

### *what do we use Escape characters in ?*
* Escape characters are used to include special  characters in your pages such as `<`, `>`, and `©`.

## *HTML5 Layout*
### *What does html5 elements indicate?*
*The new HTML5 elements indicate the purpose of  different parts of a web page and help to describe its structure.
	
### *what does the new element provide for us?*
* The new elements provide clearer code (compared  with using multiple `<div>` elements).
      
    
> Older browsers that do not understand HTML5  elements need to be told which elements are block-level elements."

### *What we should do To make our html5 work on Older browsers?*
* To make HTML5 elements work in Internet Explorer 8  (and older versions of IE), extra JavaScript is needed,  which is available free from Google.

## *Process & Design*
*The goal is to develop a page diagram that will be utilized to structure the website. This is referred to as a site map, and it shows how those pages can be organized.*

#### *card sorting:*

*Card sorting is writing down each item of information that a visitor could require on a separate piece of paper and then grouping the information into categories. Each group corresponds to a page, which, on bigger sites, can be grouped together to form distinct sections of the website. The information is then organized into categories and converted into a graphic known as a site map.*

#### *Wireframes:*
*sketching or shading areas  where each element of the page  will go (such as the logo, primary  navigation, headings and main  bodies of text, user logins etc). By creating a wireframe you can  ensure that all of the information  that needs to be on a page is  included.*

### *What are the thing that we need to take when we make any website?*
* It's important to understand who your target audience  is, why they would come to your site, what information  they want to find and when they are likely to return.

### *how does  Site maps help us?*
 * Site maps allow you to plan the structure of a site.

### *What does Wireframes  allowed us to do ?*
* Wireframes allow you to organize the information that  will need to go on each page.

### *What does Design all about ?*
* Design is about communication. Visual hierarchy helps  visitors understand what you are trying to tell them.

### *How can we differentiate between pieces of information?*
 * You can differentiate between pieces of information  using size, color, and style. 

### *For what can we use grouping and similarity?*
 * You can use grouping and similarity to help simplify  the information you present.

 ## *DESIGNING A SCRIPT:*
 *Once you know the goal of your script, you can work out the individual tasks needed to achieve it. This high-level view of the tasks can be represented using a flowchart.*

## *DESIGNING A SCRIPT:*
*Each individual task may be broken down into a sequence of steps. When you are ready to code the script, these steps can then be translated into individual lines of code.Every step for every task shown in a flowchart needs to be written in a language the computer can understand and follow.*

###  *What exactly is a script, and how can I make one?*
 *A script is a set of instructions that the computer may use to do a task. The script may only use a portion of all the instructions each time it runs. Because computers take a different approach to problems than humans, your instructions must allow the machine to accomplish the task programmatically. To begin creating a script, break down your aim into a series of activities, then plan out each step required to achieve each assignment (a flowchart can help).*

 ### *How do computers interact with the rest of the world?*
  *Data is used by computers to construct global models. Objects are used to represent tangible items in the models.Objects can contain attributes that provide information about the object; methods that conduct tasks based on the object's properties; and events that occur when a user interacts with the computer.Programmers may write code that says, "Run that function when this event happens".Web browsers construct a model of the web page using HTML syntax. Each element generates a node of its own (which is a kind of object).You develop code that leverages the browser's representation of the web page to make web pages interactive.*

### *How do I build a web page script?*
*JavaScript code should be kept in its own JavaScript file. JavaScript files are text files with the. js suffix, similar to HTML pages and CSS style sheets.In HTML pages, the `<Script>` element instructs the browser to load the JavaScript file (much like the `<1ink>` element instructs the browser to load a CSS file).Because the script works with the model of the web page that the browser has produced, the HTML will not have been altered if you inspect the source code of the page in the browser.*















	






