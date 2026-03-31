# Docker & Containerisierung: Die Grundlagen

## 1. Was ist Containerisierung?
Containerisierung ist eine Technologie, um Anwendungen inklusive ihrer Abhängigkeiten isoliert zu verpacken. Ein Container ist eine leichtgewichtige, portierbare und unabhängige Umgebung. Im Gegensatz zu virtuellen Maschinen (VMs) teilt ein Container denselben Kernel mit dem Host-Betriebssystem.

### Eigenschaften von Containern
*   **Leichtgewichtig:** Da kein eigenes Betriebssystem gestartet werden muss, werden minimale Systemressourcen benötigt. Dies führt besonders in der Cloud zu Kostensenkungen.
*   **Portabel:** Ein Container läuft auf jedem System, das die entsprechende Container-Engine unterstützt, da er alle Abhängigkeiten selbst mitbringt.
*   **Isoliert:** Jeder Container läuft getrennt von anderen und vom Host-System, was die Sicherheit erhöht und gegenseitige Beeinflussung verhindert.

> **Kontext:** Container sind essenziell für Microservices, Cloud-Native-Anwendungen und moderne DevOps-Pipelines (CI/CD), um Konsistenz zwischen Entwicklung und Produktion zu garantieren.

---

## 2. Container vs. Virtualisierung (VMs)
Der Hauptunterschied liegt in der Art der Ressourcennutzung und der Architektur.



### Architektur-Vergleich
*   **Virtuelle Maschinen (VMs):** Simulieren ein komplettes physisches System inklusive eigener Hardware-Ressourcen und einem vollständigen **Gast-Betriebssystem**. Die Verwaltung erfolgt über einen **Hypervisor**.
*   **Container:** Nutzen direkt den **Kernel des Host-Betriebssystems**. Sie enthalten lediglich die Anwendung und deren Abhängigkeiten.

### Vorteile von Containern gegenüber VMs
1.  **Schnellere Startzeit:** Start in Sekundenbruchteilen statt Minuten.
2.  **Geringerer Ressourcenverbrauch:** Weniger RAM- und CPU-Last durch Shared-Kernel-Nutzung.
3.  **Einfachere Verwaltung:** Images sind deutlich kleiner und lassen sich schneller verteilen.
4.  **Höhere Dichte:** Auf einem einzelnen Host können wesentlich mehr Container als VMs gleichzeitig betrieben werden.

---

## 3. Die Docker-Architektur im Detail
Die praktische Umsetzung der Containerisierung mit Docker basiert auf vier zentralen Komponenten:

| Begriff | Kurzbeschreibung | Analogie |
| :--- | :--- | :--- |
| **Dockerfile** | Textdatei mit der Bauanleitung und allen Installationsschritten. | Das Rezept |
| **Docker Image** | Die fertige, unveränderliche Vorlage (Snapshot), die aus dem Dockerfile gebaut wurde. | Die Backmischung |
| **Docker Container** | Die aktive, isolierte Laufzeitinstanz, die aus einem Image gestartet wird. | Der fertige Kuchen |
| **Docker Registry** | Das digitale Lagerhaus (z. B. Docker Hub) zum Speichern und Teilen von Images. | Der Supermarkt |

---
*Dokumentationsstand: März 2026 | Bearbeitungszeit: 25 Minuten*
