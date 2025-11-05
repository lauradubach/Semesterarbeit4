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
| 1.0 | 29.10.25 | Laura Dubach | Teil Initialisierung dokumentiert |
| 1.1 | 31.10.25 | Laura Dubach | Zeitplanung, SCRUM |
| 1.2 | 03.11.25 | Laura Dubach | Start Teil Konzeption dokumentieren |

# Aufgabenstellung

Im Rahmen der Semesterarbeit soll der bestehende Microservice „Music Eventfinder“ nach modernen DevOps-Prinzipien automatisiert und skalierbar in einer Kubernetes-Umgebung bereitgestellt werden.
Ziel ist es, einen vollständigen End-to-End DevOps-Prozess zu realisieren, der die Containerisierung, den Aufbau einer CI/CD-Pipeline sowie das Deployment in einem Kubernetes-Cluster umfasst.
Der Entwicklungsprozess wird nach dem agilen Vorgehensmodell Scrum durchgeführt.

## Ausgangslage

Mit der zunehmenden Verbreitung von Microservice-Architekturen und Cloud-nativen Anwendungen wächst der Bedarf an effizienten DevOps-Prozessen.
Unternehmen stehen vor der Herausforderung, Software schneller, zuverlässiger und skalierbarer bereitzustellen.
Hierbei sind Automatisierung, Continuous Integration / Continuous Deployment (CI/CD) und Container-Orchestrierung mit Kubernetes zentrale Erfolgsfaktoren.
Der „Music Eventfinder“-Microservice soll als praxisnahes Beispiel dienen, um diese Konzepte in einer realistischen Umgebung umzusetzen.

## Ziele

Folgende messbare Ziele werden verfolgt:

**DevOps-Prozess aufbauen:**
Entwicklung eines automatisierten End-to-End-Prozesses für den Microservice.
Messbar: Vollständig automatisierter Build-, Test- und Deploymentprozess.

**CI/CD-Pipeline implementieren:**
Aufbau einer Pipeline, die bei jedem Code-Commit automatisch den Microservice baut, testet und bereitstellt.
Messbar: Erfolgreicher Pipeline-Durchlauf mit Deployment auf Kubernetes.

**Kubernetes-Deployment realisieren:**
Bereitstellung des Microservices in einem Kubernetes-Cluster.
Messbar: Zugriff auf den Service über einen definierten Endpunkt im Cluster.

**Scrum-Methodik anwenden:**
Umsetzung nach agilen Prinzipien inklusive Product Backlog, Sprintplanung und Retrospektiven.
Messbar: Vollständige Scrum-Artefakte und dokumentierter Sprint-Verlauf.

## Mittel und Methode

Die Arbeit orientiert sich an der agilen Softwareentwicklung nach Scrum und setzt DevOps-Prinzipien wie Automatisierung, kontinuierliche Integration und schnelles Feedback konsequent um.

- Vorgehensweise (nach Scrum)
- Iteratives Arbeiten in Sprints 
- Regelmäßige Reviews und Retrospektiven
- Dokumentation aller Sprint-Ergebnisse und Artefakte
- Technischer Ansatz
- Aufbau einer Container-basierten Architektur
- Automatisierte Build-, Test- und Deployment-Prozesse (CI/CD)
- Bereitstellung und Skalierung in einer Kubernetes-Umgebung
- Nutzung von GitHub Actions bzw. GitLab CI/CD als Automatisierungsplattform

### Sachmittel

IT-Infrastruktur:

- Kubernetes-Cluster (Cloud oder lokal via Minikube)
- CI/CD-System (GitHub Actions oder GitLab CI)
- Entwicklungsrechner mit Docker und kubectl

Software & Tools:

- Git, Docker, Kubernetes
- CI/CD-Tools: GitHub Actions, GitLab CI
- Scrum-Tools: Jira

Entwicklungsumgebung: 

- Visual Studio Code

### Programmiersprache

Die Arbeit basiert auf dem bereits bestehenden Music Eventfinder-Microservice. Es wird Python, Java oder JavaScript (Node.js) verwendet. Der Fokus der Arbeit liegt jedoch nicht auf der Programmiersprache selbst, sondern auf der DevOps-Integration und Automatisierung.

## Werkzeuge

| Kategorie            | Werkzeuge / Technologien                             |
| -------------------- | ---------------------------------------------------- |
| Versionsverwaltung   | Git                                                  |
| Containerisierung    | Docker                                               |
| Orchestrierung       | Kubernetes                                           |
| CI/CD                | GitHub Actions / GitLab CI                           |
| Agile Planung        | Jira (SCRUM)                                         |
| Entwicklung          | Visual Studio Code                                   |
| Testing              | Kubernetes Dashboard, kubectl, Unit-Tests            |

## SCRUM-Überblick

Im Rahmen der Umsetzung des Microservices wird das agile Vorgehensmodell Scrum als Projektmanagement-Framework eingesetzt, um den Entwicklungsprozess strukturiert und iterativ zu gestalten. Das Projekt wird in mehrere Sprints unterteilt, in denen jeweils spezifische Teilziele verfolgt werden.

Zu Beginn jedes Sprints erfolgt eine Sprint-Planung, in der die anstehenden Aufgaben priorisiert und im Product Backlog dokumentiert werden. Nach Abschluss jedes Sprints wird ein Sprint Review sowie eine Retrospektive durchgeführt, um Fortschritte zu evaluieren und den weiteren Projektverlauf anzupassen.

Durch den Einsatz von Scrum bleibt das Projekt flexibel und kann trotz der technischen Komplexität des DevOps-Ansatzes effektiv auf Veränderungen, technische Herausforderungen und neue Erkenntnisse reagieren. Dieses iterative Vorgehen fördert eine kontinuierliche Verbesserung und unterstützt die erfolgreiche Umsetzung eines automatisierten, skalierbaren Bereitstellungsprozesses für den Microservice.

## Defenition of Done

Ein Product Backlog Item, gilt als "Done", wenn **alle** folgenden Kriterien erfüllt sind:

### Funktionale Umsetzung

- Die Funktionalität ist vollständig implementiert gemäß der User Story und den Akzeptanzkriterien.
- Microservice-Endpunkte liefern valide, erwartete Ergebnisse.
- Automatisierte Tests zur Überprüfung der Business-Logik und Filterfunktionen sind vorhanden und erfolgreich.

### Technische Qualität

- Der Code wurde dokumentiert.
- Es existieren Tests.
- Es gibt keine kritischen oder offenen Bugs.

### Sicherheit & Stabilität

- Eingaben werden validiert, und Sicherheitsaspekte sind berücksichtigt.
- Der Microservice läuft stabil in Docker-Containern und kann skaliert werden.

### Deployment

- Die Anwendung ist containerisiert und erfolgreich in einem Kubernetes-Cluster bereitgestellt.
- CI/CD-Pipeline baut, testet und deployt den Microservice automatisch.
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
Github: pstark-code
E-Mail: philip.stark@tbz.ch
```

# Datensicherung

Damit keine Daten verloren gehen, werde ich alle Dokumente auf meinem OneDrive abspeichern. Durch das Pushen ins Github, wird dies ja auch in der Cloud gesichert. Zusätzlich werde ich die Daten auf einen USB-Stick abspeichern, damit ich im Worstcase Szenario ein Backup besitze.


> Back [Page](https://lauradubach.github.io/Semesterarbeit4/)
>
> Next [Page](https://lauradubach.github.io/Semesterarbeit4/Sites/Teil%202%20Konzeption.html)