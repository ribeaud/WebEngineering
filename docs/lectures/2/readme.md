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
]

???
- Separation of concerns: **CSS** (_presentation_) vs. **HTML** (_content_)
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

