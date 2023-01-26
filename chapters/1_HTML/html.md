# HTML 
* Hypertext Markup Language
* Hypertext - uses http portion of internet markup -> code you write is annotated with keywords -> browser reads keywords and produces visual stuff
* language - is human readable aswell, has some rules
* it is a sequence of tags that tell browsers how to make or show a webpage
* standard markup language for creating web pages and web apps (together with CSS and JS to create the foundation of the web)

# HTML Elements

* unit of content - HTML element
* basic structure of element: 

```
<p class="dog"> content </p>
```

1. The opening tag
2. The content (between the opening and closing tags). Only this is displayed
3. Closing tag - end of element 
4. (optional) The attribute name and value


2 types of tags:
* block elements
  *  structure the main parts of the page
  * `<p>`, lists (`<ul>`, `<ol>`), headings(`<h1>` to `<h6>`), article `<article>`, section `<section>`, long quotes `<blockquotes>`
* inline elements
  * differentiate part of a text, to give it particular function or meaning (usually one/a few words)
  * `<a>`, emphasized words `<em>`, important words `<strong>`


# Attributes 

* additional info about an element
* always specified in start tag
* id, src, href 
* come in name/value pairs `name="value"`
* links
  * web was initially designed to be an information network of documents "linked" between each other 
  * HTML "HyperText" defines what kind of links we use: hypertext links, a.k.a hyperlins
  * `href` - hyperlink reference
  * 3 types of link destinations
   * anchor targets (same page)
   * relative URLs (same website)
   * absolute URLs (different website)
  * specify the relationship between the current and linked document with the `rel` attribute
  * specify where to open the linked document with the `target` attribute

# DOM 
* document object model (the model our web document is presented as)
* tree structure 


# HTML DOCUMENTS

* let them know you are using html with the document type declaration: 
* html files require certain elements to set up the document properly

```<!DOCTYPE html>```

* is an instruction, must be the first line of code
* what type of document to expect, version of HTML (html5 with the above)
* prevents browser from going into [quirks mode](https://developer.mozilla.org/en-US/docs/Web/HTML/Quirks_Mode_and_Standards_Mode)

## The Head 

1. Declared to the browser that your code is HTML with `<!DOCTYPE html>`
2. Added the HTML element `<html>` that will contain the rest of the code
3. the `<head>` goes above the `<body>` element

## Metadata

* contained in `<head>` 
* information about the page that isn't displayed directly on the web page
* unlike information in the `<body>`, the metadata in the head is information about the page itself 

## Title 

* a browser's tab displays the title specified in the `<title>` tag (always inside the `<head>`)

## Body
 
* text, images and buttons can be added to the body

## Hierarchy 

* HTML is organized as a collection of family tree relationships
* element contained inside another element -> child of that element
* child element is nested inside the parent element
* relationships between elements and their ancestors and descendents is known as hierarchy
* child elements can inherit behavior and styling from their parent element

## Semantic elements

* structure elements allow you to organize the main parts of the page
* a typical webpage can include: 
  * `<header>` as the first element
  * `<nav>` as a list of links that go to different pages of the website
  * `<h1>` as the title of the page
  * `<article>` as the main content 
  * `<footer>` as the last element fo the page 

## Forms

* forms in real life - write down info and give it to someone to process
* HTML `<form>` element is responsible for collecting info to send somewhere else
* forms are the "money pages" - how e-commerce sites sell their products etc

### Input types, select and text area

* text, checkbox and radio button forms are spcfieid by an `input type`

```
<!-- A text input -->
<input type="text" />
<!-- A checkbox -->
<input type="checkbox" />
<!-- A radio button -->
<input type="radio" />
```

* a dropdown menu can be created usng `select`

```
<label for="color-select">Choose a color:</label>

<select id="color-select">
  <option value="">--Please choose an option--</option>
  <option value="blue">Blue</option>
  <option value="red">Red</option>
  <option value="green">Green</option>
  <option value="yellow">Yellow</option>
  <option value="orange">Orange</option>
  <option value="pink">Pink</option>
</select>
```

* `textarea` creates a more free-form text field 

```
<label for="learn">What do you hope to learn today?</label>

<textarea id="learn" name="learn" rows="5" cols="30">
I hope to learn about...
</textarea>
```
