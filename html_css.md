# HTML and CSS
https://developer.mozilla.org/en-US/docs/Web/HTML/reference

https://developer.mozilla.org/en-US/docs/Web/CSS/Reference

&nbsp;

---

### HTML Validation
https://validator.w3.org/

### CSS Validation
https://jigsaw.w3.org/css-validator/

&nbsp;

---
## Design/Layout
https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model

https://developer.mozilla.org/en-US/docs/Web/CSS/display

https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing

https://developer.mozilla.org/en-US/docs/Web/CSS/font-size

## Browser Shortcuts (Chrome)
| Shrtcut | Usage |
|---------|-------|
| ctrl + o | open a file in the browser |
| ctrl + shift + i | open developer tools |

https://developers.google.com/web/tools/chrome-devtools/dom/

## Skeleton Boilerplate
```html
<!DOCTYPE html>
<html lang="EN">
  <head>
    <title></title>
    <meta charset="utf-8" />
    <link rel="stylesheet" type="text/css" href="index.css">
  </head>

  <body>

  </body>
</html>
```

## Comments
```html
<!-- HTML Comment -->
```
```css
/* CSS Comment */
```

## Style Conventions
- Use lowercase letters within element names, attributes, and values
- Indent nested elements
- Strictly use double quotes, not single or completely omitted quotes
- Remove the forward slash at the end of self-closing elements
- Omit the values on Boolean attributes

- Use class and id names that indicate purpose, not literal stylizations subject to change, i.e., 'alert' instead of 'red'
- always use alt="text" on images
- never use inline styles with HTML -- separate content from style and put styles in an external stylesheet
- use semantic HTML tags (article, header, footer, aside) instead of generic div tags wherever possible

- keep styles organized in logical groups for ease of finding them and label each group with a comment at the start
- write CSS using multiple lines and spaces, making it easier to read
- class names should be modular and pertain to content, not appearance; they should be lowercase and hyphen-delimited

- keep the specificity of selectors as low as possible
- with the above in mind, avoid using id's since they break the cascade and are of heaviest specificity
- use a single specific class when it makes sense, such as to reduce performance hits of applying too many classes to the same element
- use shorthand properties and values (margin - or padding - for example, instead of margin-left, margin-right, etc.)
- use shorthand hex codes
- drop units from zero values

