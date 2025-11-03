# Teil 2 Konzeption

Nun gehen wir ins Thema Konzeption über. In diesem Kapitel wird das ganze Projekt vorbereitet. Die Ausgangslage und Anforderungen werden beschrieben, auch was das Ziel des Projektes ist, wird aufgezeigt. Die Planung wird gemacht und es werden Entscheidungen getroffen um das Projekt mit den Optimalen Tools umzusetzten.

- [Teil 2 Konzeption](#teil-2-konzeption)
- [Informieren](#informieren)
  - [Was ist SCRUM?](#was-ist-scrum)
    - [Die wichtigsten Merkmale](#die-wichtigsten-merkmale)
    - [Die zentralen Rollen](#die-zentralen-rollen)
    - [Die wichtigsten Ereignisse (Events)](#die-wichtigsten-ereignisse-events)
    - [Zentrale Artefakte](#zentrale-artefakte)
    - [Wieso SCRUM](#wieso-scrum)
  - [Ausgangslage \& Motivation](#ausgangslage--motivation)
  - [Anforderungen erheben](#anforderungen-erheben)
    - [Funktionale Anforderungen](#funktionale-anforderungen)
    - [Nicht-funktionale Anforderungen](#nicht-funktionale-anforderungen)
  - [Relevanz und Nutzen eines Event-Finders](#relevanz-und-nutzen-eines-event-finders)
    - [Die Arbeit zeigt konkret, wie ein realer Microservice:](#die-arbeit-zeigt-konkret-wie-ein-realer-microservice)
    - [Dies bringt Vorteile für:](#dies-bringt-vorteile-für)
  - [Seusag](#seusag)
- [Planen](#planen)
  - [Zeitplan](#zeitplan)
  - [Meilensteine](#meilensteine)
    - [1. Initialisierung](#1-initialisierung)
    - [2. Konzeption](#2-konzeption)
    - [3. Realisieren](#3-realisieren)
    - [4. Abschluss](#4-abschluss)
  - [Ist und Soll](#ist-und-soll)
    - [Ist Zustand](#ist-zustand)
    - [Soll Zustand](#soll-zustand)
  - [Risikomatrix](#risikomatrix)
  - [Implementierungsplan](#implementierungsplan)
- [Entscheiden](#entscheiden)
  - [SWOT-Analyse](#swot-analyse)
  - [Technologieentscheidungen](#technologieentscheidungen)
      - [Entscheidungsmatrix](#entscheidungsmatrix)


# Informieren

In diesem Kapitel werde ich alle Informationen zusammentragen, um das Projekt umsetzen zu können.

## Was ist SCRUM?

SCRUM ist ein agiles Rahmenwerk (Framework) für Projektmanagement, das vor allem in der Softwareentwicklung eingesetzt wird. Es hilft Teams, komplexe Projekte schrittweise zu bearbeiten und regelmäßig Ergebnisse zu liefern.

![SCRUM_Prozess](../Pictures/SCRUM_Prozess.png)

### Die wichtigsten Merkmale

- Die Arbeit wird in festen Zeitabschnitten, sogenannten Sprints (meist 2–4 Wochen), erledigt.
- Transparenz, Überprüfung und Anpassung: Nach jedem Sprint wird das Ergebnis vorgestellt und gegebenenfalls der Plan angepasst.

### Die zentralen Rollen

- Product Owner – Verantwortlich für das Produkt und dessen Anforderungen (Pflege des Product Backlogs).
- Scrum Master – Unterstützt das Team, entfernt Hindernisse und sorgt für die Einhaltung von SCRUM.
- Entwicklungsteam – Umsetzt die Anforderungen und liefert am Ende eines Sprints ein fertiges Produktinkrement.

### Die wichtigsten Ereignisse (Events)

- Sprint Planning – Planung, was im kommenden Sprint erreicht werden soll.
- Daily Scrum – Tägliches 15-Minuten-Meeting zur Abstimmung.
- Sprint Review – Vorstellung der Ergebnisse am Sprintende.
- Sprint Retrospective – Rückblick auf den Sprint zur Prozessverbesserung.

### Zentrale Artefakte

- Product Backlog – Liste aller Anforderungen an das Produkt.
- Sprint Backlog – Auswahl der Aufgaben für den aktuellen Sprint.
- Increment – Das am Ende eines Sprints fertige und getestete Produktstück.

> (Chat GPT) [Quelle](https://chatgpt.com/share/6818f168-0354-800e-8c00-119b2ed7c509)

### Wieso SCRUM

Ich habe mich bewusst für SCRUM als Vorgehensmodell entschieden, weil es ein etabliertes, agiles Framework ist. SCRUM ermöglicht es, in kurzen Zyklen (Sprints) kontinuierlich, funktionsfähige Ergebnisse zu liefern, die regelmäßig überprüft und angepasst werden können.

Durch die klare Struktur, regelmäßigen Events (Sprint Planning, Sprint Review, Retrospektive) und einem fokussierten Backlog-Management entsteht ein hohes Maß an Transparenz, Planbarkeit und Flexibilität.

Ein weiterer, entscheidender Vorteil von SCRUM ist, die enge Einbindung von Feedback. So kann frühzeitig auf Veränderungen oder neue Erkenntnisse reagiert werden, ohne die gesamte Projektplanung überarbeiten zu müssen. Dies fördert eine nutzerzentrierte Entwicklung und reduziert das Risiko, am Bedarf vorbei zu arbeiten.

Zusätzlich haben wir im Unterricht SCRUM in der Theorie angeschaut und nun kann ich es im Praktischen lernen umzusetzten. Natürlich wird einiges am Standard Prozess angepasst, da ich das Projekt alleine durchführe. Hier ist zum Beispiel ein Daily SCRUM nicht notwendig.

> (Chat GPT) [Quelle](https://chatgpt.com/share/68230b9b-2d9c-800e-a1eb-64bd9fe8ed96)


## Ausgangslage & Motivation

Mit der zunehmenden Verbreitung von Cloud-Technologien, Microservice-Architekturen und DevOps-Methoden wächst der Bedarf an skalierbaren, automatisierten und flexibel wartbaren Systemen.
Unternehmen stehen vor der Herausforderung, Software schnell, zuverlässig und reproduzierbar bereitzustellen — insbesondere in dynamischen Umgebungen wie Kubernetes-Clustern.

Der Music Eventfinder-Microservice dient in dieser Arbeit als praxisnahes Beispiel, um den vollständigen Lebenszyklus eines Cloud-basierten Microservice-Systems zu realisieren.
Im Fokus steht nicht die fachliche Weiterentwicklung der Anwendung, sondern der Aufbau einer modernen, automatisierten Bereitstellungs- und Betriebsumgebung auf Basis von:

- Containerisierung
- Continuous Integration und Continuous Deployment (CI/CD)
- Kubernetes-Orchestrierung
- Agiler Projektsteuerung nach Scrum

Die persönliche Motivation liegt im Interesse an Cloud-nativem Deployment, moderner Softwarebereitstellung und dem praxisnahen Einsatz von DevOps-Werkzeugen und Kubernetes-Infrastruktur.

## Anforderungen erheben

Für die erfolgreiche Umsetzung des Projektes werden sowohl funktionale als auch technische/non-funktionale Anforderungen definiert.

### Funktionale Anforderungen

- Bereitstellung des bestehenden Music Eventfinder-Microservices in Containern
- Externe Event-API-Anbindung bleibt funktional
- Bereitstellung einer REST-API für Eventdaten
- Zugriff auf Nutzer-/Einstellungsdaten über Datenbank

### Nicht-funktionale Anforderungen

- Automatisierter Build-, Test- und Deployment-Prozess (CI/CD)
- Containerisierung mit Docker zur Portabilität
- Deployment in einem Kubernetes-Cluster
- Möglichkeit zur Skalierung (Pods/ReplicaSets/Autoscaling)
- Verwaltung von Konfiguration und Secrets (ConfigMaps & Secrets)
- Nachvollziehbare Versionierung & Dokumentation
- Sichere Verarbeitung von Benutzerdaten gemäß modernen Standards

## Relevanz und Nutzen eines Event-Finders

### Die Arbeit zeigt konkret, wie ein realer Microservice:

- automatisiert entwickelt, gebaut, getestet und deployt wird
- in einer Kubernetes-Umgebung betrieben und skaliert werden kann

### Dies bringt Vorteile für:

**Entwickler/innen & Studierende**

- Hands-on-Erfahrung mit Kubernetes & DevOps-Pipelines
- Praxiswissen zu Container-Workflows & Cloud-Infrastruktur

**Unternehmen / Plattformbetreiber**

- Vorlage für automatisierte Softwarebereitstellung
- Erweiterbare Microservice-Struktur
- Basis für skalierbare, cloud-native Anwendungen

**Endnutzer/innen**

- Zugriff auf personalisierte Musik-Eventdaten über einen stabilen, skalierbaren Service

Durch den Einsatz moderner Kubernetes und DevOps-Technologien entsteht eine zukunftsfähige, skalierbare und wartungsfreundliche Lösung, die reale Anforderungen an moderne Softwarebereitstellung abbildet.

> (Chat GPT) [Quelle](https://chatgpt.com/share/6908ec06-4a2c-8007-834a-6013e399ba13)

## Seusag

# Planen

Hier werde ich das ganze Projekt planen. Es wird ein Zeitplan erstellt, wann welche Tätigkeiten fällig sind und die Meilensteine sind genau beschrieben.

## Zeitplan

![Zeitplan](../Pictures/Zeitplan.png)

## Meilensteine
### 1. Initialisierung

In der Initialisierungsphase wird das Projekt offiziell gestartet. Ziel ist es, eine klare Projektgrundlage zu schaffen. Dazu gehören die Definition von Zielen, die Identifikation von Stakeholdern, die grobe Planung sowie die Erstellung eines Projektauftrags. Risiken und Chancen werden frühzeitig analysiert und es wird geprüft, ob das Projekt wirtschaftlich und realistisch durchführbar ist.

### 2. Konzeption

In dieser Phase wird das Projekt inhaltlich konkretisiert. Anforderungen werden detailliert erhoben und dokumentiert (z. B. als User Stories), Lösungsansätze erarbeitet und bewertet. Es entsteht ein Fach- und ggf. ein technisches Konzept, das die Grundlage für die spätere Umsetzung bildet.

### 3. Realisieren

Jetzt beginnt die eigentliche Umsetzung: Entwicklung, Konfiguration, Tests und Integration der Komponenten. Die Arbeit erfolgt meist iterativ (z. B. in Sprints), um regelmäßig funktionierende Zwischenstände zu liefern.

### 4. Abschluss

Das Projekt wird formal beendet. Es finden eine Abnahme, eine Übergabe an den Betrieb sowie ggf. eine Schulung der Nutzer statt. Ausserdem werden Lessons Learned dokumentiert, um aus dem Projekt für zukünftige Vorhaben zu lernen.

## Ist und Soll

### Ist Zustand

### Soll Zustand

## Risikomatrix

## Implementierungsplan

Hier wird grob dargestellt, wie in diesem Projekt vorgegangen wird.

# Entscheiden

Im Kapitel Entscheiden werden die Produkte die zur Auswahl stehen verglichen. Es gibt eine SWOT Analyse und eine Entscheidunsmatrix. Zusätzlich wird beschrieben, wieso ich mit den Ausgewählten Programmen und Tools arbeite.

## SWOT-Analyse

Die folgende SWOT-Analyse fasst die wesentlichen Einflussfaktoren zusammen:

## Technologieentscheidungen

#### Entscheidungsmatrix

> Back [Page](https://lauradubach.github.io/Semesterarbeit3/Sites/Teil%201%20Initialisierung.html)
>
> Next [Page](https://lauradubach.github.io/Semesterarbeit3/Sites/Teil%203%20Realisierung.html)