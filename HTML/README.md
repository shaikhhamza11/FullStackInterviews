## [[⬆]](../README.md) HTML5 Interview Questions

#### Q: What is an iframe and how it works? ⭐
**Answer:**
An **iframe** is an **HTML document** which can be embedded inside another HTML page.

**Example**:

```html
<iframe src="https://github.com" height="300px" width="300px"></iframe>
```

#### Q: Explain meta tags in HTML ⭐
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

#### Q: What is the purpose of the alt attribute on images? ⭐
**Answer:**
The `alt` attribute provides alternative information for an image if a user cannot view it. The `alt` attribute should be used to describe any images except those which only serve a decorative purposes, in which case it should be left empty.

#### Q: Write a HTML table tag sequence that outputs the following ⭐
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

#### Q: What were some of the key goals and motivations for the HTML5 specification? ⭐⭐
**Answer:**
HTML5 was designed to replace HTML 4, XHTML, and the HTML DOM Level 2. The key goals and motivations behind the HTML5 specification were to:

* Deliver rich content (graphics, movies, etc.) without the need for additional plugins, such as Flash.
* Provide better semantic support for web page structure through new structural element tags.
* Provide a stricter parsing standard to simplify error handling, ensure more consistent cross-browser behaviour, and simplify compatibility with documents written to older standards.
* Provide better cross-platform support whether running on a PC, Tablet, or Smartphone.

#### Q: What's the difference between an "attribute" and a "property" in HTML? ⭐⭐
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

#### Q: Briefly describe the correct usage of the following HTML5 semantic elements: `<header>`, `<article>`, `<section>`, `<footer>` ⭐⭐
**Answer:**
* `<header>` is used to contain introductory and navigational information about a section of the page. This can include the section heading, the author’s name, time and date of publication, table of contents, or other navigational information.

* `<article>` is meant to house a self-contained composition that can logically be independently recreated outside of the page without losing it’s meaining. Individual blog posts or news stories are good examples.

* `<section>` is a flexible container for holding content that shares a common informational theme or purpose.

* `<footer>` is used to hold information that should appear at the end of a section of content and contain additional information about the section. Author’s name, copyright information, and related links are typical examples of such content.


#### Q: How Can I Get Indexed Better by Search Engines? ⭐⭐
**Answer:**
It is possible to get indexed better by placing the following two statements in the `<HEAD>` part of your documents:

```html
<META NAME="keywords" CONTENT="keyword keyword keyword keyword">
<META NAME="description" CONTENT="description of your site">
```
Both may contain up to 1022 characters. If a keyword is used more than 7 times, the keywords tag will be ignored altogether. Also, you cannot put markup (other than entities) in the description or keywords list.

#### Q: What is Character Encoding? ⭐⭐
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

#### Q: What is the difference between span and div? ⭐⭐
**Answer:**
* `div` is a block element
* `span` is inline element 

For bonus points, you could point out that it’s illegal to place a block element inside an inline element, and that while `div` can have a `p` tag, and a `p` tag can have a `span`, it is not possible for `span` to have a `div` or `p` tag inside.

#### Q: What is a self closing tag?  ⭐⭐
**Answer:**
In HTML5 it is not strictly necessary to close certain HTML tags. The tags that aren’t required to have specific closing tags are called “self closing” tags.

An example of a self closing tag is something like a line break (`<br />`) or the meta tag (`<meta>`). This means that the following are both acceptable:

```html
<meta charset="UTF-8">
...
<meta charset="UTF-8" />
```

#### Q: How can you highlight text in HTML? ⭐⭐
**Answer:**
If you are working with an HTML5 page, the `<mark>` tag can be a quick and easy way of highlighting or marking text on a page:

```html
<mark>highlighted text</mark>
```

To highlight text with just HTML code and support for all browsers, set the background-color style, as shown in the example below, using the <span> HTML tag.
```html
<span style="background-color: #FFFF00">Yellow text.</span>
```

#### Q: Can a web page contain multiple `<header>` elements? What about `<footer>` elements? ⭐⭐⭐
**Answer:**
Absolutely, a web page can contain multiple `<header>` elements and multiple `<footer>` elements. The HTML5 specification allows for multiple `<header>` and `<footer>` elements within a single HTML document.

The `<header>` element typically represents introductory content at the beginning of a section or a page. For instance, a website might have a main `<header>` that contains the site's logo, navigation, and some introductory text, and within various sections or articles, there might be additional `<header>` elements providing more specific information about those sections.

