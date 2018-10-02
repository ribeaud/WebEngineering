# WebEngineering Module, MVC

## Goals

### Abilities
- Writing tests for page navigation
- Writing tests for form submission
- Implementing basic workflow: form - controller - view
- Constructing html views with derived content

### Knowledge
- Understanding the purpose and benefit of functional tests on the web
- Understanding the purpose and benefit of unit tests
- Understanding the web MVC cycle, request-response paradigm
- Using models for request data binding and response view creation

## Assignment 1

1. Make sure that you have a Java **JDK 1.8** installed and `JAVA_HOME` set appropriately. Check by running `java -version`
1. Fork and clone the boilerplate project located at https://github.com/Dierk/WebEngineering-HS18.
1. Import the project into **IntelliJ IDEA** as described on project's [README.md](https://github.com/Dierk/WebEngineering-HS18) page
1. Run the automatically loaded run configuration and browse to http://localhost:8080/static/GradeCalculator.html.

## Assignment 2

1. Write a test, that goes to http://www.fhnw.ch and clicks on any link of the navigation bar.
2. Validate the page title.

## Assignment 3

Checkout branch _feature/calculator_ (`git checkout feature/calculator`) and have a look at:

- `http://localhost:8080/static/GradeCalculator.html`
- `src/main/resources/public/GradeCalculator.html`
- `src/test/groovy/mvc/CalculatorControllerSpec.groovy`
- `src/integration-test/groovy/mvc/CalculatorSpec.groovy` (note line 26 with _placeholder goes here_)
- `grails-app/controllers/mvc/CalculatorController.groovy`
- `grails-app/views/calculator/CalculatorOutput.gsp` (note the _output_ placeholder)

Use `${result}` in **CalculatorOutput.gsp** to put that calculated result in the right place. Verify that the test is still green.

## Assignment 4

In the GradeCalculator:
what happens when _en_ or _exam_ do not represent numbers?

Extend the integration test to cover the invalid input scenario.

## Assignment 5

What happens when _en_ or _exam_ do not fall into 1.0 - 6.0?

Write down how you would address this issue.
Unit test or integration test?
Which code needs change: test, controller, view?
