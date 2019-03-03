name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering
## MVC

.footnote[<a href="mailto:dierk.koenig@fhnw.ch">Prof. Dierk König</a><br /><a href="mailto:christian.ribeaud@fhnw.ch">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## MVC
]
.right-column[
- **Model-View-Controller**
![fh_500_mvc](mvc.png "MVC")
- Avantages? Disadvantages?
]
???
- **Avantages**:
  - MVC supports rapid and parallel development.
- **Disadvantages**:
  - Increased complexity.
---
layout: false
.left-column[
  ## MVC
  ### Model
]
.right-column[
- Handles data and business logic.
- Interacts with the database (using **SQL**) or perform complex operations.
]
---
layout: false
.left-column[
  ## MVC
  ### Model
  ### View
]
.right-column[
- Presents data to the user in any supported format and layout.
- Could be _static_ **HTML** pages or _dynamic_ server pages.
]
---
layout: false
.left-column[
  ## MVC
  ### Model
  ### View
  ### Controller
]
.right-column[
- Receives user requests and calls appropriate resources to carry them out.
- Validates the input
- Calls the appropriate _model_ for the task and then selects the proper _view_.
]
---
layout: false
.left-column[
  ## Grails
]
.right-column[
- https://grails.org/
- **Groovy**-based web application framework for the **JVM** built on top of **Spring Boot**
- _Convention-over-configuration_ with sensible defaults
]
---
layout: false
.left-column[
  ## Groovy
]
.right-column[
- http://groovy-lang.org/
- https://www.manning.com/books/groovy-in-action-second-edition
- Example:
```java
def transform(List elements, Closure action) {
  def result = []
  elements.each {
    result << action(it)
  }
  result
}
String describe(Person p) {
  "$p.name is $p.age"
}
def action = this.&describe
def list = [
  new Person(name: 'Bob',   age: 42),
  new Person(name: 'Julia', age: 35)]
assert transform(list, action)
    == ['Bob is 42', 'Julia is 35']
```
]
---
layout: false
.left-column[
  ## Spring Boot
]
.right-column[
]
---
layout: false
.left-column[
]
.right-column[
]
---
.left-column[
  ## Abilities
]
.right-column[
- Writing tests for page navigation.
- Writing tests for form submission.
- Implementing basic workflow: _form_ - _controller_ - _view_.
- Constructing **HTML** views with derived content.
]
---
.left-column[
  ## Knowledge
]
.right-column[
- Understanding the purpose and benefit of _functional_ tests on the web.
- Understanding the purpose and benefit of _unit_ tests.
- Understanding the web **MVC** cycle, _request-response_ paradigm.
- Using models for request data binding and response view creation.
]

