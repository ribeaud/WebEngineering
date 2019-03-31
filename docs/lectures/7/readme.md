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
  ## 3-tier architecture
]
.right-column[
![fh_three_tier_architecture](three_tier_architecture.png "Three Tier Architecture")
]
---
.left-column[
  ## Server with service
]
.right-column[
![fh_server_with_service](server_with_service.png "Server With Service")
]
---
.left-column[
  ## Smart UI with service
]
.right-column[
![fh_smart_ui_with_service](smart_ui_with_service.png "Smart UI With Service")
]
---
.left-column[
  ## REST API
]
.right-column[
- https://www.flickr.com/services/api/request.rest.html
- Get a key (for now use following one `865ae530a7dbb28c085dee3ef95e9986`)
]
---
.left-column[
  ## REST call
  ### REST client
]
.right-column[
![fh_rest_client](rest_client.png "REST client")
]
---
.left-column[
  ## REST API
  ### REST client
  ### Response
]
.right-column[
![fh_rest_call_result](rest_call_result.png "REST call result")
]
---
.left-column[
  ## Abilities
]
.right-column[
- Being able to use simple services from both client (smart view) and server (controller).
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