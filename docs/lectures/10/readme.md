name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering
## JavaScript

.footnote[<a href="mailto:dierk.koenig@fhnw.ch">Prof. Dierk König</a><br /><a href="mailto:christian.ribeaud@fhnw.ch">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## JavaScript
]
.right-column[
Where To:
- Code as string (`eval` method)
- **HTML** attribute value (i.e., `onclick` attribute)
- Text content  of `<script>` element
- External **.js** file

To quickly try out some **JavaScript**:
- Developer tools of your browser
- Write a small **HTML** file
- https://jsfiddle.net/
]
---
.left-column[
  ## Event attributes
]
.right-column[
**onclick**, **onmouseover**, **onchange** (_input_ field), ...
```html
<!DOCTYPE html>
<html>
<body>
<h1 onclick="this.innerHTML = 'Ooops!'">
  Click on this text!</h1>
</body>
</html>
```
]
---
.left-column[
  ## Document
]
.right-column[
When an **HTML** document is loaded into a web browser, it becomes a **document object**.

We have following useful methods:
- `document.write(html)`: Writes **HTML** expressions to a document.
- `document.getElementById(id)`: Gets the element with the specified ID.
- `document.querySelector(selector)`: Gets the first element found with given _selector_.
- `document.querySelectorAll(selector)`: Gets all the elements found with given _selector_.

#### Examples

```html
document.querySelector("p.example");
document.querySelector("div > p");
```
]
---
.left-column[
  ## Element
]
.right-column[
In the **HTML** DOM, the **element object** represents an **HTML** element, like `p`, `div`, `a`, `table`, or any other **HTML** element.

We have following useful attributes/methods:

- `element.id // Gets the ID of an element`
- `element.value = newValue; // Set element's value to given new one`
- `element.innerHTML = newContent; // Sets or returns the content of an element`
- `element.classList.add(newStyle); // Adds new style class to list of already present ones`
]
---
.left-column[
  ## Function declaration
]
.right-column[
![fh_function_anatomy](function-anatomy.png "Function Anatomy")
]
---
.left-column[
  ## Engineering Aspects
]
.right-column[
#### Where to put **JavaScript** code:
- _in-line_ only for one-liners
- _in-page_ for **local** functions
- _.js_ files for **cross-page** sharing,  unit testing, [linting](https://en.wikipedia.org/wiki/Lint_%28software%29), tool support, ...
]
---
.left-column[
  ## Abilities
]
.right-column[
- Being able to use **JavaScript** for form validation
- Using **JavaScript** for client-side application logic
- Modularize **JavaScript** code in functions
- Integration testing of pages that use javascript
]
---
.left-column[
  ## Knowledge
]
.right-column[
- Understanding how to use event handling attributes and **JavaScript** code
- Distinguishing between _in-line_, _in-page_, and _.js-file_ code
- Understanding the idea of _scripting_
- Understanding the general differences between **Java** and **JavaScript**
]
---
.left-column[
  ## Resources
]
.right-column[
Basic **JavaScript** objects for use in the browser:
- https://www.w3schools.com/js/
- https://www.codecademy.com/learn/learn-javascript

Favorite **JS** learning resources from [Joel from egghead](https://egghead.io/instructors/joel-hooks):
- https://learnvanillajs.com/roadmap/
- https://learnjavascript.online/
- https://learn.co/courses/introduction-to-javascript
- https://watchandcode.com/p/practical-javascript
- https://javascript.info/
]
---
.left-column[
  ## Demo/Live-coding
]
.right-column[
1. Project [RoomReservation](https://github.com/ribeaud/RoomReservation), branch _services_solution_
1. Start the application and o to the static page _pictures.html_ (http://localhost:8080/static/pictures.html)
1. Work through the **JavaScript** solution to fetch **Flickr** photos
]
---
.left-column[
  ## Practical work
]
.right-column[
- Extend the solution to fetch the next 10 photos when needed.
]
---