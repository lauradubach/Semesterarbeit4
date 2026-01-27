# Teil 4 Abschluss

Der letzte Teil der Arbeit. Hier wird die ganze Auswertung des Projektes beschrieben. Eine Selbstreflexion und die ganzen Anhänge und Quellen sind hier dokumentiert.

- [Teil 4 Abschluss](#teil-4-abschluss)
- [Auswerten](#auswerten)
  - [Zusammenfassung](#zusammenfassung)
  - [Reflexion](#reflexion)
    - [Persönliche Reflexion](#persönliche-reflexion)
      - [Herausforderungen und Lösungen](#herausforderungen-und-lösungen)
    - [Reflexion der technischen Umsetzung](#reflexion-der-technischen-umsetzung)
      - [Analysen und Planung](#analysen-und-planung)
      - [Entscheidung](#entscheidung)
      - [Umsetzung des Projektes](#umsetzung-des-projektes)
  - [Fazit](#fazit)
    - [Effizienzsteigerung](#effizienzsteigerung)
    - [Lernerfahrungen](#lernerfahrungen)
  - [Mögliche Weiterentwicklung](#mögliche-weiterentwicklung)
    - [Erweiterte Funktionalität](#erweiterte-funktionalität)
    - [Skalierbarkeit und Performance](#skalierbarkeit-und-performance)
  - [Quellen](#quellen)

# Auswerten

Im Kapitel Auswerten wird der Abschluss des Projektes beschrieben. Es wird Zusammengefasst, Reflektiert und Analysiert. Auch alle Quellen die verwendet wurden, werden angehängt.

## Zusammenfassung

Im Rahmen dieses Projekts lag der Schwerpunkt auf dem Aufsetzen und der Konfiguration eines Kubernetes-Clusters für einen bereits bestehenden „Music Eventfinder“-Microservice. Ziel war es, eine stabile und reproduzierbare Laufzeitumgebung zu schaffen, in der Anpassungen automatisiert über eine CI/CD-Pipeline und Argo CD bereitgestellt werden können.  
Das Projekt diente dazu, grundlegende Kubernetes-Konzepte, GitOps-Ansätze sowie die Integration in einen DevOps-Prozess praxisnah umzusetzen.

## Reflexion

### Persönliche Reflexion

Das Projekt bot mir die Möglichkeit, mich intensiv mit Kubernetes als Orchestrierungsplattform auseinanderzusetzen. Da der Microservice bereits entwickelt war, konnte ich mich vollständig auf die Infrastruktur und deren Betrieb konzentrieren. Besonders herausfordernd und zugleich lehrreich war das Verständnis der verschiedenen Kubernetes-Komponenten und deren Zusammenspiel innerhalb eines Clusters.

#### Herausforderungen und Lösungen

Eine zentrale Herausforderung bestand im initialen Aufsetzen des Kubernetes-Clusters. Dabei traten unter anderem Probleme bei der ArgoCD konfiguration, der Secrets hinterlegung und dem Driver Hyper V auf. Diese Herausforderungen konnten durch gezielte Fehlersuche sowie durch das Studium von Logs und Statusinformationen gelöst werden. Hilfreich war zudem, das Cluster zunächst minimal aufzusetzen und anschließend schrittweise zu erweitern.

### Reflexion der technischen Umsetzung

#### Analysen und Planung

Zu Beginn wurde analysiert, welche Anforderungen der bestehende Microservice an die Kubernetes-Umgebung stellt. Dazu gehörten Aspekte wie benötigte Ressourcen, Netzwerkzugriff und Deployment-Struktur.  
Auf dieser Basis wurde entschieden, wie der Cluster aufgebaut sein soll und welche Komponenten für den Betrieb notwendig sind, beispielsweise Ingress, Service-Definitionen und Namespaces.

#### Entscheidung

Die Entscheidung, den Schwerpunkt auf den Kubernetes-Cluster zu legen, wurde bewusst getroffen, da ein korrekt konfigurierter Cluster die Grundlage für alle weiteren DevOps-Prozesse bildet. Zusätzlich fiel die Wahl auf Argo CD als Deployment-Tool, um den Cluster nach GitOps-Prinzipien zu betreiben und eine saubere Trennung zwischen Infrastruktur, Anwendung und Deployment-Prozess zu gewährleisten.

#### Umsetzung des Projektes

Die Umsetzung begann mit dem Aufbau des Kubernetes-Clusters und der Konfiguration der grundlegenden Cluster-Komponenten. Anschließend wurde der bestehende Microservice in den Cluster integriert und über definierte Services erreichbar gemacht.  
Ergänzend wurde eine CI/CD-Pipeline eingerichtet, die Änderungen automatisch verarbeitet und an Argo CD übergibt, welches die Synchronisation mit dem Cluster übernimmt.

## Fazit

### Effizienzsteigerung

Durch das strukturierte Aufsetzen des Kubernetes-Clusters konnte eine stabile und skalierbare Umgebung geschaffen werden. In Kombination mit Argo CD und der CI/CD-Pipeline lassen sich Anpassungen nun automatisiert und reproduzierbar ausrollen. Dies reduziert manuelle Eingriffe und erhöht die Betriebssicherheit deutlich.

### Lernerfahrungen

Das Projekt hat mein Verständnis für Kubernetes, Cluster-Architekturen und containerisierte Anwendungen wesentlich vertieft. Besonders wertvoll war die praktische Erfahrung im Aufbau und Betrieb eines Clusters sowie das Zusammenspiel mit GitOps- und CI/CD-Ansätzen. Ich habe gelernt, dass eine saubere Cluster-Konfiguration die Grundlage für erfolgreiche DevOps-Prozesse darstellt.

## Mögliche Weiterentwicklung

### Erweiterte Funktionalität

Eine mögliche Weiterentwicklung wäre die stärkere Automatisierung der Infrastruktur durch den Einsatz von Infrastructure as Code (IaC), beispielsweise mit Tools wie Terraform oder Ansible. Dadurch könnte das gesamte Kubernetes-Cluster reproduzierbar erstellt und versioniert werden, was insbesondere bei mehreren Umgebungen wie Development, Staging und Production von Vorteil wäre.

Zusätzlich könnte das GitOps-Konzept weiter ausgebaut werden, indem auch Konfigurationsänderungen auf Ingress-, Netzwerk- oder Sicherheits­ebene vollständig über das Git-Repository gesteuert werden.

### Skalierbarkeit und Performance

Im Bereich Skalierbarkeit und Performance könnten fortgeschrittene Deployment-Strategien wie Rolling Updates oder Canary Deployments implementiert werden. Diese würden es ermöglichen, neue Versionen des Microservices schrittweise auszurollen und Risiken bei Updates zu minimieren.

Darüber hinaus könnte eine stärkere Trennung der Workloads durch dedizierte Node Pools oder Taints und Tolerations umgesetzt werden, um Ressourcen gezielter zu nutzen und die Performance einzelner Anwendungen im Cluster weiter zu optimieren.

> (Chat GPT) [Quelle](https://chatgpt.com/share/696df157-04c4-8007-81c0-1f42a0b725c9)

## Quellen

Kapitel Konzeption
Chat GPT. (2025): SCRUM Erklärung. Aufgerufen am: 05.11.2025. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/6818f168-0354-800e-8c00-119b2ed7c509)

Kapitel Konzeption
Chat GPT. (2025): Warum SCRUM. Aufgerufen am: 05.11.2025. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/68230b9b-2d9c-800e-a1eb-64bd9fe8ed96)

Kapitel Konzeption
Chat GPT. (2025): Semesterarbeit DevOps Umsetzung. Aufgerufen am: 05.11.2025. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/6908ec06-4a2c-8007-834a-6013e399ba13)

Kapitel Konzeption
Chat GPT. (2025): Minikube vs Docker Kubernetes. Aufgerufen am: 05.11.2025. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/690b5e67-32b4-8007-999a-8bbbb27517c1)

Kapitel Konzeption
Chat GPT. (2025): Dokumentation schreiben. Aufgerufen am: 12.11.2025. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/69145d5b-1d28-8007-a9ab-019f02a428de)

Kapitel Konzeption
Chat GPT. (2025): Entscheidungsmatrix. Aufgerufen am: 18.11.2025. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/691c4131-e78c-8007-b99b-0448ad90d2e2)

Kapitel Konzeption
Chat GPT. (2025): Risikomatrix anpassen. Aufgerufen am: 28.11.2025. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/691c4eab-5f0c-8007-8817-4b7039fabc74)

Kapitel Konzeption
Chat GPT. (2025): Ist und Soll Zustand. Aufgerufen am: 18.11.2025. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/691c5c94-df1c-8007-92fd-93219b75bf52)

Kapitel Konzeption
Chat GPT. (2025): Implementierungsplan Projekt. Aufgerufen am: 18.11.2025. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/691c632c-1b80-8007-9f6a-b2ee70f95a04)

Kapitel Initialisieren
Chat GPT. (2026): Fibonacci in SCRUM implementieren. Aufgerufen am: 07.01.2026. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/695e11ee-aca0-8007-a795-4b48d14060d5)

Kapitel Abschluss
Chat GPT. (2026): Projekt Anfrage. Aufgerufen am: 19.01.2026. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/696df157-04c4-8007-81c0-1f42a0b725c9)

Kapitel Realisierung
Chat GPT. (2026): Textverbesserung Semesterarbeit. Aufgerufen am: 21.01.2026. Online unter:
> (Chat GPT) [Quelle](https://chatgpt.com/share/6970a9d5-3468-8007-8da6-0980bcc9719a)

> Back [Page](https://lauradubach.github.io/Semesterarbeit4/Sites/Teil%203%20Realisierung.html)
>
> Back [Start](https://lauradubach.github.io/Semesterarbeit4/)