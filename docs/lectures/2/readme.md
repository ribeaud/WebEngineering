name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering
## CSS

.footnote[<a href="mailto:dierk.koenig@fhnw.ch">Prof. Dierk König</a><br /><a href="mailto:christian.ribeaud@fhnw.ch">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## CSS
]
.right-column[
- **C**ascading **S**tyle **S**heet
- Contains the rules for the _presentation_ of **HTML**
- **CSS** + **HTML** = **Web Page**
- One **HTML** Page - Multiple Styles!
]
???
- Separation of concerns: **CSS** (_presentation_) vs. **HTML** (_content_)
- https://www.w3schools.com/css/css_intro.asp
---
.left-column[
  ## CSS Rule
]
.right-column[
![fh_css_rule](css_rule.png "CSS Rule")
]
---
.left-column[
  ## CSS Selectors
  ### element
]
.right-column[
### CSS
```css
div {
  text-align: center;
  color: red;
}
```
### HTML excerpt
```html
<div>Hello</div>
<div>Again</div>
<p>
  <div>Enjoying the day...</div>
</p>
```
]
???
- https://jsfiddle.net/a5bw10Lf/
---
.left-column[
  ## CSS Selectors
  ### element
  ### id
]
.right-column[
### CSS
```css
#flower {
  text-align: center;
  color: red;
}
```
### HTML excerpt
```html
<div id="flower">rose</div>
<div id="language">JavaScript</div>
```
]
---
.left-column[
  ## CSS Selectors
  ### element
  ### id
  ### class
]
.right-column[
### CSS
```css
.center {
  text-align: center;
  color: red;
}
```
### HTML excerpt
```html
<div class="center">center</div>
<div class="left">left</div>
<footer class="center">
&copy; Karakun AG
</footer>
```
]
???
- Could be a list like `right top`
- `*` selects **all** elements
---
.left-column[
  ## Special Selectors
  ### attribute
]
.right-column[
### CSS
```css
[title] {
  text-align: center;
  color: red;
}
```
### HTML excerpt
```html
<div title="My Div">One</div>
<div title>Two</div>
<div class="left">left</div>
```
]
---
.left-column[
  ## Special Selectors
  ### attribute
  ### attribute/value
]
.right-column[
### CSS
```css
[title="x"] {
  text-align: center;
  color: red;
}
```
### HTML excerpt
```html
<div title="x">One</div>
<div title>Two</div>
<div class="left">left</div>
```
]
???
- `^=`, `$=`, `*=`, `~=`
---
.left-column[
  ## Special Selectors
  ### attribute
  ### attribute/value
  ### pseudo-class
]
.right-column[
### CSS
```css
div:hover {
  color: red;
}
```
### HTML excerpt
```html
<div title="x">One</div>
<div title>Two</div>
<div>left</div>
```
]
???
- `:first-child`
---
.left-column[
  ## Combinators
  ### next sibling
]
.right-column[
### CSS
```css
p + em {
  color: red;
}
```
### HTML excerpt
```html
<p><em>Some text</em></p>
<em>Another text</em><br />
<em>Is this red?</em>
```
]
---
.left-column[
  ## Combinators
  ### next sibling
  ### all siblings
]
.right-column[
### CSS
```css
p ~ em {
  color: red;
}
```
### HTML excerpt
```html
<p><em>Some text</em></p>
<em>Another text</em><br />
<em>Is this red?</em>
```
]
---
.left-column[
  ## Combinators
  ### next sibling
  ### all siblings
  ### descendant
]
.right-column[
### CSS
```css
p em {
  color: red;
}
```
### HTML excerpt
```html
<p><em>Some text</em><br /><em>Some text</em></p>
<em>Another text</em><br />
<em>Is this red?</em>
```
]
---
.left-column[
  ## Combinators
  ### next sibling
  ### all siblings
  ### descendant
  ### direct child
]
.right-column[
### CSS
```css
p > em {
  color: red;
}
```
### HTML excerpt
```html
<p><em>Some text</em><br /><em>Some text</em></p>
<em>Another text</em><br />
<em>Is this red?</em>
```
]
???
- [Video](CSS_Combinator_Selectors.mp4)
---
.left-column[
  ## More ...
  ### union
]
.right-column[
### CSS
```css
span, h3 {
  color: red;
}
```
### HTML excerpt
```html
<p>This text is <span>red</span></p>
<h2>That one is NOT red</h2>
<h3>This header is red as well</h3>
```
]
---
.left-column[
  ## More ...
  ### union
  ### element with class
]
.right-column[
### CSS
```css
h2.red {
  color: red;
}
```
### HTML excerpt
```html
<h2 class="red">This header is red</h2>
<h2>This header is black (default)</h2>
```
]
---
.left-column[
  ## More ...
  ### union
  ### element with class
  ### element with attribute
]
.right-column[
### CSS
```css
h2[red] {
  color: red;
}
```
### HTML excerpt
```html
<h2 red="true">This header is red</h2>
<h2>This header is black (default)</h2>
```
]
???
- Is that valid?
---
.left-column[
  ## Adding CSS
  ### inline
]
.right-column[
- An _inline_ **CSS** is used to apply an unique style to a single **HTML** element.
- An _inline_ **CSS** uses the style attribute of a **HTML** element.
```html
<p style="font-size:20px">Lorem ipsum dolor sit
amet, consectetur adipiscing elit.</p>
```
]
---
.left-column[
  ## Adding CSS
  ### inline
  ### internal
]
.right-column[
- An _internal_ **CSS** is used to define a style for a single **HTML** page.
- An _internal_ **CSS** is defined in the `<head>` section of an **HTML** page, within a `<style>` element
```html
<head>
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>
</head>
```
]
---
.left-column[
  ## Adding CSS
  ### inline
  ### internal
  ### external
]
.right-column[
- An _external_ style sheet is used to define the style for many **HTML** pages.
- With an _external_ style sheet, you can change the look of an entire web site, by changing one file!
```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```
]
???
- The `@import` rule allows you to import a style sheet into another style sheet (see https://way2tutorial.com/css/how_to_write_css_style.php#import_css_style)
- Exercises on https://www.w3schools.com/css/css_exercises.asp
---
.left-column[
  ## Precendence
]
.right-column[
1. _Inline_ overrides **CSS** rules in `<style>` tag and **CSS** file.
1. A _more_ specific selector takes precedence over a _less_ specific one.
1. Rules that appear later in the code override earlier rules if both have the same specificity.
1. A **CSS** rule with `!important` always takes precedence.
]
---
.left-column[
  ## Abilities
]
.right-column[
- Styling of **HTML** pages with respect to appearance and layout
- Being able to use **CSS** rules creatively
- Avoiding duplication in style information
- Separating _what_ from _how_
- Writing maintainable web documents
]
---
.left-column[
  ## Knowledge
]
.right-column[
- Basic selectors: _element_, _class_, _id_
- Selector combinations: collection, descendant, child
- Sourcing: inline, style element, link element
- Basic knowledge of cascading and specificity
- CSS box model
- Basic knowledge of CSS units
]

