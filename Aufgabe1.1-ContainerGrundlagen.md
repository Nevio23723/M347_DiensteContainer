# Docker Grundlagen & Konzepte

## 1. Welche Problematik löst Docker?
Docker bietet eine **isolierte Umgebung**, in der Software mitsamt allen benötigten Komponenten verpackt wird. Dies vereinfacht die globale Nutzung und das Deployment von Anwendungen massiv.

*   **Dependency Management:** Da moderne Software viele Abhängigkeiten (Dependencies) benötigt, können diese direkt im Docker Container vorinstalliert werden, um Konflikte zu vermeiden.
*   **Effizienz:** Docker verbraucht deutlich weniger Ressourcen als herkömmliche virtuelle Maschinen, da sich die Container das Betriebssystem teilen.

## 2. Unterschied: VM vs. Container
Der Hauptunterschied liegt in der Art der Ressourcenverteilung und der Architektur:

*   **Virtuelle Maschinen (VMs):** Nutzen eine **Hypervisor-Schicht**, um Hardware-Ressourcen zu verteilen. Jede VM benötigt ein eigenes, vollständiges Gast-Betriebssystem.
*   **Container:** Teilen sich den Kernel des Host-Betriebssystems. Sie besitzen **kein eigenes Host-OS**, wodurch sie extrem leichtgewichtig sind und Ressourcen einsparen.



## 3. Die vier Kernbegriffe
Die Arbeit mit Docker lässt sich in vier zentrale Komponenten unterteilen:

| Begriff | Kurzbeschreibung | Analogie |
| :--- | :--- | :--- |
| **Dockerfile** | Textdatei mit der Bauanleitung und allen Installationsschritten. | Das Rezept |
| **Docker Image** | Die fertige, unveränderliche Vorlage, die aus dem Dockerfile gebaut wurde. | Die Backmischung |
| **Docker Container** | Die aktive, isolierte Laufzeitinstanz, die aus einem Image gestartet wird. | Der fertige Kuchen |
| **Docker Registry** | Das digitale Lagerhaus zum Speichern und Teilen von Images. | Die Bibliothek |

---
