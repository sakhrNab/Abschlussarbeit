# Anforderungsanalyse
### Zielsetzung 
By the end of the project it's intended to reach to a decoupled application, which is split into different services. The whole project consisted of all the requirements will be separated into different services, which will be independent from each other, and replaceable.

Each Service will be stored in a container and within each container there will be a running IDE, a specific framework will be implemented, and will work completely fine without the need for the other services. 

The services will then contact with each other using interfaces and if one service needs a resource from another one, it will use this interface to get it, to complete the required task. 


### funktionale Anforderung
êine Funktion was etwas tut.
was ist vom System haben will.
Wartbarkeit, Skalierbarkeit, Qualität, 

### User Stories - Nicht-funktionale Anforderungen
- Als Anwender des Systems möchte ich jede Funktion nach 3 Sekunden bedienen können, um meine Arbeit flüssig zu erledigen.
### Anwendungsumgebung
  - Sammlung von Ressourcen
    - Eine Ressource ist ein Bereitstellungsziel wie eine DB oder ein Java-Platform, Container.
    - Ressourcen befinden sich i.d.R. auf demselben Host wie der Agent, der sie verwaltet. Es kann ein pyhsiches System, eine VM oder cloudbasiert sein.
  - Zusammenstellung von Komponenten
  - In der Phase des Lebenszyklus eines SW-Projketes
    - Bspl: Entwicklung, Qualitätssicherung, oder Produktion
  - Sie können unterschiedlichen Topologien haben.
    - Bspl: Besteht aus einem Server, über mehrere Server verteilt, oder sich über mehrere Servercluser erstecken
  - Intellij
  - PyCharm
  - GitHub
  - Ubuntu
  - Containers

- Rahmenbedingung (Frameworks)
  - Python (Django, Flask), ReactJS
  - auf dem Cloud
  - Technische vs wirtschaftliche RB `https://www.youtube.com/watch?v=JXhO1DNgxrc`
- Meine Anfordeungen - i.e. User Stories
  - Use-Case-Diagramm, Kriterien schreiben
  - Epics  


Second Task - 2 Wochen
---
# Entwurf / Konzeption
- Systemarchitektur
  - Komponenten
    - Wiederverwendbar
    - Austauschbar
    - Testbar
- Abgrenzung
- Festlegung der Technolgien
- MVC
  - Model: DB-Diagramm
  - View: Mock-ups (APIs) - Powerpoint - 
  - Controller: Businness-logik - Suchservice, usw..

Third Task - ~3-4 Wochen
---
# Implementierung
- Archetiktur
- Technolgien
- MVC
- solr - fuer die Suchfunktion
- 


------------------------------
# Einleitung
### Motivation
The presence of different languages makes it sometimes difficult to make a choice of which one to choose for your project. Also, when working on a monolithic application, it makes it harder for new developers to add new features to a running project without risking to effect the performance, or even cause the whole application to stop runnning completely, because of some new bugs or a new featuer which doesn't end-up communicating with the rest of the other features, the way it's supposed to. This is why it was very important to find a way to separate this issues in a way that it makes it more efficient for the developers whenever they want to add a new feature, without effecting the work of other developers and the integrity of the application. Microservices didn't only allow developers to build loose, independent services, but it also made it possibile for developers to develop these features in the language they see fit to that exact feature. This is why companies like amazon, facebook and many others started implementing this architecture in their business structure and this is why the Webportal is going to be developed using microservices.

A microservice is not a layer within a monolithic application (example, the web controller, or the backend-for-frontend).( "Backends For Frontends Pattern". Microsoft Azure Cloud Design Patterns. Microsoft.
 - https://docs.microsoft.com/en-us/azure/architecture/patterns/backends-for-frontends). Rather, it is a self-contained piece of busines functionaliy with clear interfaces, and may, through its own internal components, implement a layered architecture. From a strategy perspective, microservice architecture essentially follows the Unix philosophy of "Do one thing and do it well". ( Lucas Krause. Microservices: Patterns and Applications. ASIN B00VJ3NP4A.
- ).
integrate to the running project
### Zielsetzung
- Abgrenzung
The goal of this project is to create an application (portal) with the use of microservices. By the end, the portal should be scalable and the services highly independet from each other, but still can communicate with each other without any distrubtions. The services will be separated according to functionality and will be run on a container like Docker. For the backend, the main application service will be implemented with python using the flask framework, where the admin application service will be using the Django framework. For the frontend, ReactJS wil l be used, because it's currently one of the most popular JavaScript libraries for building Web applications and it's highly performant. It also can be used for handling the view layer for web and mobile apps, in case someone decides to make the portal applicable on mobile phones using React Native. According to, (quote). This means, there should be around 3 services by the end of the project and each implemented on it's own container. These services should be able to communicate with each other simulatniously and without any interruption and in-case one service goes down, others should stay running and the rest of the application functionality should be not influenced by it.
- Aufbau der Arbeit

