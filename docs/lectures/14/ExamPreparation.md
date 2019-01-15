### HTML
* Play around with https://validator.nu/
* Global attributes
* Custom data attributes
* Exercises at https://www.w3schools.com/html/exercise.asp
* Entities, `&nbsp;`, ...
* `the cat is <strong>mine</strong>` vs. `the <strong>cat</strong> is mine`.
* Semantic elements = elements with a meaning. Many web sites contain HTML code like: `<div id="nav">`, `<div class="header">` `<div id="footer">``
to indicate navigation, header, and footer. Why?
  1. Accessibility
  1. OS integration
  1. Search engine optimisation
* **Block** elements (_A block-level element always starts on a new line and takes up the full width available (stretches out to the left and right as far as it can)._) vs **inline** elements (_An inline element does not start on a new line and only takes up as much width as necessary_)
* Metadata will not be displayed on the page, but will be machine parsable. `<meta name="viewport" content="width=device-width, initial-scale=1.0">`

### CSS
* https://jsfiddle.net/6r5mqhj3/
* https://jsfiddle.net/c18er6zq/
* https://www.w3schools.com/css/tryit.asp?filename=trycss_boxmodel_width.
When you set the width and height properties of an element with CSS, you just set the width and height of the content area. To calculate the full size of an element, you must also add padding, borders and margins.
* Margins collapse: http://jsfiddle.net/blinkmacalahan/RHrxL/

### MVC
* Integration tests vs. Unit tests
* https://github.com/ribeaud/WebEngineering-HS18/blob/feature/inplacecalculator/src/integration-test/groovy/mvc/CalculatorSpec.groovy

### Server Pages
* **Template**: der View muss eine Tabelle mit einer fixen Anzahl von Spalten darstellen. Alle Zeilen haben die gleich Struktur (bing!), die Werte sind aber unterschiedlich.
* **Layout**: https://gsp.grails.org/latest/guide/layouts.html
* **Taglib**: http://guides.grails.org/grails-taglib-wyswyg-trix/guide/index.html

### REST
* https://medium.com/@suhas_chatekar/why-you-should-use-the-recommended-http-methods-in-your-rest-apis-981359828bf7

### Security
* `Requestmap` vs `Annotation` vs `interceptUrlMap` (More on https://grails-plugins.github.io/grails-spring-security-core/latest/)

