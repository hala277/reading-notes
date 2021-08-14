# Audio, Video, Images
##Images

### controlling sizes of  Images In css
*You can control the size of an  image using the width and height properties in CSS, just  like you can for any other box.  Specifying image sizes helps  pages to load more smoothly  because the HTML and CSS  code will often load before the  images, and telling the browser  how much space to leave for an  image allows it to render the rest  of the page without waiting for  the image to download.Whenever you use consistently  sized images across a site, you can use CSS to control the dimensions of the images, instead of putting the  dimensions in the HTML.*

### aligning Images Using css
+ There are two ways  to align img:
1. The float property is added  to the class that was created to  represent the size of the image.
2. New classes are created with  names such as align-left or align-right to align the images  to the left or right of the page.These class names are used in  addition to classes that indicate  the size of the image.

```
img.align-left {
 float: left;
 margin-right: 10px;}
img.align-right {
 float: right;
 margin-left: 10px;}
img.medium {
 width: 250px;
 height: 250px;}

```
   
### centering Images Using css
+ two common ways you can horizontally center an image:
1. On the containing element, you can use the text-align  property with a value of center.
2. On the image itself, you can use the use the margin property and set the values of the left and right margins to auto.

```
img.align-center { 
 display: block; 
 margin: 0px auto;} 
img.medium { 
 width: 250px; 
 height: 250px;}

```
### background-image

*The background-image  property allows you to place an image behind any HTML  element. This could be the entire  page or just part of the page. By  default, a background image will  repeat to fill the entire box. The path to the image follows the letters url, and it is put inside parentheses and quotes.*

```
body {
 background-image: url("images/pattern.gif");}

```
**Or**

```
p {
 background-image: url("images/pattern.gif");}

```
### repeating Images

+ The background-repeat property can have four values:
1. **repeat**
The background image is repeated both horizontally and  vertically 

2. **repeat-x**
The image is repeated horizontally only

3. **repeat-y**
The image is repeated vertically only.

4. **no-repeat**
The image is only shown once.

### background-attachment

*The background-attachment property specifies whether a  background image should stay in one position or move as the user  scrolls up and down the page.* 

+ It can have one of two values:
1. **fixed**
The background image stays in the same position on the page.

2. **scroll**
The background image moves up and down as the user scrolls up and down the page.

![reapeat img](https://bitsofco.de/content/images/2016/06/repeat.png)

### background position
*When an image is not being  repeated, you can use the background-position  property to specify where in the  browser window the background  image should be placed. This property usually has a pair  of values. The first represents  the horizontal position and the  second represents the vertical.*

```
body {
 background-image: url("images/tulip.gif");  background-repeat: no-repeat;
 background-position: center top;}

```
![background position](https://bitsofco.de/content/images/2016/06/position.png)

### shorthand background
*The background property acts like a shorthand for all of the other background properties you have just seen, and also the background-color property. The properties must be specified in the following order, but you can miss any value if you do not  want to specify it.*

![background property](https://devrix.com/wp-content/uploads/2015/07/background-property.jpg) 

**Conclusion:**
*You can specify the dimensions of images using CSS.  This is very helpful when you use the same sized  images on several pages of your site. Images can be aligned both horizontally and vertically using CSS. You can use a background image behind the box  created by any element on a page. Background images can appear just once or be  repeated across the background of the box. You can create image rollover effects by moving the  background position of an image. To reduce the number of images your browser has to  load, you can create image sprites.*

## Practical Information
*The term "search engine optimization" refers to the process of optimizing a website for search engines. In basic terms, it refers to the process of enhancing your website in order to enhance its exposure when consumers use Google, Bing, and other search engines to look for items or services connected to your business. The higher your pages' exposure in search results, the more likely you are to draw attention and attract new and existing consumers to your company.*

![SEO](https://i.pinimg.com/564x/2c/82/dc/2c82dc2736e0bbd5b96e61e9599c3ec4.jpg)



*Search engine optimization helps visitors find your  sites when using search engines. Analytics tools such as Google Analytics allow you to  see how many people visit your site, how they find it,  and what they do when they get there. To put your site on the web, you will need to obtain a  domain name and web hosting. FTP programs allow you to transfer files from your  local computer to your web server. Many companies provide platforms for blogging, email  newsletters, e-commerce and other popular website  tools (to save you writing them from scratch).*

## Video and Audio APIs
### HTML5 video and audio
*The `<video>` and `<audio>` elements allow us to embed video and audio into web pages.a typical implementation looks like this:*
``` 
<video controls>
  <source src="rabbit320.mp4" type="video/mp4">
  <source src="rabbit320.webm" type="video/webm">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>

```

### The HTMLMediaElement API
*Part of the HTML5 spec, the `HTMLMediaElement` API provides features to allow you to control video and audio players programmatically — for example `HTMLMediaElement.play()`, `HTMLMediaElement.pause()`, etc. This interface is available to both `<audio>` and `<video>` elements, as the features you'll want to implement are nearly identical.*




