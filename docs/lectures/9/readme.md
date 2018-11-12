name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering
## Security

.footnote[<a href="mailto:christian.ribeaud@fhnw.ch">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## Authenti-cation
]
.right-column[
Authentication is the process of verifying who you are. When you log on to a PC with a user name and password you
are authenticating.
]
---
.left-column[
  ## Authenti-cation
  ## Authorization
]
.right-column[
Authorization is the process of verifying that you have access to something. Gaining access to a resource
(e.g. directory on a hard disk) because the permissions configured on it allow you access is authorization.
]
---
.left-column[
  ## User
]
.right-column[
- `username`
- `password`
- `...`
]
---
.left-column[
  ## User
  ## Role
]
.right-column[
The **Spring Security** plugin uses an _authority_ class to represent a user’s roles in the application.
In general this class restricts URLs to users who have been assigned the required access rights.
A user can be granted multiple roles to indicate various access rights in the application, and should have at least one. 
]
---
template: inverse

## grails s2-quickstart
---
.left-column[
  ## Grails CLI
]
.right-column[
https://docs.grails.org/latest/guide/gettingStarted.html
]
---
.left-column[
  ## Grails CLI
  ## s2-quicktart
]
.right-column[
Creates a user and role class (and optionally a requestmap class) in the specified package.
See [here](https://grails-plugins.github.io/grails-spring-security-core/latest/#s2-quickstart).
]
---
.left-column[
  ## Grails CLI
  ## s2-quicktart
  ## feature/ security
]
.right-column[
Checkout `feature/security` branch (after a `git fetch upstream` if needed).
Have a look at following parts:
- `BootStrap`
- `resources.groovy`
- `application.groovy`
]
---
template: inverse

## Exercises
---
.left-column[
  ## Exercises
]
.right-column[
- Make `/dbconsole` _publicly_ accessible
- Current user and logout on _main.gsp_ using `<sec:ifLoggedIn>`
- Setup a new user `admin` which has role `ROLE_ADMIN`
- Make users manageable for principals having role `ROLE_ADMIN`
]
---
