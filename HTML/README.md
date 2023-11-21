## [[⬆]](../README.md) HTML5 Interview Questions


#### Q1: What is an iframe and how it works? ⭐
**Answer:**
An **iframe** is an **HTML document** which can be embedded inside another HTML page.

**Example**:

```html
<iframe src="https://github.com" height="300px" width="300px"></iframe>
```

#### Q2: Explain meta tags in HTML ⭐
**Answer:**
- **Meta tags** always go inside **head tag** of the HTML page
- **Meta tags** is always passed as name/value pairs
- **Meta tags** are not displayed on the page but intended for the browser
- **Meta tags** can contain information about **character encoding**, **description**, **title** of the document etc,

**Example**:

```html
<!DOCTYPE html>
<html>
<head>
  <meta name="description" content="I am a web page with description"> 
  <title>Home Page</title>
</head>
<body>
  
</body>
</html>
```

#### Q3: What is the purpose of the alt attribute on images? ⭐
**Answer:**
The `alt` attribute provides alternative information for an image if a user cannot view it. The `alt` attribute should be used to describe any images except those which only serve a decorative purposes, in which case it should be left empty.

#### Q4: Write a HTML table tag sequence that outputs the following ⭐
**Answer:**
Write a HTML table tag sequence that outputs the following:
```
50 pcs 100 500
10 pcs 5 50
```

**Answer:**
```html
<table>
  <tr>
    <td>50 pcs</td>
    <td>100</td>
    <td>500</td>
  </tr>
  <tr>
    <td>10 pcs</td>
    <td>5</td>
    <td>50</td>
  </tr>
</table>
```

#### Q5: What were some of the key goals and motivations for the HTML5 specification? ⭐⭐
**Answer:**
HTML5 was designed to replace HTML 4, XHTML, and the HTML DOM Level 2. The key goals and motivations behind the HTML5 specification were to:

* Deliver rich content (graphics, movies, etc.) without the need for additional plugins, such as Flash.
* Provide better semantic support for web page structure through new structural element tags.
* Provide a stricter parsing standard to simplify error handling, ensure more consistent cross-browser behaviour, and simplify compatibility with documents written to older standards.
* Provide better cross-platform support whether running on a PC, Tablet, or Smartphone.

#### Q6: What's the difference between an "attribute" and a "property" in HTML? ⭐⭐
**Answer:**
Attributes are defined on the HTML markup but properties are defined on the DOM. To illustrate the difference, imagine we have this text field in our HTML: `<input type="text" value="Hello">`.

```js
const input = document.querySelector('input');
console.log(input.getAttribute('value')); // Hello
console.log(input.value); // Hello
```

But after you change the value of the text field by adding "World!" to it, this becomes:

```js
console.log(input.getAttribute('value')); // Hello
console.log(input.value); // Hello World!
```

#### Q7: Briefly describe the correct usage of the following HTML5 semantic elements: `<header>`, `<article>`, `<section>`, `<footer>` ⭐⭐
**Answer:**
* `<header>` is used to contain introductory and navigational information about a section of the page. This can include the section heading, the author’s name, time and date of publication, table of contents, or other navigational information.

* `<article>` is meant to house a self-contained composition that can logically be independently recreated outside of the page without losing it’s meaining. Individual blog posts or news stories are good examples.

* `<section>` is a flexible container for holding content that shares a common informational theme or purpose.

* `<footer>` is used to hold information that should appear at the end of a section of content and contain additional information about the section. Author’s name, copyright information, and related links are typical examples of such content.


#### Q8: How Can I Get Indexed Better by Search Engines? ⭐⭐
**Answer:**
It is possible to get indexed better by placing the following two statements in the `<HEAD>` part of your documents:

```html
<META NAME="keywords" CONTENT="keyword keyword keyword keyword">
<META NAME="description" CONTENT="description of your site">
```
Both may contain up to 1022 characters. If a keyword is used more than 7 times, the keywords tag will be ignored altogether. Also, you cannot put markup (other than entities) in the description or keywords list.

