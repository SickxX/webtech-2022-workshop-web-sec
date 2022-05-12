# Workshop für das Modul Web Technologien
Authentification Fehler und wie man sie verhindert

## Directory
In diesem Repository befinden sich die Präsentation als keynote und als pdf im Ordner [slides](./slides/), die Aufgabentexte im Ordner [challenges](./challenges/), und die hackbare Umgebung als Submodule im Ordner [juice-shop](./juice-shop/). 

## Requisiten
- [node.JS](https://nodejs.org/en/)
- [Burp suite Community Edition](https://portswigger.net/burp/releases/professional-community-2022-3-6?requestededition=community&requestedplatform=)
## Setup Repo mit Submodules
Repo klonen mit 
```sh
git clone https://github.com/SickxX/webtech-2022-workshop-web-sec.git
```
in das Repo bewegen mit `cd webtech-2022-workshop-web-sec ` und dann `git submodule init` und `git submodule update`

ODER gleich alles auf einmal clonen mit:
```sh
git clone --recurse-submodules https://github.com/SickxX/webtech-2022-workshop-web-sec.git
```
## Setup juice-shop mit node.JS und npm
Anschließend in den juice-shop Ordner bewegen und `npm install` und zuletzt `npm start` abschicken.
Der Shop läuft jetzt unter [localhost](http://localhost:3000).

[Hier](https://github.com/juice-shop/juice-shop#setup) sind noch andere Wege der Installation zu finden.
