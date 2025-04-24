

HTML – Day 001:

Client – server architecture:

clinet → request → web server

← response←

web servers examples like IIS, apache,

client side languages:

- HTML

- CSS

- JavaScript

  

Server-side (backend)

- .Net

- PHP

- Node.js

- Python

  

web server is needed to host our website.

Domain name → to direct to our website.

IANA → controls top-level domains registrations for example: .eg domain

  

Web roles:

1. UI/UX → UI stands for User interface, UX stands for user experience.

UI/UX Designer & skills:

- photoshop.

- illustrator.

  

Wireframe (design) → website template

  

2. UI/UX Developer:

is responsible for turning ui/ux design into functional website.

  

3. Front-end developer:

HTML, CSS, Angular, react.js, Vue.js

  

4. Back-end developer:

a. .NET → MVC, SQL Server, .NET Core.

  

5. Full-stack developer:

front-end + back-end developer.

→ .NET Full stack developer.

→ MEAN stack developer.

→ PHP (LAMP) developer.

  

  

**HTML (Hyper-text Markup Language):**

- HTML is a language for describing webpages.

- it is not a programming language, it is a markup language.

- It uses markup tags to describe web pages.

- it is browser dependent language.

  

- An HTML element usually consists of a start tag and end tag, with the content inserted in between <p> My first paragraph </p>

- HTML element with no content are called empty elements. Empty elements do not have an end tag, such as <br> element which indicates a line break.

- HTML elements can be nested (elements contain elements).

- the HTML5 standard does not require lowercase tags, but W3C recommends lowercase in HTML elements, and demands lowercase for stricter document types like XHTML.

<img /> is self-closing tag, which doesn’t require closing tag.

<img src=””> src is an attribute to img tag.

<b> </b> → for bold text.

- comments are not displayed by the browser, but they can help document your HTML source code.

- HTML Comment:
-
```

 <!-- this is a comment →

- conditional comments: defines some HTML tags to be executed by specific browser only.

<!-- [if IE 9]>

… some HTML here …

<![endif] →
```
  

HTML Entities:

- reserved characters in HTML must be replaced with character entities.

- like whitespace, <, >, &.

- to display reserved characters, we must use character entites in the HTML source code, like : &Entity_Name; or &#entity_number;

- Note: Entity names are case sensitive.

Example:

&nbsp → whitespace. (non-breaking space)

&#160 → whitespace.

  

Check reference for HTML entities.

  

HTML Colors:

* in HTML, a color can be specified by using a color name, an RGB value, or a HEX value.

- color name: red, blue, yellow.

- RGB Value: using this formula: rgb(red, green, blue), each parameter defines the intensity of the color between 0 & 255. example: rgb(255,0,0) is red, rgb(0,0,0) is black, rgb(255,255,255) is white.

- hex value: a color can also be specified using a hexadecimal value in the form: #RRGGBB, where RR(red), GG(green), BB(blue) are hexadecimal values between 00 & FF. Example: #FF0000 is displayed as red, because red is set to its highest value (FF) and the others are set to the lowest value (00).

  

to allow browser identify document as HTML web page:

<!DOCTYPE html>

  

We can use style attribute to allow inline CSS code:

for example:
```


<p style="color: #F3AADF; font-size:28; text-align: center">

<!-- <font color="#30E4DD"> -->

<b>Hello, World!</b> <br>

Welcome to my page!

<!-- </font> --->

</p>

```  

Head Section:

contains:

* title tag: define web page’s title.

<head>

<title> My Page </title>

</head>

  

* Meta tag: used to store information usually relevant to browsers and search engines.

<head>

<meta charset="UTF-8">

</head>

- to display an HTML page correctly, a web browser must know which character set (character encoding) to use.

- ASCII was the first character encoding standard (also called character set). ASCII defined 127 different alphanumeric.

- ANSI (windows-1252) was the original Windows character set, with support 256 different codes.

- ISO-8859-1 was the default character set for HTML 4. this character set also supported 256 different character codes.

- because ANSI & ISO 8859-1 were so limited, the default character encoding was changed to UTF-8 in HTML5.

- UTF-8 (Unicode) covers almost all of the characters and symbols in the world.

  

Body Section:

HTML Headings:

- headings are defined with <h1> to <h6> tags.

- <h1> defines the most important heading (bigger font). <h6> defines the least important heading (smaller font).

- <h1> headings should be used for main headings, followed by <h2> headings, then the less important <h3>, and so on.

  

Headings Are Important:

- Search engines use the headings to index the structure and content of your web

pages.

- Users skim your pages by its headings. It is important to use headings to show

the document structure.

  

HTML grouping (container) tags:

- Often used as a container for other HTML elements.

- <div> Defines a section in a document (block-level).

- <span> Defines a section in a document (inline).

  

**HTML Block and Inline Elements:**

- Every HTML element has a default display value depending on what

type of element it is. The default display value for most elements is

block or inline.

**Block-level Elements:**

- A block-level element always starts on a new line and takes up the full

width available (stretches out to the left and right as far as it can).