- indent nested tags
- avoid putting more than two elements on a single line
- Use '/ > ' with self-closing tags for improved readability (or don't, just be consistent)
- Order properties alphabetically or logically to make them easier to find inside a selector block

&nbsp;

## Special HTML Character Entities
| Entity | Description|
|------|------------|
| \&nbsp; | blank line |
| \&ndash; | dash |
| \&mdash; | long dash |
| \&copy; | copyright |
| \&[letter]acute; | accent; ex. -- resum\&eacute; --> resum&eacute; |
| \&lt; \&gt; | less than (<) greater than (>) |
| \&amp; | ampersand (&) |
| \&quot; | double quote ("), used to embed a double quote inside a double-quoted attribute value |

## Links
### Parameter Encodings
Note: URL parameters, which can be used in links, must be appended to a URL beginning with a question mark (?) and joined to other parameters with an ampersand (&).

ex. &ndash; 
```html
<a href="mailto:shay@awesome.com?subject=Reaching%20Out&body=How%20are%20you">Email Me</a>
```

| Parameter | Meaning |
|-----------|---------|
| \%20 | space |
\%0A | line break |

### Link Target
#### A new window
```html
<a href="http://shayhowe.com/" target="_blank">Shay Howe</a>
```

#### Part of the same page
```html
<body id="top">
  ...
  <a href="#top">Back to top</a>
  ...
</body>
```

&nbsp;

---
## HTML
### Terms/Concepts
*element* - designators that define the structure and content of objects within a page
*tag* - a set of opening and closing tags (keywords surrounded by a < and a >) which delineate an element
*attribute* - properties used to provide additional information about an element

### boilerplate
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Hello World</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>This is a web page.</p>
  </body>
</html>
```

&nbsp;

### HTML Semantics
the practice of giving content on the page meaning and structure by using the proper element. Semantic code describes the value of content on a page, regardless of the style or appearance of that content.

#### Semantic Elements
| Element | Description |
|---------|-------------|
| \<h1> \</h6> | headings |
| \<p> \</p> | paragraph|
| \<strong> | givces strong importance to text |
| \<b> | stylistically-offset bold text |
| \<em> \</em> | place a stressed emphasis on text |
| \<i> \</i> | convey text in an alternative voice or tone almost as quotation marks |

NOTE: If you intend to use boldface for important text, use &lt;strong&gt; instead of &lt;b&gt; if you wish to use italics for emphasis, use &lt;em&gt; instead of &lt;i&gt;.

#### Structural Elements
| Element | Description |
|---------|-------------|
| \<header> \</header> | IDs the top (heading, intro. text, navigation menu) of a page, article, section or other segment of a page |
| \<nav> \</nav> | IDs a section of major navigational links, used for primary navigation sections only |
| \<article> \</article> | IDs a section of independent, self-contained content which may be independently distributed or reused, i.e., blog post, newspaper article, user-submitted content, etc. |
| \<section> \</section> | IDs a thematic grouping of content which generally includes a heading; specifies content as related together | \<aside> \</aside> | holds content such as sidebars, inserts or brief explanations tangentially related to the content surrounding it |
| \<footer> \</footer> | IDs closing or end of a page, article, section or other segment of a page |
| \<blockquote>\</blockquote> | IDs a section of quoted text |
| \<address>\</address> | IDs contact information |

## HTML Element Flowchart
http://html5doctor.com/downloads/h5d-sectioning-flowchart.pdf

&nbsp;

---
```html
<!-- HTML Cheatsheet -->
<!DOCTYPE html>
<html lang="en-US">
<head>
  <title>Budget Planner</title>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="/stylesheets/whitespace-reset.css">
  <script src="/javascripts/jquery-3.5.0.js"></script>  
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
</head>
  <body>
    <a href="https://www.wikipedia.org/" target="_blank">This Is A Link To Wikipedia</a>
  </body>
</html>
 
<img src="url" alt="text" />
  
<video src="myVideo.mp4" width="320" height="240" controls>
  Video not supported
</video>


/* Tables */
  <div class="search">Search the table</div>
  <table>
    <thead>
      <tr>
        <th>Company Name</th>
        <th>Number of Items to Ship</th>
        <th>Next Action</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td colspan="2"></td>
        <td></td>
        <td></td>
      </tr>
      <tr>
        <td rowspan="2">Davie's Burgers</td>
        <td>2</td>
        <td>Send Invoice</td>
      </tr>
      <tr>
        <td>Baker's Bike Shop</td>
        <td>3</td>
        <td>Send Invoice</td>
      </tr>
    <tfoot>
      <td>Total</td>
      <td>28</td>
    </tfoot>
  </table>


/* Forms and Form Elements */
    <section id="overlay">
      <img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-6/htmlcss1-img_burger-logo.svg" alt="Davie's Burgers Logo" id="logo">
      <hr>
      <form action="submission.html" method="POST">
        <h1>Create a burger!</h1>
          <section class="protein">
          <label for="patty">What type of protein would you like?</label>
          <input type="text" name="patty" id="patty">
        </section>
        <hr>
        <section class="toppings">
          <span>What toppings would you like?</span>
          <br>
          <input type="checkbox" name="topping" id="lettuce" value="lettuce">
          <label for="lettuce">Lettuce</label>
          <input type="checkbox" name="topping" id="tomato" value="tomato">
          <label for="tomato">Tomato</label>
          <input type="checkbox" name="topping" id="onion" value="onion">
          <label for="onion">Onion</label>
        </section>
        <hr>
        <section class="submission">
          <input type="submit" value="Submit">
        </section>
        
      </form>
    </section>

/* Client-side Validation */
   <section class="overlay">
      <h1>Sign Up</h1>
      <p>Create an account:</p>
      <form action="submission.html" method="GET">
        <label for="username">Username:</label>
        <br>
        <input id="username" name="username" type="text" required minlength="3" maxlength="15">
        <br>
        <label for="pw">Password:</label>
        <br>
        <!--Add the pattern attribute to the input below-->
        <input id="pw" name="pw" type="password" required minlength="8" maxlength="15">
        <br>
        <input type="submit" value="Submit">
      </form>
    </section>
```

&nbsp;

&nbsp;

---
## CSS

&nbsp;

---
### Referencing CSS in HTML
```html
<head>
  <link rel="stylesheet" href="stylesheets/main.css">
</head>
```

### CSS Resets
Resets are a good practice for acheiving uniformity across browsers and devices and should go at the top of a css file.
Eric Meyer's Reset: https://meyerweb.com/eric/tools/css/reset/
Normalize.css: https://necolas.github.io/normalize.css/

&nbps;

---
### Responsive Design/Layout
#### box-sizing: content-box|border-box;
```css
/* the next two snippets are alternate versions of the same thing -- defaulting to border-box instead of content-box while still being able to override border-box when needed for components that rely on content-box */

/* version 1 (old version with override for .component class elements which require the default content-box) */
* {
  box-sizing: border-box;
}

.component * {
   box-sizing: content-box;
}

/* version 2 */
html {
  box-sizing: border-box;
}

*, *::before, *::after {
  box-sizing: inherit;
}
/* this is a CSS reset which uses box-sizing for responsive layout and also covers pseudo elements */

/* legacy vendor prefix support: */
html {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
*, *:before, *:after {
  -webkit-box-sizing: inherit;
  -moz-box-sizing: inherit;
  box-sizing: inherit;
  }
```
border-box makes responsive layouts easier to make because sizing specifies the entire size of the object, including the padding and border, unlike the default.  It's commonly used in CSS resets for responsive design purposes.

&nbsp;

### display: block|inline|inline-block|flex|grid
- block elements take up the entire width of a row, automatically separated with newline characters
- inline elements are fitted as many as will fit across the width of a row before being moved to the next row
- inline-block elements will allow other inline or inline-block elements next to them if there is width left in the parent containter
- flex (see below)
- grid (see below)

NOTE: newlines introduce space between elements which can cause layout problems.  Here is a workaround using comments in the case of a list:
```html
  <ul>
    <li>Item 1</li><!--
  --><li>Item 2</li><!--
  --><li>Item 3</li><!--
  --><li>Item 4</li>
  </ul>
```

```css
body {
  margin: 50px;
}

ul {
  background-color: #a7ceff;
  border: 10px solid blue;
  list-style: none;
  padding: 0;
}

li {
  background-color: #ffc;
  border: 10px solid red;
  box-sizing: border-box;
  line-height: 120px;
  min-height: 120px;
  text-align: center;
  display: inline-block;
  width: 25%;
}
```

&nbsp;

---
### flex
```css
/* CSS Flexbox -- 1-dimensional layouts */
```

&nbsp;

---
### grid
```css
/* CSS Grid -- 2-dimensional layouts */
/*
    grid-template-columns defines the number and sizes of the columns of the grid
    grid-template-rows defines the number and sizes of the rows of the grid
    grid-template is a shorthand for defining both grid-template-columns and grid-template-rows in one line
    grid-gap puts blank space between rows and/or columns of the grid
    grid-row-start and grid-row-end makes elements span certain rows of the grid
    grid-column-start and grid-column-end makes elements span certain columns of the grid
    grid-area is a shorthand for grid-row-start, grid-column-start, grid-row-end, and grid-column-end, all in one line
*/
/* 
    grid-template-areas specifies grid named grid areas
    grid layouts are two-dimensional: they have a row, or inline, axis and a column, or block, axis.
    justify-items specifies how individual elements should spread across the row axis
    justify-content specifies how groups of elements should spread across the row axis
    justify-self specifies how a single element should position itself with respect to the row axis
    align-items specifies how individual elements should spread across the column axis
    align-content specifies how groups of elements should spread across the column axis
    align-self specifies how a single element should position itself with respect to the column axis
    grid-auto-rows specifies the height of rows added implicitly to the grid
    grid-auto-columns specifies the width of columns added implicitly to the grid
    grid-auto-flow specifies in which direction implicit elements should be created
*/
```

```css

/* CSS Grid */
.container {
  display: grid;
  max-width: 900px;
  position: relative;
  margin: auto;
  grid-gap: 10px;
  grid-template-areas: "header header"
                       "nav nav"
                       "left right"
                       "footer footer";
  grid-template-columns: 200px 400px;
  grid-template-rows: 150px 200px 600px 200px;
}

h1, h2 {
  font-family: monospace;
  text-align: center;
}

header {
  grid-area: header;
  background-color: dodgerblue;
}

nav {
  grid-area: nav;
  background-color: beige;
}

.left {
  grid-area: left;
  background-color: dodgerblue;
}

.right {
  grid-area: right;
  background-color: beige;
}

footer {
  grid-area: footer;
  background-color: dodgerblue;
}
```

```css
/* Example */
.grid {
  border: 2px blue solid;
  height: 500px;
  width: 500px;
  display: grid;
  grid-template: repeat(2, 200px) / repeat(2, 25%) 2fr 1fr;
  grid-gap: 10px 15px;
}

.box {
  background-color: beige;
  color: black;
  border-radius: 5px;
  border: 2px dodgerblue solid;
}

.a {
  grid-column: 1 / span 2;
  grid-row-start: 1;
  grid-row-end: 3;
}

/* Another Example */
.grid {
  border: 2px blue solid;
  height: 500px;
  width: 500px;
  display: grid;
  grid-template-columns: 25% 25% 2fr 1fr;
  grid-template-rows: repeat(2, 200px);
  grid-gap: 10px 15px;
}

.box {
  background-color: beige;
  color: black;
  border-radius: 5px;
  border: 2px dodgerblue solid;
}
.a {
  grid-column: 1 / span 2;
  grid-row-start: 1;
  grid-row-end: 3;
}

/* more examples: */
#grid-container {
  display: grid;
  width: 100px;
  grid-template-columns: 20px 20% 60%;
}

.grid {
  display: grid;
  width: 100px;
  grid-template-columns: 1fr 60px 1fr;
}

#grid-container {
  display: block;
}

/*
In this example, the second column take 60px of the avaiable 100px so the first and third columns split the remaining available 40px into two parts (`1fr` = 50% or 20px)
*/
```

```css
.grid {
  display: grid;
  width: 100px;
  grid-template-columns: 1fr 60px 1fr;
}

// The distance between rows is 20px
// The distance between columns is 10px
#grid-container {
  display: grid;
  grid-gap: 20px 10px;
}

