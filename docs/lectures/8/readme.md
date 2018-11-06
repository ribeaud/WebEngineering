# WebEngineering Module, Services

## Goals

### Abilities
- Being able to use simple services from both client (smart view) and server (controller).
- Implementing the full range of REST services for a persistent Grails domain model.

### Knowledge
- Understanding REST principles on top of HTTP verbs.

## Resources

Seven keys
- https://www.theguardian.com/technology/2014/feb/28/seven-people-keys-worldwide-internet-security-web
- https://www.icann.org/news/blog/the-problem-with-the-seven-keys

Robustness principles
https://en.wikipedia.org/wiki/Robustness_principle

REST
- By Roy Fielding: http://www.ics.uci.edu/~fielding/pubs/dissertation/top.htm
- Best practices: https://restfulapi.net/resource-naming/

REST in Grails
- http://docs.grails.org/latest/guide/webServices.html
- http://guides.grails.org/rest-hibernate/guide/index.html
- https://docs.grails.org/latest/guide/REST.html

Rest docs usage
https://github.com/jlstrater/grails-spring-restdocs-example

## Homework recap

Going through the proposed solution for Booking requests.

## Demo / Live-coding

- Go to the static page Pictures.html
- Work through the JavaScript solution to fetch flickr photos.

- Show how to expose Grails domain classes and controller actions
  as REST endpoints with @Resource and "respond".

## practical work

- Extend the solution to fetch the next 10 photos when needed.

## Homework

Finish the practical work

By following the approach of the practical work from above,
change the search page for the Room reservation app such that
a click on a link shows the results not in a new page but
right in the search page itself.
You will also need to prepare the respective Booking controller
if you want to fetch the booking data as JSON.
