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
---
.left-column[
  ## More ...
  ### union
]
.right-column[
### CSS
```css
span, em {
  color: red;
}
```
### HTML excerpt
```html
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
a.red {
  color: red;
}
```
### HTML excerpt
```html
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
a[data-red] {
  color: red;
}
```
### HTML excerpt
```html
```
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