# Grundlagen
- Python</br>
In the last few years, Python has exploded in popularity. The programming language has surpassed Java in popularity, but, for many, this is no surprise. With the rise in machine learning, data analysis, and web application development, many developers utilize Python for its powerful and abundant libraries, easy-to-learn syntax, and portability. (https://www.educative.io/blog/web-development-in-python).<br/>
**Advantages of using python to develop a web application**</br>
1. Easy to learn
2. Rich ecosystem and libraries.
3. Fast prototyping
4. Wide-spread popularity


  - Python-Frameworks
    - Django  (Definitionen, Erklärungen)<br/>
    Django is a Python web framework that offers an open-source, high-level framework that “encourages rapid development and clean, pragmatic design.” It’s fast, secure, and scalable. Django offers strong community support and detailed documentation.

      Django is incredibly flexible in which you can work with MVPs to larger companies. For some perspective, some of the largest companies that use Django are Instagram, Dropbox, Pinterest, and Spotify.

    -  Flask <br/>
      is considered a microframework, which is a minimalistic web framework. It’s less “batteries-included,” meaning that it lacks a lot of features and functionality that full-stack frameworks like Django offer, such as a web template engine, account authorization, and authentication.

        Flask is minimalistic and lightweight, meaning that you add extensions and libraries that you need as you code without automatically being provided with it by the framework.

        The philosophy behind Flask is that it gives only the components you need to build an app so that you have the flexibility and control.

        Flask is also a prevalent and powerful web framework as it’s used by large companies like Netflix, Linkedin, and Uber.
- ReactJS
- Microservice<br/>

It is hard to determine exactly who used the term microservice an dwhen. While it seems most likey that although the term first appeared on the scene around 2011, some companies adopted this style much earlier. 
  One example is Amazon, weich broke apart its previously monolithic Obidos appliation into many  small services. In a 2006 interview with Microsoft Fellow Jim Gray for ACM queue, (Wener Vogels, "A conversation with Werner Vogels: Learning from the Amazon technology platform," interview by Jim Gray. ACM Queue, Volume 4, Issue 4. June 30, 2006.) Amazon CTO Werner Vogels describes as a general "service orientation" what comes very close to our definition of microservices:
    "For us service orienation means encapsulating the data iwth the business logic that operates on the data, with the only access through a blished esrvice interface. No directe database access is allowed form outside the service, and there's no data sharing among the services."<br/>

    Former eBay and Google executive Randy Shoup summarizes (3) microesrvice characteristics as having three main features: 
      
      1. They've a very focused scope that concentrates on a very few functionalities (at times a single one), expressed by a small and also well-defined API.
      
      2. They're all very modular, and independently deployable, essentially elevating the rules of software encapsulation and modularity from the progra to the deployment unit level.
      
      3. Finally, microservices have isolated persistence, meaning that they do not share persistent storage, such as a common database.

- RabbitMQ
- Travis-CI
Travis CI is a hosted[2] continuous integration service used to build and test software projects hosted on GitHub[3] and Bitbucket.[4]

Travis CI was the first CI service which provided services to open-source projects for free and continues to do so. TravisPro provides custom deployments of a proprietary version on the customer's own hardware.

The source is technically free software and available piecemeal on GitHub under permissive licenses. The company notes, however, that the large number of tasks that a user needs to monitor and perform can make it difficult for some users to successfully integrate the Enterprise version with their own infrastructure.[5] (Wikipedia)


First Task - 2 Wochen
---
# Anforderungsanalyse
The first question we should be asking ourselves is how should the requirement analysis be done in the right order. Should we start with acquiring the user stories first or should we jump to writing the functional and non-functional requirements first? Which makes more sense and which one is the right way for a proper understanding for what we need for the application we tend to develop?
Let's start by understanding the difference between the two of them.  
### User stories

.....
The different tasks will then be splitted in forms of ToDO's, in Progress, and done. For this JIRA is going to be used to have a clear view of which features are still open, which needs to be worked on, and which are already done. Normally, such processes are done in teams and these tasks can be assigned accordingly to team-members. The User stories are stored in a product log and from them anyone can take a user story and start working on it. In companies, to keep an eye if everyone is doing the right requirement, to avoid any kind of missunderstanding and to check if no one needs anything or any assistance to finish their task. Spring planning meetings take place. The Spring planning meeting is subdivided into: During Spring, Daily Standup in a sprint, and daily scrum meetings. These won't be discussed as part of these thesis, hence the project is being developed by only one person and not in a corporate environemt (nicht in einer Unternehmensumgebung).
### Requirments
### Zielsetzung - 
### Anwendungsumgebung

The services are going to be build on an Ubuntu OS using Intellij as an IDE. Hence, the microservices architecture is going to be applied, the use of frameworks and implementation of features are going to be done systematically. This means, first a task is going to be put in place, where first the features using the Django Framework are going to be implemented and afterwards a new task is going to be added where new features are going to be built using the Flask Framework, which are supposed to be independent from the other features built in Django. All of these implementations are going to take place in Intellij. After this is done the communication between both the service is going to be made possible using an open-source message-broker software like RabbitMQ. The whole code is going to be pushed to github and monitored using an application like Travis-CI for a continuous Integeration and Deployment. This allows the discovery of any bugs in each feature as soon as it gets pushed to GitHub.

In short, our application environment is going to be consisted of the following: Ubuntu OS, Intellij, see drawing - Anwendungsumgebung.drawio.

### Rahmenbedingung
- Meine Anfordeungen - i.e. User Stories
  - Use-Case-Diagramm, Kriterien schreieben
  - Epics

Second Task - 2 Wochen
---
# Entwurf / Konzeption
- Systemarchetiktur
- Abgrenzung
- Festlegung der Technolgien
- MVC
  - Model: DB-Diagramm
  - View: Mock-ups (APIs) - Powerpoint - 
  - Controller: Businness-logik - Suchservice, usw..

Third Task - ~3-4 Wochen
---
# Implementierung
- Archetiktur
- Technolgien
- MVC
- 