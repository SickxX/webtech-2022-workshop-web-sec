---
layout: workshop
titel: Web Security – Authentication Fehler und wie man sie verhindert
social-media-untertitel: Online-Workshop am 24. Mai 2022
datum: 2022-05-24
modul: wt
published: false
autor: Benedikt Engel
bild: ../hero.png
art: workshop
termin: Dienstag, 24. Mai 2022, 13:00 Uhr
dauer: 120-150 Minuten
raum: https://th-koeln.zoom.us/j/83055835045 (Zugangscode webtech) 
---

Die Authentication ist der Prozess der Echtheitsüberprüfung einer Entität gegenüber eines Systems. Dies geschiet in aller Regel über Login-Daten wie Nutzername und Passwort und eventuell weiteren faktoren. Die [OWASP-top-ten](https://owasp.org/www-project-top-ten/) Liste zeigt, das Authentication Fehler immer noch ein hohes Sicherheitsrisiko darstellen. Um dies mit ein paar Beispielen zu demonstrieren, werden wir uns mit dem `Juice-Shop` beschäftigen, welcher eine sehr unsichere Webanwendung darstellt. Außerdem wird ein bisschen OSINT (Open Source Intelligence, das Sammeln von öffentlich zugänglichen Informationen) einfließen, um zu zeigen, wie mittels bestimmter Informationen über ein Ziel in das System eingedrungen werden kann. Die `Burp-Suite` ist, wie Metasploit, ein Tool zum testen der Sicherheit, hier genauer die Sicherheit der Webanwendung. Wir werden `Burp-Suite` jedoch nur für einen bestimmten Fall verwenden. 


## Vorraussetzungen

Um am Workshop teilzunehmen, müsst ihr nur das Repo clonen und die Burp-Suite Community Edition herunterladen und installieren. Im Repo sind die Slides sowie die Aufgaben zu finden sowie der Juice-Shop als Submodule. Man kann den Juice-Shop auch einfach separat clonen. Als kleine Anleitung ist die Installation via `npm/NodeJS` gegeben. Andere Anleitungen, wie z.B. Docker, finden sich im Repo des [Juice-Shops](https://github.com/juice-shop/juice-shop#setup)

## Vorbereitungen

### Zu installieren
- [node.JS](https://nodejs.org/en/)
- [Burp suite Community Edition](https://portswigger.net/burp/releases/professional-community-2022-3-6?requestededition=community&requestedplatform=)

Das Repository des Workshops clonen mit:
```sh
git clone --recurse-submodules https://github.com/SickxX/webtech-2022-workshop-web-sec.git
```

### Setup juice-shop mit node.JS und npm
Anschließend in den juice-shop Ordner bewegen und `npm install` und zuletzt `npm start` abschicken.
Der Shop läuft jetzt unter [localhost](http://localhost:3000).

[Hier](https://github.com/juice-shop/juice-shop#setup) sind noch andere Wege der Installation zu finden.

## Material

### Dokus

- [juice-shop auf Github](https://github.com/juice-shop/juice-shop)
- [OWASP-top-ten Liste](https://owasp.org/www-project-top-ten/)
- [Andere vulnerable Apps](https://owasp.org/www-project-vulnerable-web-applications-directory/)

### Workshop-Material

- [Workshop-Repository](https://github.com/SickxX/webtech-2022-workshop-web-sec) wird am Tag des Workshops veröffentlicht.
