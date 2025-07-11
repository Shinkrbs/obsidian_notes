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

An anchor element is defined by wrapping the text or another HTML element we want to be a link using the a tag.

```html
<a> About our Page </a>
```

## HTML Attribute

This is used to tell the anchor where is the destination to go to when it is clicked.  It is always in the opening tag. 

```html
<a href = "thisisalink.com"> The Odin Project </a>
```

---
