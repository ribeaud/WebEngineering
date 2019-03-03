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
- https://spring.io/projects/spring-boot
- **Spring Boot** is a project built on the top of the **Spring** framework. It provides a simpler and faster way to set up, configure, and run both simple and web-based applications.
- auto-configuration, standalone, opinionated
- A lot of magic ...
]
---
layout: false
.left-column[
  ## Gradle
]
.right-column[
]
---
layout: false
.left-column[
  ## Exercises
  ### Assignment 1
]
.right-column[
1. Make sure that you have a Java **JDK 1.8** installed and `JAVA_HOME` set appropriately. Check by running `java -version`
1. Fork and clone the boilerplate project located at https://github.com/Dierk/WebEngineering-HS18.
1. Import the project into **IntelliJ IDEA** as described on project's [README.md](https://github.com/Dierk/WebEngineering-HS18) page
1. Run the automatically loaded run configuration and browse to http://localhost:8080/static/GradeCalculator.html.
]
---
layout: false
.left-column[
  ## Exercises
  ### Assignment 1
  ### Assignment 2
]
.right-column[
1. Write a test, that goes to http://www.fhnw.ch and clicks on any link of the navigation bar.
1. Validate the page title.
]
---
layout: false
.left-column[
## Exercises
### Assignment 1
### Assignment 2
### Assignment 3
]
.right-column[
Checkout branch _feature/calculator_ (`git checkout feature/calculator`) and have a look at:

- `http://localhost:8080/static/GradeCalculator.html`
- `src/main/resources/public/GradeCalculator.html`
- `src/test/groovy/mvc/CalculatorControllerSpec.groovy`
- `src/integration-test/groovy/mvc/CalculatorSpec.groovy` (note line 26 with _placeholder goes here_)
- `grails-app/controllers/mvc/CalculatorController.groovy`
- `grails-app/views/calculator/CalculatorOutput.gsp` (note the _output_ placeholder)

Use `${result}` in **CalculatorOutput.gsp** to put that calculated result in the right place. Verify that the test is still green.
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

