# Teil 3 Realisieren

Kommen wir zur Umsetzung des Projektes. In diesem Teil wird genau beschrieben, wie alles realisiert wurde und wie ich vorgegangen bin. Es wird getestet und geprüft, sodass ersichtlich ist, ob alles funktioniert wie es soll. Falls Probleme aufgetaucht sind, werden diese ebenfalls beschrieben, inklusive Lösungsweg.

- [Teil 3 Realisieren](#teil-3-realisieren)
- [Realisieren](#realisieren)
  - [Architekturdiagramm](#architekturdiagramm)
  - [So funktionierts](#so-funktionierts)
    - [Überblick](#überblick)
    - [Komponenten im Detail](#komponenten-im-detail)
      - [Zusammenspiel der Komponenten](#zusammenspiel-der-komponenten)
  - [Datenbank](#datenbank)
  - [API](#api)
  - [Github Secrets](#github-secrets)
  - [Entwicklung](#entwicklung)
  - [Aufgetretene Probleme](#aufgetretene-probleme)
  - [Fallbacksolution](#fallbacksolution)
- [Kontrollieren](#kontrollieren)
  - [Testing](#testing)
    - [Testkonzept](#testkonzept)
    - [Testdurchführung](#testdurchführung)
      - [Umgebung:](#umgebung)

# Realisieren

Nun wird die Realisierung beschrieben. Die Umsetzung der Arbeit wird gezeigt inklusive Bilder der Produktiven Umgebung.

## Architekturdiagramm

```mermaid
graph TB
    subgraph Version["Versionsverwaltung"]
        A[GitHub<br/>App Repository<br/>Quellcode + CI/CD]
        A2[GitHub<br/>Config Repository<br/>Deployment YAMLs]
        CR[GitHub Container Registry<br/>Docker Images]
    end
    
    subgraph Virt["Virtualisierung"]
        E[Hyper-V<br/>Laufzeitumgebung für Minikube]
    end
    
    subgraph K8s["Kubernetes Cluster"]
        B[Argo CD<br/>GitOps Controller]
        H[Ingress<br/>Traffic-Routing]
        F[Musiceventfinder App<br/>Externe API-Anbindung]
    end
    
    G[Externe APIs<br/>Music Event Services]
    
    A -->|CI Pipeline baut| CR
    A -.->|Updated Image-Tags in| A2
    B -->|Pullt Manifeste aus| A2
    B -->|Pullt Images aus| CR
    B -->|Deployed| F
    H -->|Leitet Traffic zu| F
    F <-->|Kommuniziert mit| G
    E -.->|Host für| K8s
    
    classDef github fill:#e1f5ff,stroke:#0366d6,stroke-width:1px,color:#222222
    classDef registry fill:#e1ffe1,stroke:#28a745,stroke-width:1px,color:#222222
    classDef gitops fill:#fff4e1,stroke:#f9826c,stroke-width:1px,color:#222222
    classDef hyperv fill:#f5e1ff,stroke:#8b5cf6,stroke-width:1px,color:#222222
    classDef app fill:#ffebe1,stroke:#dc3545,stroke-width:1px,color:#222222
    classDef external fill:#f0f0f0,stroke:#6c757d,stroke-width:1px,color:#222222
    classDef ingress fill:#fffacd,stroke:#ffc107,stroke-width:1px,color:#222222
    
    class A,A2 github
    class CR registry
    class B gitops
    class E hyperv
    class F app
    class G external
    class H ingress
```

## So funktionierts

### Überblick

### Komponenten im Detail
 
#### Zusammenspiel der Komponenten

## Datenbank

## API

## Github Secrets

## Entwicklung

## Aufgetretene Probleme

## Fallbacksolution

Da das Projekt nicht für den Produktiven Gebrauch gedacht ist, weil es sich auf einem Learner LAB befindet, benötigt es keine Fallbacksolution. Falls etwas nicht klappt, kann das ganze einfach heruntergefahren werden und wieder auf der lokalen Umgebung bearbeitet werden.

# Kontrollieren

## Testing
### Testkonzept

| Testperson | Datum |
| ---------- | ----- |

| System | Testmittel | Testmethode |
| -------| ---------- | ----------- |

### Testdurchführung

| Testfall | Erwartetes Ergebnis | Testresultat |
| ---------| ------------------- | ------------ |


#### Umgebung:

> Back [Page](https://lauradubach.github.io/Semesterarbeit4/Sites/Teil%202%20Konzeption.html)
>
> Next [Page](https://lauradubach.github.io/Semesterarbeit4/Sites/Teil%204%20Abschluss.html)