Similarly, `<footer>` elements can be used multiple times within a webpage. Each `<footer>` could contain information related to its specific section, article, or the main footer at the bottom of the page, which might include copyright information, contact details, or additional navigation.

Here's an example:
```html
<!DOCTYPE html>
<html>
<head>
  <title>Multiple Headers and Footers</title>
</head>
<body>

  <header>
    <!-- Main website header with logo and navigation -->
    <h1>Main Header</h1>
    <nav>
      <!-- Navigation links -->
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
      </ul>
    </nav>
  </header>

  <section>
    <header>
      <!-- Section-specific header -->
      <h2>Section Header</h2>
      <p>Additional information about this section</p>
    </header>

    <!-- Section content -->
    <p>Content of the section goes here.</p>
  </section>

  <article>
    <header>
      <!-- Article-specific header -->
      <h2>Article Header</h2>
      <p>Details about the article</p>
    </header>

    <!-- Article content -->
    <p>Content of the article goes here.</p>
  </article>

  <footer>
    <!-- Main website footer -->
    <p>Main Footer - Copyright information</p>
  </footer>

  <footer>
    <!-- Section-specific footer -->
    <p>Section Footer - Additional information</p>
  </footer>

</body>
</html>
```


#### Q: What are `data-` attributes good for? ⭐⭐⭐
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

#### Q: Have you used different HTML templating languages before?
**Answer:**
Yes, ERB, Handlebars and EJS just to name a few. In my opinion, they are more or less the same and provide similar functionality of escaping content and helpful filters for manipulating the data to be displayed. 


#### Q: How do you change the direction of html text? ⭐⭐⭐
**Answer:**
You can change the direction of text in HTML using the dir attribute. The dir attribute specifies the text directionality of an element's content. It accepts two main values:

* ltr: Left-to-right (the default direction for most languages).
* rtl: Right-to-left (used for languages such as Arabic, Hebrew, etc., that are written right-to-left).

Here's an example:
```html
<!DOCTYPE html>
<html>
<head>
  <title>Text Direction in HTML</title>
</head>
<body>

  <p dir="ltr">This text will be displayed left-to-right.</p>

  <p dir="rtl">هذا النص سيتم عرضه من اليمين إلى اليسار.</p>

</body>
</html>
```


#### Q: What is an optional tag? ⭐⭐⭐
**Answer:**
The idea of optional HTML tags: you don't have to write an HTML tag if you can easily infer it from the context.

For instance, there's no point in writing the `<html>` tag. The document is shown in the browser, so we already know it's an HTML document. Similarly, there's no point in wrapping the `<head>` tag around the `<title>` tag, and the `<body>` around the `<for>` or `<p>` tag. Both forms and paragraphs make only sense in the body of an HTML document, so it's easy to infer the `<body>` tag.

