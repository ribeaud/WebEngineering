name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering
## Security

.footnote[<a href="mailto:dierk.koenig@fhnw.ch">Prof. Dierk König</a><br /><a href="mailto:christian.ribeaud@fhnw.ch">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## Authenti-cation
]
.right-column[
Authentication is the process of verifying who you are.

When you log on to a PC with a user name and password you are _authenticating_.
]
---
.left-column[
  ## Authenti-cation
  ## Authori-zation
]
.right-column[
Authorization is the process of verifying that you have access to something.

Gaining access to a resource (e.g. directory on a hard disk) because the permissions configured on it allow you access is _authorization_.
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
The **Spring Security** plugin uses an _authority_ class to represent a user’s role in the application
(consider _authority_ and _role_ as the same concept for now).

In general this class restricts URLs to users who have been assigned the required access rights.

A user can be granted multiple roles to indicate various access rights in the application, and should have at least one.
]
???
- https://www.baeldung.com/spring-security-granted-authority-vs-role
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
  ## s2-quickstart
]
.right-column[
Creates a user and role class (and optionally a `Requestmap` class) in the specified package.
See [here](https://grails-plugins.github.io/grails-spring-security-core/latest/#s2-quickstart).
]
---
.left-column[
  ## Grails CLI
  ## s2-quickstart
  ## Mappings
]
.right-column[
You can choose among the following approaches to configuring request mappings for secure application URLs.

The goal is to map URL patterns to the roles required to access those URLs.

- `@Secured` annotations (default approach)
- A simple Map in _application.groovy_
- Requestmap domain class instances stored in the database
]
---
template: inverse

## Exercises
---
.left-column[
  ## Demo/Live-coding
]
.right-column[
The following exercise is based on project https://github.com/ribeaud/RoomReservation (branch _solution_ as starting point).

1. Adapt _build.gradle_ with following change (without it **s2-quickstart** plugin will NOT be available):
```groovy
dependencies {
   ...
   compile 'org.grails.plugins:spring-security-core:4.0.0'
   ...
}
```
1. `./grailsw s2-quickstart roomreservation User Role` (branch _s2-quickstart_)
1. Add some controllers and implement first accesses (branch _security_usage_)
1. Add logout button (branch _security_logout_)
1. Debugging security (branch _security_debugging_)
]
???
- _security_debugging_: play with _/h2-console_ and _passwordEncoder_
---
.left-column[
  ## Exercises
]
.right-column[
- Make `/h2-console` _publicly_ accessible
- How are passwords stored in the database? (look for `UserPasswordEncoderListener`)
- Current user and logout on _main.gsp_ using `<sec:ifLoggedIn>`
- Setup a new user `admin` which has role `ROLE_ADMIN`
- Make users manageable for principals having role `ROLE_ADMIN`
- How to beautify the login view (`login/auth.gsp`)?
]
???
- See as well: https://github.com/Dierk/WebEngineering-HS18/commits/dk_security
---
template: inverse

## Links
---
.left-column[
  ## Links
]
.right-column[
- [Eine kurze Frage an T-Mobile Österreich endete für den Mobilfunkanbieter im Fiasko](https://www.watson.ch/digital/online-sicherheit/521968741-eine-frage-an-den-t-mobile-kundendienst-endete-fuer-den-mobilfunkanbieter-im-fiasko)
- [Grails Basic Auth](http://guides.grails.org/grails-basicauth/guide/index.html)
- [How to do user login, logout and signup in GRAILS 3](https://www.youtube.com/watch?v=nOxeKwGoMf4)
- [Spring Security Core Plugin](http://grails-plugins.github.io/grails-spring-security-core/latest)
]
