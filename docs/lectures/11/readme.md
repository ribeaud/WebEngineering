name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering
## Mobile Web

.footnote[<a href="mailto:dierk.koenig@fhnw.ch">Prof. Dierk König</a><br /><a href="mailto:christian.ribeaud@fhnw.ch">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## Responsive Design
]
.right-column[
**Responsive Web Design** is an approach whereby a designer creates a web page that _responds to_ or resizes itself depending on the type of device it is being seen through.

![fh_responsive_design](responsive_design.jpg "Responsive Design")
]
???
- https://github.com/WebEngineering-FHNW/fs19-de-cr-graded-exercise-Humbi1992
---
layout: false
.left-column[
  ## Approaches
]
.right-column[
Prerequisite Knowledge: **HTML**, **CSS**, **JavaScript**, **Web-MVC**
- Flexible layout (**CSS**)
- Media queries (**CSS**)
- Dynamic in-page logic (**HTML**, **JS**)
- Serve different views per capability (**MVC**)
]
---
layout: false
.left-column[
  ## Approaches
  ### Flexible layout
]
.right-column[
Responsive sites use _fluid grids_. All page elements are sized by proportion, rather than pixels. Eventually, you could use [calc](https://www.w3schools.com/cssref/func_calc.asp) method.

From [float](https://www.w3schools.com/css/css_float.asp), to [flex](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) layout (and to [grid](https://css-tricks.com/snippets/css/complete-guide-grid/) layout)

https://jsfiddle.net/86eLnadb/21/
]
???
- https://www.smashingmagazine.com/2017/07/enhancing-css-layout-floats-flexbox-grid/
---
layout: false
.left-column[
  ## Approaches
  ### Flexible layout
  ### Media queries
]
.right-column[
```css
#title { width: 50%; }

@media screen and (max-width: 800px) {
   #title { width: 100%; }
}
```
```html
<link rel="stylesheet" type="text/css" media="screen and
(min-width: 361px) and (max-width: 480px)"
href="landscape.css">
```
#### Media query attributes
max-width, max-device-width, min-width, min-device-width, (height) orientation (portrait, landscape), [min-,max-,device-]aspect-ratio, ...
]
???
- [Media queries examples](https://www.w3schools.com/css/css3_mediaqueries_ex.asp)
- [min-width vs. min-device-width](https://stackoverflow.com/questions/15276218/css-media-queries-min-width-and-min-device-width-conflicting)
---
layout: false
.left-column[
  ## Approaches
  ### Flexible layout
  ### Media queries
  ### Dynamic in-page logic
]
.right-column[
```html
<body onresize="adapt()">

<script>
   function adapt() { …; screen.size … }
</script>
screen vs. window vs. page
```
]
---
layout: false
.left-column[
  ## Approaches
  ### Flexible layout
  ### Media queries
  ### Dynamic in-page logic
  ### View per Capability
]
.right-column[
#### Questions
- How to detect the capability?
- How to change the view?

![fh_request_response](request_response.png "Request - Response")
]
---
layout: false
.left-column[
  ## Demo / Live-coding / Lecture
]
.right-column[
- How to connect with a mobile device to localhost
- Using flexible layout
- Using media queries
- Using Server Pages for mobile views
]
---
layout: false
.left-column[
  ## Practical Work
]
.right-column[
- Make a page of your choice web friendly. Suggestion: in the InPlaceCalculator, make labels not appear left but on top of the input field.
]
---
layout: false
.left-column[
  ## Abilities
]
.right-column[
Being able to make a web experience mobile-friendly.
]
---
layout: false
.left-column[
  ## Knowledge
]
.right-column[
Knowing the four ways of adapting a web presence to varying
device capabilities.
]
