# demo reverse proxy backend

## Setup

* Bitte Sicherstellen, dass folgende Komponenten auf dem System verfügbar sind:
  *  docker
  *  docker-compose
* Sollte auf dem eigenen System Fehler auftreten, kann auch auf eine Virtuelle Maschine in der Cloud zurück gegeriffen werden
* diese Repository clonen und in das entsprechende Verzeichnis wechseln

## Ausgangssituation

* Die `docker-compose.yml` Datei enthält drei Dienste: Proxy, Frontend und Backend
  * Der Proxy ist vorgeben und kann zum testen benutzt werden
* Sie haben ein backend-docker-image erstellt, in diesem Beispiel heißt es `christianheimke/demo-backend-nodejs:001`
  * das Backend ist auf Port 5000 verfügbar im Container
* Sie haben ein frontend-docker-image erstellt, in diesem Beispiel heißt es `christianheimke/demo-frontend-nodejs:001`
  * das Frontend ist auf Port 80 verfügbar im Container

## Aufgabenstellung

* Tauschen Sie das Frontend und Backend Image gegen Ihr Image aus
* Führen Sie `docker-compose up` aus
* Rufen Sie die URL http://localhost:8080/ auf und überprüfen Sie die Funktionsweise Ihrer Webapp

