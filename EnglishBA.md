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