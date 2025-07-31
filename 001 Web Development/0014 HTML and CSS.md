Tags: #HTML #CSS #HTMLShortcutKey

A collection of notes about HTML and CSS.

[HTML shortcut keys for faster coding.](Medium](https://medium.com/@akshayayathakula/12-essential-html-shortcuts-for-faster-coding-2e3d5723bd5d)

**HTML (Hypertext Markup Language)**: creates the structure of the website.

**CSS (Cascading Style Sheets)**: creates the style of the structure made from HTML.
JavaScript: makes the website more interactive and engaging for users.

---
# Elements and Tags in HTML

Tags: #Elements #Tags 

**Elements** on an HTML page are pieces of content wrapped in opening and closing HTML tags.

**Opening Tags** tell the browser that this is the start of an HTML element. It is comprised of a keyword enclosed in angle brackets **<>**, one example is the paragraph tag.

**Closing Tags** tell the browser where an element ends. They are identical to the opening tags but contains a forward slash before the keyword, example of this is the closing tag for the paragraph tag.

A full paragraph element looks like this.
```html
<p> some text content </p>
```

An element can be considered as a container for content. The opening and closing tags tell the browser what content the element contains.

[HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements)

***ALWAYS USE PROPER TAGS***

---
# Void Elements in HTML

Tags: #Void

HTML elements that does not have a closing tag.  These elements just have a single tag. They are known as void elements because they are void of any content, there is nothing inside of them, No closing tag means can't wrap content like other tags do.

Example:
```html
<br   />
<img  />
```

---
# Meta Information in HTML

Tags: #MetaInformation

Meta information in HTML is defined by the meta tag, which provides metadata about the HTML document. 

**Metadata** is data about data and is used by browsers, search engines, and other web services to understand and process the content of the webpage.

---
# Nesting and Indentation in HTML

Tags: #Nesting #Indentation

Indent any elements that are within other elements. When an element is nested with other elements, a parent and a child relationship is created between the elements. The nested elements are the children and the element they are nested within is the parent.

```html
<head></head>
<body>
	<p>Just some text</p>
</body>
```

In the code above the body element is the parent and the paragraph is the child.

HTML parents can have many children. Elements at the same level of nesting are considered to be siblings.

Example of siblings:
```html
<head></head>
<body>
	<p>The first child of body tag</p>
	<p>Another paragraph that is a sibling of the first paragraph.</p>
</body>
```

Indentation is used to make the level of nesting clear and readable for ourselves and other developers.

---
# Ordered and Unordered List in HTML

Tags: #List #OrderedList #UnorderedList

**Unordered List** are used to make a list where order doesn't matter.

```html
<ul>
	<li>Saging</li>
	<li>Manga</li>
	<li>Bayabas</li>
</ul>
```

**Ordered List** are used to make a list where the order matters.

```html
<!-- List about waking up -->
<ol>
	<li>Go to Bed</li>
	<li>Wake Up</li>
</ol>
```

***Take note the the li tag is the list item***

---

# Anchor Elements in HTML

Tags: #Links #Anchor

An anchor element is defined by wrapping the text or another HTML element we want to be a link using the a tag. The anchor element is one of the void elements in HTML.

```html
<a> About our Page </a>
```

## HTML Attribute

This is used to tell the anchor where is the destination to go to when it is clicked.  It is always in the opening tag. 

```html
<a href = "thisisalink.com"> The Odin Project </a>
```

---

# Rel Attribute in Anchor Tags in HTML

Tags: #Rel #Anchor

Used to define the relationship between the current document and the lined resource. Commonly used in anchor tags, link tags, and area tags.

**Rel Attributes in anchor tags common values:**
- noopener: Prevents then new page from accessing the window.opener property improving security.
- noreferrer: Prevents the browser from sending the HTTP referrer header
- nofollow: Tells search engines not to follow link
- external: Indicates the link leads to an external resource

```html
<a href = "somelink.com" target = "-blank" rel = "noopener noreferrer">Click This</a>
```

**NOTE: noopener and noreferrer are added for security reasons and is always recommended that the two are always paired.**

---
# Absolute and Relative Links in HTML

Tags: #AbsoluteLinks #RelativeLinks #Links 

Generally, there are two links used in a website, Absolute and Relative links. 

**Absolute Links:** links to pages on other websites on the internet. A typical absolute link will be made up of the following parts: **scheme://domain/path**.

**Relative Links:** Links to other pages within own website. It does not include the domain name, since it is another page on the same site.  It only includes the file path to the other page, relative to the page the link being created on. 

---
# Images in HTML

Tags: #Images #Links 

To display an image in HTML the image element is used. The image element is considered one of the void elements. 

**Example:**
```html
<img src = "some/location/in/the/code/base">
```

---
# Basic Syntax in CSS

Tags: #CSS #CSSSyntax

***Graphical representation of basic CSS syntax:***

![[Pasted image 20250716122749.jpg]]


---
# The DIV Element in HTML

Tags: #Div

The div is one of the basic HTML elements. It is an empty container. It is used to define a division or a section in an HTML document. It is a block-level element that is commonly used as a container for other HTML elements, which can then be styled with CSS or manipulated with [[0011 JavaScript]].

```html
<div class = "example">
	<!-- Some Tags and elements here -->
	<h1> Header </h1>
</div>
```

---
# Selectors in CSS

Tags: #Selectors

Selectors refer to the HTML elements to which CSS rules apply; they're what is actually being "selected" for each rule. 

## Universal Selector

The universal selector will select elements of every type (meaning the whole document).  Example:

```css
/* Adding the color purple throughout the design*/
* {
	color: purple; 
}
```

## Type Selectors

Tags: #Type

A type selector (can also be called as element selector) will select all elements of the given element type. Example:

```html
<!-- index.html -->
<div> Hello World! </div>
<div> Just another div in the page</div>
<p> This is a paragraph </p>
<div> This is another another div in the page</div>
```

```css
/* styles.css */
div {
	color: red;
}
```

The example above results to all with div elements in the index will have a color of red and those elements/tags that are not div will remain as is (int the example it was the paragraph tag).

## Class Selectors

Tags: #Class

 This selector will select all elements with the given class. Example:

```html
<!-- index.html -->
<div = "sample_class"> 
	<h1> </h1>
</div>
```

```css
/* styles.css */
.sample_class {
	color:red;
}
```

***Syntax for class selectors:**
	A period immediately followed by the case-sensitive value of the class attribute.  Classes aren't required to be specific to a particular element, so multiple use of the same class to many elements can be done.

**Adding multiple classes to a single element as a space-separated list.***

```html
<div class="alert-text severe-alert"> Some values here </div>
```

## ID Selectors

Tags: #ID 

ID selectors are similar to class selectors. Select an element with the given ID, which is another attribute you place on an HTML element. 

The difference is that an element can only have **one** ID whereas it can have multiple class names. Example:

``` html
<!-- index.html -->
<div id="data"> Some data and elements here </div>
```

```css
#title {
	background-color: red;
}
```

### When Should You Use ID and/or Class?

Tags: #Class  #ID #WhenToUseClassandID

Best Practices:
- Use **ID**s for unique elements like navigation bars, headers, or specific JavaScript targets.
- Use **Classes** for styling and grouping multiple elements to maintain flexibility and scalability in the codebase.

## The Grouping Selector

Tags: #Grouping

Use this if two groups of elements share the same style declarations. Example:

``` css
/* Instead of doing this */

.read {
	color: white;
	background-color: black;
}

.unread {
	color: white;
	background-color: black;
}

/* Do this */

.read, .unread {
	color: white;
	background-color: black;
}

/* If they have unique declarations to them, we can add this*/

.read {
	/* Unique Declarations here*/
}

.unread {
	/* Unique Declarations here*/
}
```

This selector is used to minimize repetition of code fore more readability.

## Chaining Selectors

Tags: #Chaining

Chaining selectors as a list without any separation. For example we have:

```html
<div>
	<div class="subsection header">Latest Posts</div>
	<p class="subsection preview">This is where a preview for a post might go.</p>
</div>
```

There are two elements with the **subsection** class that have some sort of unique styles. Their are also a space containing another class name. We can chain both the class selectors together in the CSS style sheet.

```css
.subsection.header {
	color: red;
}

/*When you want to edit the classes with the subsection class name*/
.subsection {
	color: white;
}
```

**Chain a class and an ID**
```html
<div>
	<div class="subsection header">Latest Posts</div>
	<p class="subsection" id="preview">
		This is where a preview for a post might go.
	</p>
</div>
```

You can chain them by:
```css
.subsection.header {
  color: red;
}

.subsection#preview {
  color: blue;
}
```

Chaining more than one type of selector is not possible since an element can't be two different types at once. Example, chaining two types of selectors like div and p would render the result divp, which would not work since their is no divp element.

**Chaining selectors is efficient when you want to target a specific element with a specific design**

---
# Combinators

Tags: #Combinator 

**Combinators** allows combining multiple sectors differently than either grouping or chaining them, as they show a relationship between the selectors. 

**Targets Elements based on relationships (parent -> child ->sibling etc.)**
## Descendant Combinator

Tags: #DescendantCombinator #Relationship 

Represented by a single space between selectors. This combinator will only cause elements that match the last selector to be selected if they also have an ancestor (parent, grandparent, etc.) that matches the previous selector.

```html
<div class="ancestor">
	<!-- Some information of ancestor here -->
	<div class="contents">
		<!-- Some information of contents here -->
		<div class="sibling_conten">
			<!-- Some information of sibling content here -->
		</div>
	</div>
</div>

<div class="solo">
	<!-- Some information of solo div here -->
</div>
```

```css
.ancestor.contents {
	/*Some designs here
	All children of contents will be 
	edited here*/
}
```

---
# Basic Properties to Get Started with CSS

Tags: #CSS #Styles

## color and background-color

The color property sets an element's text color, while background-color sets the background color of an element.

**Example:**
```css
p {
  /* hex example: */
  color: #1100ff;
}

p {
  /* rgb example: */
  color: rgb(100, 0, 127);
}

p {
  /* hsl example: */
  
}
```

## typography basics and text-align

Tags: #Typography #Texts

**font-family** can be a single value or a comma-separated list of values that determine what font an element uses.

If a browser cannot find or does not support the first font in a list, it will use the next one, then the next one and so on. Therefore, it is best practice to include a list of values for this property, **starting with the most important font and ending with a generic font.**

**font-size** will change the size of the fonts. **font-weight** affects the boldness of the text, assuming the font supports the specified weight.

**text-align** will align text horizontally within an element, and can use the common keywords such as center, left, right.

## image height and width

Tags: #Images 

By default, an image element's height and width values will be the same as the actual image file's height and width. If there is a need to adjust the size of the image without causing it to lose its proportions, the use of value **auto** for the height property is needed and adjust the width value.

```css
img {
	height: auto;
	width: 400px;
}
```

Example:

```html
<!-- Image here -->

<div class="image_placeholder">
	<h1>This is an Image</h1>
	<div class="image">
		<img src="banner.jpg" alt="banner">
	</div>
</div>
```

```css
.image_placeholder .image img {
	height: auto;
	width: 700px;
	border: 3px solid darkred;
}
```

---
# Adding CSS to HTML

Tags: #CSS #HTML #AddingCSStoHTML

```html
<!-- index.html -->
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

```css
/* styles.css */
div {
  color: white;
  background-color: black;
}

p {
  color: red;
}
```

***Why?***

1. It keeps the HTML and CSS separated, which results in the HTML file being smaller and making things look cleaner.
2.  CSS can and will be edited in one place, which is especially handy for websites with many pages that all share similar styles.

---
# Internal CSS

Tags: #CSS #InternalCSS

Internal CSS **(embedded CSS)** involves adding the CSS within the HTML file itself instead of creating a completely separate file. 

All the rules are placed inside of a pair of opening and closing head tags of the HTML file. 

```css
<head>
	<style>
		div {
			color: red;
			background-color: yellowgreen;
		}
		p {
			color: white;
		}
	</style>
</head>
```

This method can be useful for adding unique styles to a single page of a website, but is really not recommended since the HTML file will get very big and can affect readability in the long run.

---
# Inline CSS

Tags: #CSS #InlineCSS 

Makes it possible to add styles directly to HTML elements.

```html
<body>
  <div style="color: white; 
	  background-color: black;">
	  /* Some elements here*/
  </div>
</body>
```

This is recommended when a **unique style** is added for a single element. 

---
# The Cascade of CSS

Tags: #Cascade

The cascade determines which rules get applied to the HTML. 

## Specificity

Tags: #Specificity

A CSS declaration that is more specific will take precedence over less specific ones.
Specificity will only be taken into account when an element has multiple, conflicting declarations targeting it, sort of like a tie-breaker. 

1. An *ID selector* will always **beat any** *number of class selectors*
2. A *class selector* will **beat any** number of *type selectors*
3. A *type selector* will beat always **beat any** number of less specific selectors

```html
<!-- index.html -->
<div class="main">
  <div class="list subsection">Red text</div>
</div>
```
```css
/* rule 1 */
.subsection {
  color: blue;
}

/* rule 2 */
.main .list {
  color: red;
}
```

In the example above, both rules are using only class selectors, but rule 2 is more specific because it is using more class selectors, so the *color: red;* declaration would take the precedence.

```html
<!-- index.html -->
<div class="main">
  <div class="list" id="subsection">Blue text</div>
</div>
```
```css
/* rule 1 */
#subsection {
  color: blue;
}