/*  grid-row: grid-row-start / grid-row-end;  */
/*Example*/
.item {
  grid-row: 1 / span 2;
}

/* CSS syntax:
grid-row-start: auto|row-line;
grid-row-end: auto|row-line|span n;
*/
grid-row-start: 2;
grid-row-end: span 2;

/*CSS Syntax */
grid-row-gap: length; /*Any legal length value, like px or %. 0 is the default value*/
.item1 {
  grid-area: 2 / 1 / span 2 / span 3;
}

#container {
  display: grid;
  justify-items: center;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr 1fr 1fr;
  grid-gap: 10px;
}

/* Specify two rows, where "item" spans the first two columns in the first two rows (in a four column grid layout)*/
.item {
  grid-area: nav;
}

.grid-container {
  display: grid;
  grid-template-areas:
    'nav nav . .'
    'nav nav . .';
}

/*CSS Grid Syntax */
grid-auto-flow: row|column|dense|row dense|column dense;
// The grid items are positioned to the right (end) of the row.
#grid-container {
  display: grid;
  justify-items: start;
}

.grid-items {
  justify-self: end;
}

#container {
  display: grid;
  align-items: start;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr 1fr 1fr;
  grid-gap: 10px;
}
```

&nbsp;

### Approach to Styling a Page
- Start by adding some simple properties, primarily color and font, to the body selector to give the page an overall look and feel that focuses on your content.
- Set the position and size of the organizational components of the page: header, footer, sidebars, etc. to match your desired page structure.
- Apply your background and font colors to those parts of the page that need non-default styling.
- By now, your page should look a lot like your final product. Finish by concentrating on each component individually and make any adjustments you need to make to achieve the desired look.

&nbsp;

### Terms/Concepts
*selectors* - designates exactly which element or elements within our HTML to target and apply styles (such as color, size, and position) to

*property* - determines the styles that will be applied to that element. Property names fall after a selector, within the curly brackets ({}) and immediately preceding a colon (:)

*value* - determines the behavior of a property with a value. Values can be identified as the text between the colon (:) and semicolon (;)

*type selector* - targets elements by their element type

*class selector* - allow us to select an element based on the element’s class attribute value; specified with a dot (.)

*id selector* - even more precise than class selectors, as they target only one unique element at a time. Just as class selectors use an element’s class attribute value as the selector, ID selectors use an element’s id attribute value as a selector; specified with a hash (#)

### CSS Principles
*cascade* - all styles cascade down the css file, i.e., those at a lower point can override those above them if they specify the same element, id, class or property, overriding previous settings; the same holds true for either for selectors or properties inside an individual selector; different types of selectors with different specificity can break the cascade, however.

*specificity* - every CSS selector has a specificity weight; a selector's speicificity weight along with its placement in the cascade identifies how its styles will be rendered;

| Selector | Specificity Weight Point Value |
|----------|-------------|
| type | 0-0-1 |
| class | 0-1-0 |
| id | 1-0-0 |

Point Values: [id]-[class]-[type]

p.hotdog has a value of 0-1-1

.hotdog p.mustard, a value of 0-2-1

### Seletor Format
[prequalifier(s)] key_selector { parameters };

The **key selector** IDs exactly which element the styles will be applied to

- Selectors with higher values will take precedence even if they come higher in the cascade.

- It's considered best practice not to prefix a class selector with a type selector (not p.mustard, but instead better just .mustard).


### Keeping specificity weights low
The higher a specificity weight rises, the more likely the cascade is to break. Counter this by being as modular as possible, sharing similar styles from element to element; one way to to do this is to layer on different styles by using multiple classes.

ex. -
```html
<a class="btn btn-danger">...</a>
<a class="btn btn-success">...</a>
```
```css
.btn {
  font-size: 16px;
}
.btn-danger {
  background: red;
}
.btn-success {
  background: green;
}
```

### Colors
- Hex 
- RGB
- Keyword
- HSL

| keyword | hex | RGB | HSL |
|---------|-----|-----|-----|
| white | #FFFFFF | rgb(255, 255, 255) | hsl(0, 100%, 100%) |
| black | #000000 | rgb(0, 0, 0) | hsl(0, 0%, 0%) |

- Hex matching pairs can be shortened, i.e., #FFFFFF -> #FFF; #FF6600 -> #F60
- rgb has an alternate form, RGBa, which adds one more value to specify transparency, i.e., `rgba(255, 102, 0, .5)` specifies 50% transparency
- HSL stands for Hue Saturation and Lightness and has an HSLa variant much like RGBa

#### Hex Digits
| Decimal | 0 - 9 | 10 | 11 | 12 | 13 | 14 | 15 |
|---------|-------|----|----|----|----|----|----|
| Hexadecimal | 0 - 9 | A | B | C | D | E | F |

### Length/Size Units
```css
/* absolute pixels */
p {
  font-size: 14px;
}

