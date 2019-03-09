name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering
## Server Pages

.footnote[<a href="mailto:dierk.koenig@fhnw.ch">Prof. Dierk König</a><br /><a href="mailto:christian.ribeaud@fhnw.ch">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## Technology Overview
]
.right-column[
- [Grails](https://grails.org/)
- [Groovy](http://groovy-lang.org/)
- [Geb](http://www.gebish.org/) and [Spock](http://spockframework.org/)
- [Gradle](https://gradle.org/)
- [Spring Boot](https://spring.io/projects/spring-boot)
]
---
.left-column[
  ## The story so far
]
.right-column[
* Static Pages: **HTML**, **CSS**
* **MVC**: _Model_, _View_, _Controller_
]
---
template: inverse
# Page structure: 4 ways!
---
.left-column[
  ## GSP
]
.right-column[
- Server pages with values
- [Documentation](https://gsp.grails.org/)
- Example:
```gsp
<!DOCTYPE html>
<html>
<head>
    <meta name="layout" content="main"/>
    <title>Render Domain</title>
</head>
<body>
Last Name: ${person.lastName} <br/>
First Name: ${person.firstName} <br/>
Age: ${person.age} <br/>
</body>
</html>
```
]
---
.left-column[
  ## GSP
  ## Template
]
.right-column[
- **Local** composition.
- Useful for partitioning your views into maintainable chunks.
- Convention: _underscore_ before the name of a view.
- Example:
  - `_bookTemplate.gsp`:
```gsp
<div class="book" id="${book?.id}">
   <div>Title: ${book?.title}</div>
   <div>Author: ${book?.author?.name}</div>
</div>
```
  - Usage:
```gsp
<tmpl:bookTemplate book="${myBook}" />
```
]
---
.left-column[
  ## GSP
  ## Template
  ## TagLib
]
.right-column[
- **Global** composition.
- [Documentation](https://gsp.grails.org/latest/guide/taglibs.html)
- **Groovy** class that ends with the convention `TagLib`
- Example:
  - `grails-app/taglib/SimpleTagLib.groovy`:
```gsp
class SimpleTagLib {
  def emoticon = { attrs, body ->
    out << body() << (attrs.happy == 'true' ?
      " :-)" : " :-(")
  }
}
```
  - Usage:
```gsp
<g:emoticon happy="true">Hi John</g:emoticon>
```
]
---
.left-column[
  ## GSP
  ## Template
  ## TagLib
  ## Layout
]
.right-column[
- **Inverse** composition.
]
---
.left-column[
  ## Abilities
]
.right-column[
- Being able to use dynamic content in **Server Pages**
- Using _pages_, _templates_, _taglibs_, and _layouts_
- Testing appropriately
]
---
.left-column[
  ## Knowledge
]
.right-column[
- Understanding the _request-response_ cycle
- Understanding the four ways of composing **Server Pages** plus when to use which
- Where and how to validate
- Optional: using **Grails** internationalized error messages for generic error display
]
