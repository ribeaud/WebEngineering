name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering
## HTML

.footnote[<a href="mailto:dierk.koenig@fhnw.ch">Prof. Dierk König</a><br /><a href="mailto:christian.ribeaud@fhnw.ch">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## The Internet
]
.right-column[
The **Internet** is an enormous global network of billions of servers, computers, and other hardware devices. It is _decentralised_.
]

???
- We need an IP address and some protocols (TCP, email, HTTP, ...)
---
.left-column[
  ## The Web
]
.right-column[
  The **World Wide Web (WWW)**, or simply **Web**, is a way of accessing information over the medium of the **Internet**.
- WWW = HTML.red[*] + HTTP(S)

The **Web** is a _portion_ of the **Internet**.

.footnote[.red[*] including CSS, JavaScript, and other browser enabled contents]
]
???
- WWW created in 1989-91 by Tim Berners-Lee
- We have a standard and we can link to other pages
- Browsers (the first browser designed by Tim Berners-Lee - https://www.w3.org/People/Berners-Lee/WorldWideWeb.html)
---
.left-column[
  ## HTML
]
.right-column[
**HyperText Markup Language**: used for writing web pages. It describes the **content** and **structure** of _information_ on a Web page.
- `<!DOCTYPE html>`: must be the very first thing in your HTML document, before the `<html>` tag.
The `<!DOCTYPE>` declaration is not an **HTML** tag; it is an instruction to the web browser about what version of **HTML** the page is written in.
- Element: `<tag>content</tag>`. Example: `<p>This is a paragraph</p>`.
  - _Empty_ element: can be opened and closed in one tag. Example: `<img src="bunny.jpg" alt="bunny" />` (`<img ...></img>` NOT allowed).
- Attribute: `<tag name="value">`. Example: `<a href="page2.html">Next page</a>`.
- [Entities](https://www.w3schools.com/html/html_entities.asp): `&copy;`, `&#169;` for **©**
]
???
- Not the same as the **presentation** (appearance on screen)
- Most whitespace is insignificant in HTML (ignored or collapsed to a single space).
  What could you use to enforce a space?
- Current version is **HTML 5**. This is the one we are going to use.
- **HTML** is part of a bigger family **SGML** (Standard Generalised Markup Language), like **XML** (Extensible Markup Language)
- **HTML4** starts with `<?xml version="1.0" encoding="UTF-8"?><html xmlns="http://www.w3.org/1999/xhtml">`
---
.left-column[
  ## HTML5
]
.right-column[
![fh_HTML5](html5.jpg "HTML5")

```html
<!DOCTYPE html>
<html>
  <head><title>Title</title></head>
  <body><p>Body</p></body>
</html>
```
]
???
- https://dev.to/ananyaneogi/html-can-do-that-c0n
---
.left-column[
  ## Web Standards
]
.right-column[
It is important to write proper **HTML** code and follow proper syntax. Why?

Lookup:
- [World Wide Web Consortium](https://en.wikipedia.org/wiki/World_Wide_Web_Consortium)
- https://validator.nu/
- https://www.w3schools.com/
- [selfHTML](https://wiki.selfhtml.org/) (german)
- https://html5test.com/
]
???
- W3C is the main international standards organisation for the W3. Founded and currently led by Tim Berners-Lee.
- https://html5test.com/: how well does your browser support html5?
- Why validation?
  - Rendering time
  - Non uniform browser correction
  - Google prefers valid code
  - ...
---
.left-column[
  ## Know your readers!
]
.right-column[
- People with... all kinds of browsers
- [Screen Readers](https://en.wikipedia.org/wiki/Screen_reader)
- [Web Crawlers](https://en.wikipedia.org/wiki/Web_crawler), Search Engines
- OS Integration
- [Web Scrapers](https://en.wikipedia.org/wiki/Web_scraping)
]
???
- Screen readers are for blind people
- Every search engine makes use of a web crawler to index the content of the websites
---
.left-column[
  ## Block vs Inline
]
.right-column[
![Block vs. Inline](block_vs_inline.png "Block vs. Inline")

**Block** elements contain an entire large region of content. Examples: paragraphs, lists, tables, ...

**Inline** elements affect a small amount of content. Examples: bold text, images, links, ...

**Inline** elements are NOT allowed to have **block** elements inside.
]
---
.left-column[
  ## Key elements
]
.right-column[
- `<html>`
- `<head>` (NOT the same than `<header>`!)
- `<body>`
- `<title>`
- `<h1>`, `<h2>`, ...`<h6>` (_block_)
- `<p>`
- `<div>`
- `<span>`
- `<a>` (_inline_): links, or **anchors**, to other pages.
- `<img>` (_inline_)
- `<meta>`: describes meta data of the web page. Metadata will not be displayed on the page, but will be machine parsable.
]
---
.left-column[
  ## Key elements
  ### image
]
.right-column[
```xml
<a href="default.asp" title="Go to W3Schools HTML section">
  <img src="smiley.gif" alt="HTML tutorial" />
</a>
```]
---
.left-column[
  ## Key elements
  ### image
  ### meta
]
.right-column[
  ```xml
  <head>
    <meta charset="UTF-8"><!-- HTML5 specific! -->
    <meta name="description" content="Free Web tutorials">
    <meta name="keywords" content="HTML,CSS,XML,JavaScript">
    <meta name="author" content="John Doe">
    <meta http-equiv="refresh" content="30">
  </head>
  ```
]
???
- Replaces `<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">` (**HTML4** specific)
---
.left-column[
  ## Collections
]
.right-column[
- `<ol>`
- `<ul>`
- `<table>`
]
---
.left-column[
  ## Presentational
]
.right-column[
- `<em>` (`<i>`)
- `<strong>` (`<b>`)
- `<br />` (_inline_): should be immediately closed with `/>`.
- `<hr />` (_block_): horizontal rule. Should be immediately closed with `/>`.
]
???
- `This is <strong>my</strong> cat` vs. `This is my <strong>cat</strong>`
---

.left-column[
  ## Form
]
.right-column[
- `<form>`
- `<input>`
- `<textarea>`
- `<select>`
- `<button>`
]
---
.left-column[
  ## Semantic web
]
.right-column[
**Semantics** is the study of the meanings of words and phrases in a language.

**Semantic** elements = elements with a meaning.

Examples:

- `<nav>`
- `<header>`
- `<footer>`
- `<address>`
- `<article>`
- `<section>`
]
???
- One example at https://gist.github.com/thomd/9220049
- https://www.pluralsight.com/guides/semantic-html
- http://seekbrevity.com/semantic-markup-important-web-design/
- https://internetingishard.com/html-and-css/semantic-html/
- http://glaforge.appspot.com/article/covid-learning-html-semantic-tags
---
.left-column[
  ## DOM
]
.right-column[
Document Object Model

![fh_DOM](dom.png "DOM")
]
???
- https://javascript.info/dom-nodes#see-it-for-yourself
- http://software.hixie.ch/utilities/js/live-dom-viewer/
- https://javascript.info/article/dom-nodes/elks.html in the browser console
---
.left-column[
  ## Which is Which?
]
.right-column[
- `<html><body></html></body>`
- `<html><body  </body></html>`
- `<span><div></div></span>`
- `<p><em>x</em></p>`
- `<p><em>x<p>`
]
---
.left-column[
  ## HTML is forgiving
]
.right-column[
- Unknown tags are ignored
- Unknown attributes are ignored
- ... and browsers display almost anything
]
---
.left-column[
  ## Global attributes
]
.right-column[
- `id`
- `class`
- `style`
- `title`
- `data-*`: The **data-*** attributes is used to store custom data private to the page or application. The **data-*** attributes gives us the ability to embed custom data attributes on all HTML elements.
]
---
.left-column[
  ## Exercises
  ### Assignment 1
]
.right-column[
### Assignment 1

- Extend/change [first.html](first.html) and view in the browser
- Correct [first.html](first.html) to be valid HTML and **validate** your work
- Create a [GitHub](https://github.com/) account
- [Create](https://help.github.com/articles/create-a-repo/) a **GitHub** repository
- Copy [example.html](example.html) into the `/docs` folder of that repo
- Change/adapt _example.html_ document
- Commit and push
- View change in browser
]
---
.left-column[
  ## Exercises
  ### Assignment 1
  ### Assignment 2
]
.right-column[
### Assignment 2

- https://www.w3schools.com/html/html_exercises.asp
- https://www.w3schools.com/html/html_quiz.asp
]
---
.left-column[
  ## Exercises
  ### Assignment 1
  ### Assignment 2
  ### Assignment 3
]
.right-column[
### Assignment 3

- Use semantic elements in [non_semantic.html](non_semantic.html)
![fh_semantic](semantic.jpg "Semantic")
- Investigate the new **HTML5** attributes like _placeholder_ and the new **email**, **url**, and **tel** input types
]
