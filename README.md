
### Presentation: [UI Testing - Selenium? Rich-Clients? Containers?](https://rawgit.com/toschneck/presentation/apex-connect-2018/index.html#/)


### Example: [Sakuli Selenium Examples](https://github.com/ConSol/sakuli-examples/tree/master/java-selenium-example)
### Example: [Sakuli Examples](https://github.com/consol/sakuli-examples)

Das Entwickeln und Gestalten von einer UI ist für sich allein genommen bereits eine große Herausforderung. Ganz zu schweigen von der Aufgabe die UI-Tests zu automatisieren. Wurde beides erfolgreich gemeistert, kommen allerdings die nächsten Fragen:

* Sollen wir auch die PDF-Auftragsbestätigung im Test validieren?
  > Natürlich sollten wir!

* Ist der Rich-Client auch zu testen?
  > Ja, wieso denn auch nicht!

* Wo sollen die Tests ausgeführt werden?
  > Natürlich im Docker-Container und im Kubernetes-Cluster!

* Können wir die Tests auf ein anderes Framework migrieren?
  > Was bringt uns das? Wir wollen die bestehenden Tests doch weiterverwenden!

Diese Fragen sind den Einen oder Anderen bestimmt nicht neu, aber was tun? Es wurde bereits viel Aufwand und Mühe in die Pflege der umfangreichen Selenium-Testsuiten gesteckt! Daher möchte man diese nur ungern verwerfen, nur um neue Anforderungen umzusetzen. Der Talk zeigt hierfür eine Lösung auf, die mit geringen Aufwand die bestehenden Selenium-Tests einfach erweitert. Die Open-Source-Erweiterung "Sakuli Se" bietet eine umfangreiche API, die es ermöglicht Rich-Clients, PDF-Inhalte oder auch Flash-Anwendungen ebenso leicht wie ein HTML-Button im selben Ausführungskontext zu testen. An Praxisbeispielen wird ebenso demonstriert wie durch vorgefertigte Dockerimages die Testausführung skalierbar bis in Cloud-Umgebung, wie Kubernetes oder OpenShift, aufgebaut werden kann.


For more information see __[ConSol/sakuli](https://github.com/ConSol/sakuli)__.