/* relative percentage */
.col {
  width: 50%;
}

/* relative em */
/* calculated based on element's font size */
.banner {
  font-size: 14px;
  width: 5em;
}

/* automatic */
p {
  margin: auto
}
```
NOTE:
- auto can be used:
  - As a width or height, it tells the browser to try to fit the entire element (including its margins) in its container.
  - As a left or right margin value on a block element, it tells the browser to push the element all the way right or left (note the reversal!) inside its container. You can center a block element by setting both left and right margins to auto.
  - As a top or bottom margin value, auto is equivalent to 0.
  - Note that padding does not accept auto values.

- Bugs in some older browsers make it a good idea to set the root font size in both the html and body elements. Always use pixels when you do so.

- Width and height have no effect on inline elements

#### When to Use Absolute or Relative Units
- Use absolute units sparingly, and stick with pixels. Pixels work well for:
  - the root font size
  - image widths and heights
  - top and bottom margins and padding, sometimes useful with left and right margins and padding
  - width or height of fixed-width/fixed-height containers such as navigation sidebars
  - border widths

- Use relative units liberally:
  - Use rems for fonts, possibly with a fallback to ems or pixels. The root font should use pixels.
  - If you must use ems instead of rems, try to avoid compounding font sizes.
  - Use rems, ems, or pixels for left and right margins and padding.
  - Use % for measurements that are proportional to the container element's width or height. Percentages work best for container dimensions and come in handy when you want certain areas of the page to grow and shrink as the width of the browser window changes.
  - Use auto with width and height to let the browser calculate an appropriate value.
  - Use auto with left and right margins to left, center, or right justify a block element within its container.

&nbsp;

---
### CSS Selectors
| type selector combination | meaning |
|------------|---------|
| p, div | all p and div elements |
| p > div | all div elements inside a p |
| p + div | all div elements next to a p |
| p ~ div | all div elements that follow a p |
| * | everything, everywhere |
| p * | everything inside a paragraph |
| p.italic | all p with class 'italic' |
| p#about | the p with id 'about' |
| article p:first-child | first child p element inside article |
| div p:nth-child(2) | selects the second p in every div |
| article p:nth-last-child(3) | selects the 3rd-to-last p in every article |
| p:first-of-type | select the first p |
| p:nth-of-type(even) | select the even-numbered paragraphs |
| p:nth-of-type(2n + 3) | select every 2nd plate starting with the 3rd |
| p span:only-of-type | select a span in any p if it is the only span in that p |
| p:last-of-type, h1:last-of-type | select the last paragraph and last h1 header |
| p:empty | select the empty paragraphs |
| p:not(.introductory) | select any p which is not of the class 'introductory' |
| *[for] | select any type/element which has an attribute 'for' set to any value |
| p[color=blue] | select any p which has a color parameter set to blue |
| p[color^=bl] | select any p which has a color parameter set to a value which begins with 'bl' |
| *[font-family$='o'] | select any type which has a font-family parameter set to a value which ends in 'o' |
| *[font-family*='new'] | select any type with a font-family parameter set to a value which contains 'new' |

### See:  https://flukeout.github.io/

&nbsp;

---
### When to Use Padding or Margins
You probably need to use padding when:

You want to change the height or width of a border.
You want to adjust how much background is visible around an element.
You want to alter the amount of clickable area.
You want to avoid margin collapse.
You want some horizontal spacing to the left or right of an inline element.
As before, use padding to separate the left and right sides of a container from its content. Use margins for the vertical gap.

&nbsp;

---
### How to Center an Item
#### margin: 0 auto block Method
```css
img {
  display: block;
  margin: 0 auto; /* 0: top and bottom margin, auto: left and right */
}
```

#### Text-Align Method
The “text-align: center” method is perhaps the most common one you’ll see for centering. It’s used mostly for centering text on your HTML page, but it can be used to center divs as well.

The trick here is to:

    Enclose the div that you want to center with a parent element (commonly known as a wrapper or container)
    Set “text-align: center” to parent element
    Then set the inside div to “display: inline-block”

```css
/* Goes inside html file to link to css: */
<link href="./css/style.css" type="text/css" rel="stylesheet">
```

```css
/* !important overrules other settings */
#column-one {
  width: 200px !important;
}

