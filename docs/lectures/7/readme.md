# WebEngineering Module, Persistence

## Goals

### Abilities
- From a greenfield, being able to use a relational database with _create-read-update-delete_ (**CRUD**)
  functionality in a webapp. 
- Use of simple entities, _many-to-one_, and _many-to-many_ relations.   

### Knowledge
- Understanding **Grails** domain classes as simple entities.
- Understanding **Grails** domain classes with references as relations.
- Understanding dynamic finder methods.

## Resources

http://docs.grails.org/latest/guide/GORM.html

## Homework recap

Going through the proposed solution for `MultiplicationCircle`, 
incl. **JavaScript** for more convenient value changes.

## Demo / Live-coding

- Creating a room reservation system
- Domain classes: `Room`, `Person`, `Booking` (very simple)
- Static scaffolding 
- Setting up bootstrap data
- Use Controller actions to interact with the domain model

## practical work

- create an action that displays all bookings of a given person
- create an action that displays all available rooms for a requested time slot today

## Homework 

Finish the practical work

Build on the practical work from above to 
create a full Web MVC-Cycle (without scaffolding) that shows

- all bookings from today until eternity for a given person
- all available rooms for a requested day and time slot