/* rule 2 */
.main .list {
  color: red;
}
```

In the example above, despite rule 2 having more class selectors than ID selectors, rule 1 is more specific because ID beats class. In this case, the *color: blue;* declaration would take precedence.

```html
<!-- index.html -->
<div class="main">
  <div class="list" id="subsection">Red text on yellow background</div>
</div>
```
```css
/* rule 1 */
#subsection {
  background-color: yellow;
  color: blue;
}

/* rule 2 */
.main #subsection {
 color: red;
}
```

In the final example above, the first rule uses an ID selector, while the second rule combines an ID selector with a class selector. Therefore, neither rule is using a more specific selector than the other. The cascade then checks the number of each selector type. Both rules have only one ID selector, but rule has a class selector in addition to the ID selector, so rule 2 has a higher specificity.

While the *color: red;* declaration would take precedence, the *background-color: yellow;* declaration would still be applied since there's no conflicting declaration to it.

**Not Everything adds to specificity**
When comparing selectors, we may come across symbols for the universal selector (\*) as well as combinators (+, -, >, and an empty space). These symbols do not add any specificity in and of themselves.

## Inheritance

Tags: #Inheritance #InheritanceInCSS 

Refers to certain CSS properties that, when applied to an element, are inherited by that element's descendants, even if we don't explicitly write a rule for those descendants. 

```html
<!-- index.html -->
<div id="parent">
  <div class="child"></div>
</div>
```
```css
/* styles.css */
#parent {
  color: red;
}

.child {
  color: blue;
}
```

Despite the **parent** element having a higher specificity with an ID, the **child** element would have the **color: blue;** style applied since that declaration directly targets it, while **color: red;** from the parent is only inherited.

## Rule Order

Tags: #RuleOrder

The final factor, the end of the line, the tie-breaker of the tie-breakers. **Whichever rule was the** ***last*** **defined is the winner.**

```css
/* styles.css */
.alert {
  color: red;
}

.warning {
  color: yellow;
}
```

For an element that has both the **alert** and **warning** lasses, the cascade would run through every other factor, including inheritance (none here) and specificity (neither rule is more specific than the other). Since the **.warning** rule was the last one defined, and no other factor was able to determine which rule to apply, it's one that gets applied to the element.

---