- Examples of block-level elements: **<div>**, <h1> - <h6>, <p>, <form>.

**Inline Elements:**

- An inline element does not start on a new line and only takes up as much

width as necessary.

- Examples of inline elements: <span>, <a>, <img>.

  

Day - 01 task:

div [name]

div [info] [image]

div [education for example]

  

  

# text formatting elements:

<b>text</b>writes text as bold

<strong> text </strong>Important text

<i>text</i>writes text in italics

<em> text </em>Emphasized text

<u>text</u>writes underlined text (Deprecated)

<sub>text</sub>lowers text and makes it smaller

<sup>text </sup>lifts text and makes it smaller

<del>text</del>strikes a line through the text

<small> text </small>Define Smaller text than the container.

<mark> text </mark>Marked or highlighted text.

<font> text </font>Defines font size, name and color (Deprecated).

<center>text</center>Show the text on Center (Deprecated).

  

HTML Styles:

- Setting the style of an HTML element, can be done with the style attribute.

- The HTML style attribute has the following syntax:

<tagname style="property:value;">

- The property is a CSS property, the value is a CSS value.

- Example:

<body style="background-color:red;">

<h1 style="color:blue;">This is a heading</h1>

<h2 style="text-align:center;">Centered Heading</h2>

<p style="font-family:courier; font-size:16">This is a paragraph.</p>

</body>

  

HTML Images:

- In HTML, images are defined with the <img> tag.

- The <img> tag is empty, and does not have a closing tag.

- Syntax:

<img src="url" alt="some_text" width="width" height="height">

- Example:

<img src="html5.gif" alt="HTML5 Icon" width="128" height="128">

- It’s recommended to use style attribute for width and height, as the

following:

<img src="html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">

- The src attribute (Required) specifies the URL (web address) of the image.

- The alt attribute (Required) provides an alternate text for an image, If a

browser cannot find an image, it will display the value of the alt attribute.

  

<center><img src="images/500px.jpeg" alt="Sea" width="480px" height="480px"></center>

  

  

**HTML Links:**

- HTML links are hyperlinks. You can click on a link and jump to another

document.

- In HTML, links are defined with the <a> tag: <a href="url">link text </a>

- Link Colors in the Page (these body tag attributes are deprecated, and CSS

should be used instead):

- The href attribute specifies the destination web address or local page (in the

same website).

<a href="http://www.iti.gov.eg">ITI Website</a>

<a href=“about.html">HTML Images</a>

  

- Create bookmarks (link to an area in the same page):

<!—First, define bookmark using id attribute -->

<h2 id="tips">Useful Tips Section</h2>

<!-- Then add link to it-->

<a href="#tips">Go to Page Top</a>

<!-- When you link to anchors on external pages use this syntax -->

<a href="http://www.iti.gov.eg/rules/rules.htm#Section_a">Rules - Section a </a>

  

- Link Targets: The target attribute specifies where to open the linked

document.

_blank - Opens the linked document in a new window or tab

_self - Opens the linked document in the same window/tab as it was clicked (this is default)

_parent - Opens the linked document in the parent frame

_top - Opens the linked document in the full body of the window

framename - Opens the linked document in a named frame

- Example:

<a href="http://www.iti.gov.eg" target="_blank">ITI Website</a>

  

Image Link:

<a href="myfile.htm"><img src="rainbow.gif"></a>

  

Link to Email:

<a href="mailto:email@hotmail.com">Send Mail</a>

<a href="mailto:email@hotmail.com?subject=Hello">Send Email</a>

  

  

Day 002:

iframe is used to show a nested webpage/video from another site in my website.

<iframe name="second" src="http://www.aun.edu.eg" width="550" height="350"></iframe>

  

<a href="file:///" target="second">Link will open in iframe </a>

**using id of iframe as a target will open the link in the iframe.**

  

Table Tags:

<table> tag:

Used to define main table layout, and specifies start and the end of the table structure.

<tr> tag:

Used to define row inside the table, and Specifies row start and end.

<td> or <th> tag:

Used to define columns inside each row, and this tag contains cell data.

<th> used with the header cell and make it centered and bold.

  

<table border="1">

<caption align="top">Table Caption</Caption></caption>

<tr>

<td>First Cell</td>

<td>Second Cell</td>

</tr>

<tr>

<td>Seventh Cell</td>

<td>&nbsp;</td>

</tr>

</table>

  

we can use css to create border for table (outer border).

For creating inner borders of table, we need to use CSS with td tag, but to minimize work we put it in head section

<style>

td {border:solid 2px green}

</style>

  

to cancel spaces between table cells:

<table style="border:solid 3px red" cellspacing="0">

  

<caption align="top">Table Caption</Caption></caption>

caption is used to create a table caption

  

padding: leaves space between content & border.

  

Colspan and Rowspan attributes

<td colspan="2">&nbsp;</td>

<td rowspan="2">&nbsp;</td>

<td colspan="2" rowspan="2">&nbsp;</td>

  

  

HTML Forms:

form tag:

<form>

<!-- fields - ->

</form>

  

attributes:

- action = address

- method = post or get