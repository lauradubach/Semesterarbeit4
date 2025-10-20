# Teil 1 Initialisierung

In diesem Kapitel wird ins Thema der Arbeit eingeführt. Es beschreibt den Hintergrund und die Relevanz des Themas. Sie definiert das Ziel der Arbeit und formuliert die zentralen Fragen. Zudem gibt die Initialisierung einen kurzen Überblick über den Aufbau der Arbeit um eine klare Orientierung zu bieten.

- [Teil 1 Initialisierung](#teil-1-initialisierung)
- [Versionenverzeichnis](#versionenverzeichnis)
- [Aufgabenstellung](#aufgabenstellung)
  - [Ausgangslage](#ausgangslage)
  - [Ziele](#ziele)
  - [Mittel und Methode](#mittel-und-methode)
    - [Sachmittel](#sachmittel)
    - [Programmiersprache](#programmiersprache)
  - [Werkzeuge](#werkzeuge)
  - [SCRUM-Überblick](#scrum-überblick)
  - [Defenition of Done](#defenition-of-done)
    - [Funktionale Umsetzung](#funktionale-umsetzung)
    - [Technische Qualität](#technische-qualität)
    - [Sicherheit \& Stabilität](#sicherheit--stabilität)
    - [Deployment](#deployment)
    - [Dokumentation](#dokumentation)
    - [Review \& Akzeptanz](#review--akzeptanz)
- [Projektorganisation](#projektorganisation)
  - [Beteiligte Personen](#beteiligte-personen)
    - [Kanditatin](#kanditatin)
    - [Dozenten](#dozenten)
- [Datensicherung](#datensicherung)

# Versionenverzeichnis

| Version | Datum  | Autor | Bemerkung | 
| ------- | ------ | ----  | --------- |

# Aufgabenstellung

## Ausgangslage


## Ziele

## Mittel und Methode

### Sachmittel

### Programmiersprache

## Werkzeuge

## SCRUM-Überblick

Im Rahmen der Entwicklung des Microservices für personalisierte, ortsbezogene Event-Empfehlungen wird SCRUM als agiles Projektmanagement-Framework eingesetzt, um strukturierte Fortschritte zu ermöglichen. Das Projekt wird in mehrere Sprints unterteilt, in denen jeweils konkrete Teilziele wie zum Beispiel die Anbindung der externen Event-API, die Entwicklung der Filterlogik oder die Integration der REST-API fokussiert, bearbeitet werden. Zu Beginn jedes Sprints erfolgt eine Sprintplanung, in der die anstehenden Aufgaben priorisiert und aufgeteilt werden. Nach jedem Sprint wird ein Review durchgeführt. Durch den Einsatz von SCRUM bleibt man flexibel und kann trotz der technischen Komplexität effektiv auf Veränderungen und Herausforderungen reagieren.

## Defenition of Done

Ein Product Backlog Item, gilt als "Done", wenn **alle** folgenden Kriterien erfüllt sind:

### Funktionale Umsetzung

- Die Funktionalität ist vollständig implementiert gemäß der User Story und den Akzeptanzkriterien.
- Die API-Endpunkte liefern valide, erwartete Ergebnisse.
- Filterlogiken und Datenbankzugriffe funktionieren korrekt.

### Technische Qualität

- Der Code wurde dokumentiert.
- Es existieren Tests.
- Es gibt keine kritischen oder offenen Bugs.

### Sicherheit & Stabilität

- Datenvalidierung wurde umgesetzt.
- Es wurden Sicherheitsaspekte berücksichtigt.
- Die Anwendung läuft stabil in Docker-Containern.

### Deployment

- Die Anwendung ist containerisiert (Docker) und funktionsfähig bereitgestellt.
- Die Anwendung wird über die CI/CD-Pipeline automatisch auf AWS deployt.
- Der Deployment-Status ist dokumentiert oder im Log nachvollziehbar.

### Dokumentation

- Das Feature ist in der technischen Projektdokumentation beschrieben.
- Änderungen sind nachvollziehbar.
- Bei Bedarf wurden Screenshots, Diagramme oder Abläufe ergänzt.

### Review & Akzeptanz

- Die Sprint Reviews sind alle Dokumentiert
- Die Reflexion ist verständlich.
- Die Funktionalität ist im Product Backlog als „Done“ markiert.

# Projektorganisation

## Beteiligte Personen

### Kanditatin

```
Laura Joana Dubach
Funktion: Projektleiterin
P: 079 355 78 24
Github: lauradubach
Business E-Mail: laura.dubach@itnetx.ch
School E-Mail: laura.dubach@edu.tbz.ch
```
### Dozenten

```
Parisi Corrado
Funktion: PRJ-Dozent
Github: corrado-parisi
E-Mail: corrado.parisi@tbz.ch
```
```
Stark Philip
Funktion: Fachdozent
Github: 
E-Mail: philip.stark@tbz.ch
```

# Datensicherung

Damit keine Daten verloren gehen, werde ich alle Dokumente auf meinem OneDrive abspeichern. Durch das Pushen ins Github, wird dies ja auch in der Cloud gesichert. Zusätzlich werde ich die Daten auf einen USB-Stick abspeichern, damit ich im Worstcase Szenario ein Backup besitze.


> Back [Page](https://lauradubach.github.io/Semesterarbeit3/)
>
> Next [Page](https://lauradubach.github.io/Semesterarbeit3/Sites/Teil%202%20Konzeption.html)