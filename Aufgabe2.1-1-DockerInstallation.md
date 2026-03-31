## 1. Praxisteil: System-Abfrage

Um Informationen über die lokale Docker-Umgebung zu erhalten, gibt es drei gängige Wege:

### A. Über die Kommandozeile (CLI)

Dies ist der direkteste Weg für Administratoren:

* **Version prüfen:** `docker -v` (oder `docker version`)
  
  ```bash
  Docker version 20.10.23, build 7155243
  ```

* **Laufende Container anzeigen:** `docker ps`
  
  ```bash
  CONTAINER ID   IMAGE                           COMMAND        CREATED       STATUS          PORTS                                                           NAMES
  2cd9b983b1db   portainer/portainer-ce:latest   "/portainer"   3 years ago   Up 13 minutes   8000/tcp, 9000/tcp, 0.0.0.0:9443->9443/tcp, :::9443->9443/tcp   portainer
  ```

* **Vorhandene Images anzeigen:** `docker images ls`
  
  ```bash
  REPOSITORY               TAG       IMAGE ID       CREATED       SIZE
  portainer/portainer-ce   latest    5f11582196a4   3 years ago   287MB
  ```

### B. Über Visual Studio Code (Extension)

In der installierten **Docker Extension** findet man die Informationen grafisch aufbereitet in der Seitenleiste:

* Unter dem Reiter **Containers** werden alle aktiven Instanzen (z. B. Portainer) gelistet.
* Unter dem Reiter **Images** sieht man die lokal gespeicherten Abbilder (z. B. `portainer/portainer-ce`).

![Docker Extension Übersicht](img/Bild%20(5).png)

### C. Über Portainer (Web-Interface)

Portainer bietet ein Dashboard unter `https://localhost:9443`:

* **Dashboard:** Zeigt eine Übersicht des gesamten Systems.
* **Containers Menü:** Listet Details zu Status und Ressourcenverbrauch der Container.
* **Images Menü:** Ermöglicht das Verwalten und Durchsuchen der lokalen Image-Datenbank.

![Portainer Dashboard](img/Bild%20(6).png)
