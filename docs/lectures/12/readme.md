name: inverse
layout: true
class: center, middle, inverse
---
# Web Engineering
## Deployment

.footnote[<a href="mailto:dierk.koenig@fhnw.ch">Prof. Dierk König</a><br /><a href="mailto:christian.ribeaud@fhnw.ch">Christian Ribeaud</a>]
---
layout: false
.left-column[
  ## Classroom (lecturer)
]
.right-column[
To access the **AWS** classrom, perform following steps:
1. Login to https://awseducate.com/.
1. Click on **MY CLASSROOMS**. This link is ONLY present on the dashboard (click on the top-left corner if you've already used the navigation bar).<br />![fh_250_my_classrooms](my_classrooms.png "My Classrooms")
1. Go to the appropriate classroom.<br />![fh_250_go_to_classroom](go_to_classroom.png "Go To Classroom")
1. Select your class. You will find there the link to **AWS** console.<br />![fh_250_my_classes](my_classes.png "My Classes").
]
---
.left-column[
  ## Three Options
]
.right-column[
1. Upload WAR file to **Java** web server, e.g. **Tomcat** via _manager-gui_
1. Upload _fat_ JAR file to a **PaaS** provider
1. Upload executable to an **IaaS** provider (upload to a provided/available VM)
]
---
.left-column[
  ## Preparation
]
.right-column[
### Adapt grails-app/conf/application.yml
~~none~~ should become **create**
```yml
production:
  dataSource:
    dbCreate: create
```
Only on first deployment!
]
---
.left-column[
  ## Tomcat
]
.right-column[
1. Install **Java**
1. Install **Tomcat** up to a tutorial found in the Internet (I've used `brew install tomcat`)
1. Make sure you've set an user having role _manager-gui_ (you have to adapt `tomcat-users.xml` file)
1. Generate the WAR (`./grailsw war` or `./gradlew assemble`)
1. Upload WAR file via _manager-gui_

![fh_tomcat](tomcat.png "Tomcat")
]
---
.left-column[
  ## PaaS
]
.right-column[
Upload WAR file to a _Platform-as-a-Service_ (**PaaS**) provider, e.g. [Elastic Beanstalk](https://aws.amazon.com/elasticbeanstalk/)

![fh_beanstalk](beanstalk.png "Elastic Beanstalk")
]
???
http://guides.grails.org/grails-elasticbeanstalk/guide/index.html
---
.left-column[
  ## IaaS
]
.right-column[
1. Install **Java8** on the target VM
1. Upload WAR to the provisioned/prepared VM using tools like [scp](https://en.wikipedia.org/wiki/Secure_copy)
1. This WAR is executable as well. Start the application with `java -jar <my-war>`
]
---
.left-column[
  ## Web Atrocities
]
.right-column[
- Care for your data (download, backup)
- Data harvesting
- Data protection
- Forgetful data
- Denial of Service attacks, Spamming
- Proper Password handling, encryption
- Logging, Monitoring
- Localization  formats, timezones, character encoding
]
---
.left-column[
  ## Abilities
]
.right-column[
  Being able to deploy to an open **PaaS** provider.
]
---
.left-column[
  ## Knowledge
]
.right-column[
Knowing some of the atrocities and difficulties that come
with being on the web.

### Atrocities when running on the web

DDoS, spam, captcha, password storage, lost passwords, content encoding
harvesting, logging, monitoring, (locale, time zones, character encodings)
data protection, forgetful data
]