#### Q9: What is Character Encoding? ⭐⭐
**Answer:**
To display an HTML page correctly, a web browser must know which character set (character encoding) to use. This is specified in the <meta> tag:

**HTML4:**
```html
<meta http-equiv="Content-Type" content="text/html;charset=ISO-8859-1">
```

**HTML5:**
```html
<meta charset="UTF-8">
```

#### Q10: What is the difference between span and div? ⭐⭐
**Answer:**
* `div` is a block element
* `span` is inline element 

For bonus points, you could point out that it’s illegal to place a block element inside an inline element, and that while `div` can have a `p` tag, and a `p` tag can have a `span`, it is not possible for `span` to have a `div` or `p` tag inside.

#### Q11: What is a self closing tag?  ⭐⭐
**Answer:**
In HTML5 it is not strictly necessary to close certain HTML tags. The tags that aren’t required to have specific closing tags are called “self closing” tags.

An example of a self closing tag is something like a line break (`<br />`) or the meta tag (`<meta>`). This means that the following are both acceptable:

```html
<meta charset="UTF-8">
...
<meta charset="UTF-8" />
```
#### Q12: How can you highlight text in HTML? ⭐⭐
**Answer:**
If you are working with an HTML5 page, the `<mark>` tag can be a quick and easy way of highlighting or marking text on a page:

```html
<mark>highlighted text</mark>
```

To highlight text with just HTML code and support for all browsers, set the background-color style, as shown in the example below, using the <span> HTML tag.
```html
<span style="background-color: #FFFF00">Yellow text.</span>
```

#### Q13: Can a web page contain multiple `<header>` elements? What about `<footer>` elements? ⭐⭐⭐
**Answer:**


#### Q14: What are `data-` attributes good for? ⭐⭐⭐
**Answer:**
data-* attributes allow us to store extra information on standard, semantic HTML elements without other hacks such as non-standard attributes, or extra properties on DOM.
```html
<article
  id="electric-cars"
  data-columns="3"
  data-index-number="12314"
  data-parent="cars">
  …
</article>
```
Reading the values of these attributes out in JavaScript is also very simple. You could use getAttribute() with their full HTML name to read them, but the standard defines a simpler way: a DOMStringMap you can read out via a dataset property.

To get a data attribute through the dataset object, get the property by the part of the attribute name after data- (note that dashes are converted to camel case).

```js
const article = document.querySelector("#electric-cars");
// The following would also work:
// const article = document.getElementById("electric-cars")

article.dataset.columns; // "3"
article.dataset.indexNumber; // "12314"
article.dataset.parent; // "cars"
```


<h4 style="color: red;">Q15: Have you used different HTML templating languages before?</h4>
**Answer:**


#### Q16: How do you change the direction of html text? ⭐⭐⭐
**Answer:**


#### Q17: What is WebSQL? ⭐⭐⭐
**Answer:**


#### Q18: What is an optional tag? ⭐⭐⭐
**Answer:**


#### Q19: How do you serve a page with content in multiple languages? ⭐⭐⭐
**Answer:**


#### Q20: What is the difference between `<section>` and `<div>`? ⭐⭐⭐
**Answer:**


#### Q21: What does a DOCTYPE do? ⭐⭐⭐
**Answer:**


#### Q22: Explain almost standard, full standard and quirks mode ⭐⭐⭐
**Answer:**


#### Q23: When is it appropriate to use the small element? ⭐⭐⭐
**Answer:**


#### Q24: What is the purpose of cache busting and how can you achieve it? ⭐⭐⭐
**Answer:**


#### Q25: Describe the difference between a 'cookie', 'sessionStorage' and 'localStorage'. ⭐⭐⭐
**Answer:**


#### Q26: What are `defer` and `async` attributes on a `<script>` tag? ⭐⭐⭐
**Answer:**


#### Q27: What is the DOM? ⭐⭐⭐
**Answer:**


#### Q28: Discuss the differences between an HTML specification and a browser’s implementation thereof. ⭐⭐⭐
**Answer:**