.post-title {
  color: blue !important;
}
```

```css
/* Descendant Selector --  match elements that are descended from another matched selector */
div p { }

section ol li { }

/* Give multiple selectors the same attribute/value pair
h5, p {
  color: rebeccapurple !important;
}
```

### Box Model

https://s3.amazonaws.com/codecademy-content/courses/freelance-1/unit-4/diagram-boxmodel.svg

Vertical Margins collapse to the larger of the two bordering items' margins


#### Box Model Content Box

https://content.codecademy.com/courses/updated_images/htmlcssdiagram_contentbox_Updated_1.svg

Changes the box model to border-box, which improves on the old model which was 
complicated by not including border and padding in the box size
```css
* {
  box-sizing: border-box;
}
```

```css
/* @font-face: */
/* enter address into web browser address bar, as an alternative to using a link tag in your html head, for selectors to insert into your CSS stylesheets, for example: */
href="https://fonts.googleapis.com/css?family=Space+Mono:400,700

/* Ex., Space Mono, 400, 700, latin: */
@font-face {
  font-family: 'Space Mono';
  font-style: normal;
  font-weight: 400;
  src: local('Space Mono'), local('SpaceMono-Regular'), url(https://fonts.gstatic.com/s/spacemono/v5/i7dPIFZifjKcF5UAWdDRYEF8RQ.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
```

```css
/* Universal Styles */
@font-face {
  font-family: 'Space Mono';
  font-style: normal;
  font-weight: 700;
  src: local('Space Mono Bold'), local('SpaceMono-Bold'), url(https://fonts.gstatic.com/s/spacemono/v5/i7dMIFZifjKcF5UAWdDRaPpZUFWaHg.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
```

```css
/* Media Queries */

@media only screen and (max-width: 535px) {
  .header {
    font-size: 14px;
  }

  .header a {
    padding: 30px 20px;
  }

  a.home {
    display: none;
  }
}
```
&nbsp;

---
See: 

https://learn.shayhowe.com/html-css/building-your-first-web-page/

https://learn.shayhowe.com/html-css/getting-to-know-html/

https://learn.shayhowe.com/html-css/getting-to-know-css/

https://www.codecademy.com/catalog/language/html-css

https://www.freecodecamp.org/learn/responsive-web-design/basic-html-and-html5/

&nbsp;