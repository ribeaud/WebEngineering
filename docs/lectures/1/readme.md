name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering

.footnote[<a href="mailto:christian.ribeaud@karakun.com">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## The Internet
]
.right-column[
From [Wikipedia](https://en.wikipedia.org/wiki/Internet):

_The **Internet** is the global system of interconnected computer networks that use the Internet protocol suite (TCP/IP) to link devices worldwide._

![TCP/IP](tcp.jpg "TCP/IP")
]
???
- Transmission Control Protocol/Internet Protocol
---
.left-column[
  ## The Web
]
.right-column[
  The **World Wide Web (WWW)**, or simply **Web**, is a way of accessing information over the medium of the **Internet**.
- WWW = HTML.red[*] + HTTP(S)
- http://info.cern.ch/ (first website)

.footnote[.red[*] including CSS, JavaScript, and other browser enabled contents]
]
???
- WWW created in 1989-91 by Tim Berners-Lee
- Popular web browsers released: Netscape 1994, IE 1995
---
.left-column[
  ## HTML
]
.right-column[
**HyperText Markup Language**: used for writing web pages. It describes the **content** and **structure** of _information_ on a Web page.
- `<!DOCTYPE html>`: must be the very first thing in your HTML document, before the `<html>` tag.
The `<!DOCTYPE>` declaration is not an **HTML** tag; it is an instruction to the web browser about what version of **HTML** the page is written in.
- Element: `<tag>content</tag>`. Example: `<p>This is a paragraph</p>`.
  - _Empty_ element: can be opened and closed in one tag. Example: `<img src="bunny.jpg" alt="bunny" />`.
- Attribute: `<tag name="value">`. Example: `<a href="page2.html">Next page</a>`.
- [Entities](https://www.w3schools.com/charsets/ref_html_entities_4.asp): `&lt;`, `&#x3C;` for **<** 
]
???
- Not the same as the **presentation** (appearance on screen)
- Most whitespace is insignificant in HTML (ignored or collapsed to a single space)
- Current version is **HTML 5**. This is the one we are going to use.
---
.left-column[
  ## Web Standards
]
.right-column[
It is important to write proper **HTML** code and follow proper syntax. Why?

Lookup:
- [World Wide Web Consortium](https://en.wikipedia.org/wiki/World_Wide_Web_Consortium)
- https://validator.w3.org/
- https://www.w3schools.com/
- [selfHTML](https://wiki.selfhtml.org/) (german)
- https://html5test.com/
- [Can I use](https://caniuse.com/)
]
---
.left-column[
  ## Know your readers!
]
.right-column[
- People with browsers
- [Screen readers](https://en.wikipedia.org/wiki/Screen_reader)
- Search Engines
- [Web crawlers](https://en.wikipedia.org/wiki/Web_crawler)
]
---
.left-column[
  ## Key elements
]
.right-column[
- `<html>`
- `<head>`
- `<body>`
- `<title>`
- `<meta>`
- `<h1>`, `<h2>`, ...`<h6>` 
- `<p>`
- `<a>`
- `<img>`
]
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
- `<br />`
- `<hr />`
]
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
  ## Block vs Inline
]
.right-column[
![Block vs. Inline](block_vs_inline.png "Block vs. Inline")

**Block** elements contain an entire large region of content. Examples: paragraphs, lists, tables, ...

**Inline** elements affect a small amount of content. Examples: bold text, images, links, ...

**Inline** elements are NOT allowed to have **block** elements inside.
]