#### Q29: What are some differences that XHTML has compared to HTML? ⭐⭐⭐
**Answer:**


#### Q30: Where and why is the `rel="noopener"` attribute used? ⭐⭐⭐
**Answer:**


#### Q31: What is HTML5 Web Storage? Explain `localStorage` and `sessionStorage`. ⭐⭐⭐
**Answer:**


#### Q32: What is WebSQL? ⭐⭐⭐
**Answer:**


#### Q33: Explain the difference between block elements and inline elements ⭐⭐⭐
**Answer:**


#### Q34: How do you set IE compatibility mode? ⭐⭐⭐
**Answer:**


#### Q35: What's new in HTML 5? ⭐⭐⭐
**Answer:**


#### Q36: Explain the difference between cookies, session and local storage ⭐⭐⭐
**Answer:**


#### Q37: What are Web Workers? ⭐⭐⭐
**Answer:**


#### Q38: Describe the difference between `<script>`, `<script async>` and `<script defer>`. ⭐⭐⭐⭐
**Answer:**


#### Q39: Why to use HTML5 semantic tags? ⭐⭐⭐⭐
**Answer:**


#### Q40: What is WebP? ⭐⭐⭐⭐
**Answer:**


#### Q41: What kind of things must you be wary of when designing or developing for multilingual sites? ⭐⭐⭐⭐
**Answer:**


#### Q42: What is progressive rendering? ⭐⭐⭐⭐
**Answer:**


#### Q43: What are the building blocks of HTML5? ⭐⭐⭐⭐
**Answer:**


#### Q44: What's the difference between Full Standard, Almost Standard and Quirks Mode? ⭐⭐⭐⭐
**Answer:**


#### Q45: Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute. ⭐⭐⭐⭐
**Answer:**


#### Q46: HTML Markup Validity ⭐⭐⭐⭐
**Answer:**


#### Q47: How would you select svg or canvas for your site? ⭐⭐⭐⭐
**Answer:**


#### Q48: What is an HTML preprocessor and are you using it? ⭐⭐⭐⭐
**Answer:**


#### Q49: Why do I need a doctype and what does it do? ⭐⭐⭐⭐
**Answer:**


#### Q50: What is the purpose of 'main' element? ⭐⭐⭐⭐
**Answer:**


#### Q51: What are Web Components? ⭐⭐⭐⭐⭐
**Answer:**


#### Q52: What is accessibility & ARIA role means in a web application? ⭐⭐⭐⭐⭐
**Answer:**


#### Q53: Could you generate a public key in HTML? ⭐⭐⭐⭐⭐
**Answer:**


#### Q54: Why is it generally a good idea to position CSS <link>s between <head></head> and JS `<script>` just before `</body>`? Do you know any exceptions? ⭐⭐⭐⭐⭐
**Answer:**


#### Q55: What is an IndexedDB? ⭐⭐⭐⭐⭐
**Answer:**
- **IndexedDB** is javascript based **object oriented database**.
- **IndexedDB** is useful when we want to store **large amount** of **data** in a web applications.
- **IndexedDB** stores data as **key-value** pair.
- **IndexedDB** is an **asynchronous** API.
- **IndexedDB** is [**supported**](http://caniuse.com/#feat=indexeddb) in **most of browsers**.
 
### Usage

- Specify **DB schema**.
- Open a **connection** to **DB**.
- **Adding**, **Retrieval** & **Updating** the data is done within a **series** of **transactions**.   

More information on [API](https://www.tutorialspoint.com/html5/html5_indexeddb.htm)

#### Q55. What does HTML Comment looks like ?
**Answer:**
- Comments are not displayed by browser
- But you can check the comments in HTML source code

**Example**:

```html
<!-- Anything inside this is considered as HTML comment -->
```
#### 55. How do you set language in HTML

- There are **multiple ways** to set language in **HTML**
- By setting **content-language** in headers for language of the page
- By setting **accept-language** in headers for list of language that a page accept
- Setting **lang** attribute in **html** tag

**Example**:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Document Title</title>
</head>
<body>

</body>
</html>
```