#### Q: How do you serve a page with content in multiple languages? ⭐⭐⭐
**Answer:**
You can refer to the [GeeksforGeeks article on serving pages with content in multiple languages](https://www.geeksforgeeks.org/how-to-serve-a-page-with-content-in-multiple-languages/).

#### Q: What is the difference between `<section>` and `<div>`? ⭐⭐⭐
**Answer:**
You can refer to the [GeeksforGeeks article on difference between `<section>` and `<div>` tags in HTML ?](https://www.geeksforgeeks.org/what-is-the-difference-between-section-and-div-tags-in-html/).

#### Q: What does a DOCTYPE do? ⭐⭐⭐
#### Q: Why do I need a doctype and what does it do? ⭐⭐⭐⭐
**Answer:**
The DOCTYPE (Document Type Declaration) is an instruction or a preamble at the beginning of an HTML document that tells the web browser about the version of HTML or XML used in the document.

Its primary purpose is to define the type of document and instruct the browser on how to render the content. It helps the browser understand which rules and specifications to apply when parsing and displaying the web page.

For example, the `<!DOCTYPE html>` declaration at the beginning of an HTML5 document tells the browser that the document is written in HTML5 syntax. This helps the browser to switch into the standards-compliant mode for rendering the page correctly.

DOCTYPE declarations were more critical in older versions of HTML where different browsers had varying levels of support and interpretation. In modern web development, while they remain an essential part of HTML documents for compatibility and standards compliance, the DOCTYPE declaration for HTML5 (`<!DOCTYPE html>`) has simplified things significantly by providing a single, unified mode of rendering for most browsers.

#### Q: Explain almost standard, full standard and quirks mode ⭐⭐⭐
**Answer:**
In the old days, pages were written separately for supporting different browsers. It means that if you were developing a website in the early days of the internet, you would have written code separately for chrome and firefox. To solve this problem, standards were developed by W3C but browsers could not have started supporting the new standards at once as it would have broken most of the websites at that time. Therefore, different rendering modes were developed for supporting new standard-compliant sites as well as old legacy sites.

Layout Engine now uses three different rendering modes in web browsers:

* Quirks modes: Layout emulates non-standard behavior as supported  by old browsers.
* Almost standard modes: A small number of quirks/old behavior are supported while rendering the layout.
* Full standard modes: Layout emulates standard behavior as described by HTML and CSS specifications.


#### Q: When is it appropriate to use the small element? ⭐⭐⭐
**Answer:**
The `<small>` element should not be used for extended spans of text, such as multiple paragraphs, lists, or sections of text. It is only intended for short runs of text. The text of a page listing terms of use, for instance, would not be a suitable candidate for the small element: in such a case, the text is not a side comment, it is the main content of the page.

In this example, the small element is used for a side comment in an article.
```html
<p>Example Corp today announced record profits for the
second quarter <small>(Full Disclosure: Foo News is a subsidiary of
Example Corp)</small>, leading to speculation about a third quarter
merger with Demo Group.</p>
```

#### Q: What is the purpose of cache busting and how can you achieve it? ⭐⭐⭐
**Answer:**
You can refer to the [Cloudinary article on cache busting](https://cloudinary.com/glossary/cache-busting#:~:text=Cache%20busting%20is%20a%20technique,instead%20of%20using%20outdated%20ones.).

#### Q: What is HTML5 Web Storage? Explain `localStorage` and `sessionStorage`. ⭐⭐⭐
#### Q: Describe the difference between a 'cookie', 'sessionStorage' and 'localStorage'. ⭐⭐⭐
**Answer:**
You can refer to the [Free code camp article for understanding how Web storage works](https://www.freecodecamp.org/news/how-web-storage-works/)
You can refer to the [Coding Ninja artice for the difference between a 'cookie', 'sessionStorage' and 'localStorage'.](https://www.codingninjas.com/studio/library/what-are-differences-between-cookie-local-storage-and-session-storage-use-cases-accessibility)

Also you can refer to the [GeekforGeeks article the difference between a 'cookie', 'sessionStorage' and 'localStorage'.](https://www.geeksforgeeks.org/difference-between-local-storage-session-storage-and-cookies/)


#### Q: What are `defer` and `async` attributes on a `<script>` tag? ⭐⭐⭐
#### Q: Describe the difference between `<script>`, `<script async>` and `<script defer>`. ⭐⭐⭐⭐
**Answer:**
You can refer to the [Codedamn article for understanding `defer` and `async` attributes on a `<script>` tag](https://codedamn.com/news/javascript/async-and-defer-in-script-tag)

You can refer to this [article for difference](https://www.greatfrontend.com/questions/quiz/describe-the-difference-between-script-async-and-script-defer)


#### Q: What is the DOM? ⭐⭐⭐
**Answer:**
The Document Object Model (DOM) is the data representation of the objects that comprise the structure and content of a document on the web. This guide will introduce the DOM, look at how the DOM represents an HTML document in memory and how to use APIs to create web content and applications.
You can refer to the [Mozilla article for deep understanding](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)


#### Q: Discuss the differences between an HTML specification and a browser’s implementation thereof. ⭐⭐⭐
**Answer:**
HTML specifications are like the rules of a game, setting standards for how things should work. Browser implementations are how different players interpret and play that game, sometimes with their own twists or interpretations of the rules. The specifications aim for consistency, while browsers may vary in how they follow those rules, resulting in differences in how web pages look or behave across different browsers.

**Key Difference**

1. Purpose:

- Specification: Defines the rules, syntax, and behavior of HTML, aiming for consistency and interoperability across platforms.
- Browser's Implementation: Interprets the specifications to render web content, potentially introducing variations and unique features.

2. Authority:

- Specification: Created and maintained by organizations like W3C or WHATWG, serving as the authoritative guide for HTML standards.
- Browser's Implementation: Developed by browser vendors who interpret the specifications through their rendering engines, leading to potential differences in how features are implemented.

3. Consistency vs. Variations:

- Specification: Aims for consistency across browsers by defining standardized HTML elements and attributes.
- Browser's Implementation: Might interpret the specifications differently, leading to variations in rendering and support for certain features.

4. Evolution:

- Specification: Evolves with new versions to accommodate technological advancements and changes in web development practices.
- Browser's Implementation: Updates its rendering engine to align with new specifications, but updates may not always be immediate or uniform across browsers.

In essence, specifications set the standards and guidelines for HTML, while browsers interpret and implement these standards, sometimes leading to differences in how web pages are displayed or function across different browsers.

#### Q: What are some differences that XHTML has compared to HTML? ⭐⭐⭐
**Answer:**
You can refer to the [GeekforGeeks article for the differences that XHTML has compared to HTML?](https://www.geeksforgeeks.org/difference-between-xhtml-and-html5/)


#### Q: Where and why is the `rel="noopener"` attribute used? ⭐⭐⭐
**Answer:**
You can refer to the [Article for deep understanding](https://www.reliablesoft.net/noreferrer-noopener/)

#### Q: Explain the difference between block elements and inline elements ⭐⭐⭐
**Answer:**
You can refer to the [GeekforGeeks article for the difference between block elements and inline elements](https://www.geeksforgeeks.org/difference-between-block-elements-and-inline-elements/)

#### Q: How do you set IE compatibility mode? ⭐⭐⭐
**Answer:**
Internet Explorer (IE) mode in Microsoft Edge for organizations that still need Internet Explorer 11 for backward compatibility with existing websites but also need a modern browser. This feature makes it easier for organizations to use one browser, for legacy web/apps or for a modern web/app.

#### Q: What's new in HTML 5? ⭐⭐⭐
**Answer:**
You can refer to the [Top 12 html5 features](https://www.browserstack.com/guide/top-html5-features)

**Answer:**


#### Q: What are Web Workers? ⭐⭐⭐
**Answer:**
You can refer to the [Mozilla article for understanding Web workers](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers)

#### Q: Why to use HTML5 semantic tags? ⭐⭐⭐⭐
**Answer:**
You can refer to the [Free code camp article for understanding need of semantic tags](https://www.freecodecamp.org/news/semantic-html5-elements/)


#### Q: What is WebP? ⭐⭐⭐⭐
**Answer:**
The WebP image format from Google promises to replace both JPEG and PNG/GIF with more efficient compression and higher quality. Safari 14 recently added support for the format and it's now supported in all major browsers.

WebP supports lossy compression, like JPEG, where you chose a quality target between 1-100 (usually 75-85 yields nice results) and the image will be compressed. This can introduce artifacts (blocks) in the image but also great file size savings. Like PNG/GIF WebP also supports lossless compression, support for alpha transparancy and animations.

**Using WebP in HTML:**
You can use a WebP image in a normal `<img>` tag, but in browsers that without WebP support the image would be broken.

Instead the `<picture>` tag allows us to specify a list of different image formats as well as versions for dark mode and various resolutions. The browser will pick the most appropriate version and fall back to the image defined in the `<img>` tag if WebP isn't supported:

```html
<picture>
  <source type="image/webp" srcset="dark@1x.webp 1x, dark@2x.webp 2x" media="(prefers-color-scheme: dark)">
  <source type="image/webp" srcset="light@1x.webp 1x, light@2x.webp 2x">
  <source type="image/jpeg" srcset="dark@1x.jpg 1x, dark@2x.jpg 2x" media="(prefers-color-scheme: dark)">
  <source type="image/jpeg" srcset="light@1x.jpg 1x, light@2x.jpg 2x">
  <img src="fallback-light@1x.jpg" alt="describe image content" loading="lazy">
</picture>
```

#### Q: What kind of things must you be wary of when designing or developing for multilingual sites? ⭐⭐⭐⭐
**Answer:**
You can refer to this [article for understanding the kind of things must you be wary of when designing or developing for multilingual sites](https://www.greatfrontend.com/questions/quiz/designing-or-developing-for-multilingual-sites)

#### Q: What is progressive rendering? ⭐⭐⭐⭐
**Answer:**
You can refer to this [article for understanding progressive rendering](What is progressive rendering)

#### Q: What are the building blocks of HTML5? ⭐⭐⭐⭐
**Answer:**
HTML5, the latest version of Hypertext Markup Language, introduces several new elements and attributes while retaining many from previous versions. Some of the fundamental building blocks include:

1. **Semantic Elements:** HTML5 introduced new elements like `<header>`, `<footer>`, `<nav>`, `<article>`, `<section>`, `<aside>`, and `<main>` that provide better structuring and semantics to web pages.

2. **Audio and Video Elements:** `<audio>` and `<video>` tags enable easy embedding of media content, allowing you to include audio and video files directly in web pages.

3. **Canvas:** The `<canvas>` element provides a space where JavaScript can be used to create graphics, animations, and other visual elements dynamically.

4. **New Form Input Types:** HTML5 introduces new input types like `<input type="date">`, `<input type="email">`, `<input type="url">`, etc., which provide better user experience and data validation.

5. **Local Storage:** `<localStorage>` and `<sessionStorage>` allow web applications to store data locally in the user's browser, enabling persistent storage of key-value pairs.

6. **Geolocation:** HTML5 provides the ability to access a user's geographical location through the Geolocation API.

7. **Responsive Design Elements:** Elements like `<picture>`, `<srcset>`, and `<sizes>` aid in creating responsive and adaptable web designs that adjust to various screen sizes and resolutions.

These building blocks, among others, enhance the functionality, accessibility, and user experience of modern web pages.


#### Q: What's the difference between Full Standard, Almost Standard and Quirks Mode? ⭐⭐⭐⭐
**Answer:**
You can refer to this [article for the difference between Full Standard, Almost Standard and Quirks Mode?](https://www.geeksforgeeks.org/difference-between-standards-mode-and-quirks-mode/)


#### Q: Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute. ⭐⭐⭐⭐
**Answer:**
You can refer to this [article for understanding srcset](https://medium.com/@antrp93/why-you-would-use-a-srcset-attribute-in-an-image-tag-3829f3b3af90#:~:text=You%20would%20use%20the%20srcset,performance%20and%20decrease%20data%20wastage%20)


#### Q: What is the purpose of 'main' element? ⭐⭐⭐⭐
**Answer:**
The `<main>` element in HTML5 serves a specific structural purpose within a web page. Its primary role is to encapsulate the main content of the document. Here are some key aspects of the `<main>` element:

- **Semantic Structure:** `<main>` adds semantic meaning to the content by explicitly marking the primary content section of a webpage. It's meant to enclose the central content that is unique to that page, such as the main article, main features, or primary information.

- **Accessibility:** Using `<main>` helps assistive technologies, such as screen readers, to identify and navigate to the main content easily. It aids in better accessibility for users who rely on these technologies.

- **SEO and Document Outlining:** Search engines tend to prioritize content within the `<main>` element when indexing a page, understanding that this section holds the core information. It can contribute to better search engine optimization.

- **Structural Clarity:** It improves the overall structure of the HTML document by clearly delineating what constitutes the primary content area, making it easier for developers and designers to understand the page layout.

Example:

```html
<body>
  <header>
    <!-- Header content -->
  </header>
  
  <nav>
    <!-- Navigation content -->
  </nav>
  
  <main>
    <!-- Main content of the page -->
    <article>
      <!-- Main article or primary content -->
    </article>
  </main>
  
  <aside>
    <!-- Sidebar or supplementary content -->
  </aside>
  
  <footer>
    <!-- Footer content -->
  </footer>
</body>
```

#### Q: Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>` just before `</body>`? Do you know any exceptions? ⭐⭐⭐⭐⭐
**Answer:**
You can refer to [article for understanding](https://www.greatfrontend.com/questions/quiz/css-link-between-head-and-js-script-just-before-body)


#### Q: What is an IndexedDB? ⭐⭐⭐⭐⭐
**Answer:**
- **IndexedDB** is javascript based **object oriented database**.
- **IndexedDB** is useful when we want to store **large amount** of **data** in a web applications.
- **IndexedDB** stores data as **key-value** pair.
- **IndexedDB** is an **asynchronous** API.
- **IndexedDB** is [**supported**](http://caniuse.com/#feat=indexeddb) in **most of browsers**.
 
**Usage:**

- Specify **DB schema**.
- Open a **connection** to **DB**.
- **Adding**, **Retrieval** & **Updating** the data is done within a **series** of **transactions**.   

More information on [API](https://www.tutorialspoint.com/html5/html5_indexeddb.htm)

#### Q. What does HTML Comment looks like ?
**Answer:**
- Comments are not displayed by browser
- But you can check the comments in HTML source code

**Example**:

```html
<!-- Anything inside this is considered as HTML comment -->
```

#### Q. How do you set language in HTML?
**Answer:**

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
#### Q. Why are meta tags used ? What are the meta tags you know?
**Answer:**
You can refer to this [article for understanding meta tags](https://www.geeksforgeeks.org/html-meta-tag/)

#### Q.How can you improve seo just by html tags?
**Answer:**
You can refer to this [article for understanding improving seo using html](https://www.greengeeks.in/blog/html-tags-for-seo/)
