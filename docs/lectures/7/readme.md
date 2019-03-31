name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering
## Services

.footnote[<a href="mailto:dierk.koenig@fhnw.ch">Prof. Dierk König</a><br /><a href="mailto:christian.ribeaud@fhnw.ch">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## Abilities
]
.right-column[
- Being able to use simple services server (controller).
- Implementing the full range of **REST** services for a persistent **Grails** domain model.
]
---
.left-column[
  ## Knowledge
]
.right-column[
- Understanding **REST** principles on top of **HTTP** verbs.
]
---
.left-column[
  ## Resources
]
.right-column[
**REST**
- By **Roy Fielding**: http://www.ics.uci.edu/~fielding/pubs/dissertation/top.htm
- Best practices: https://restfulapi.net/resource-naming/

**REST** in **Grails**
- http://docs.grails.org/latest/guide/webServices.html
- http://guides.grails.org/rest-hibernate/guide/index.html
- https://docs.grails.org/latest/guide/REST.html

**REST** docs usage
- https://github.com/jlstrater/grails-spring-restdocs-example
]
---
.left-column[
  ## Demo/Live-coding
]
.right-column[
- Show how to expose **Grails** domain classes and controller actions as **REST** endpoints with `@Resource` and `respond`.
]
---
.left-column[
  ## Homework
]
.right-column[
- `SearchPage.gsp`
]
---
.left-column[
  ## Practical work
]
.right-column[
Change the search page for the **RoomReservation** application such that a click on a link shows the results not in a new page but right in the search page itself.

You will also need to prepare the respective `BookingController` if you want to fetch the booking data as **JSON**.
]
---