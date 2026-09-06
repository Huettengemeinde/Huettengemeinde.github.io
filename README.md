# Huettengemeinde.github.io

Dieses Repository enthält die Webseite für die Hüttengemeinde im Murgtal, erreichbar unter [huettengemeinde.de](https://huettengemeinde.de).

## Erste Schritte (Windows)

Diese Anleitung richtet sich an neue Mitwirkende unter Windows und führt von der Installation bis zum ersten Pull Request.

### 1. Voraussetzungen installieren

- **Git for Windows**: [git-scm.com](https://git-scm.com/download/win) herunterladen und mit den Standardoptionen installieren. Wird von VS Code für alle Git-Funktionen benötigt.
- **Visual Studio Code**: [code.visualstudio.com](https://code.visualstudio.com/) herunterladen. Beim Installer den **"System Installer"** wählen (nicht "User Installer"), damit VS Code für alle Benutzer des PCs verfügbar ist. Haken bei "Zu PATH hinzufügen" setzen.

### 2. VS Code Extensions installieren

In VS Code über die Extensions-Ansicht (`Strg+Shift+X`) installieren:

- **GitHub Pull Requests** (`GitHub.vscode-pull-request-github`) – zum Erstellen und Verwalten von Pull Requests direkt in VS Code, ohne zusätzliche Software wie GitHub Desktop.
- **Git Graph** (`mhutchie.git-graph`) – visualisiert die Commit-Historie und Branches.
- **Material Icon Theme** (`PKief.material-icon-theme`) – übersichtliche Datei-Icons im Explorer.
- **GitHub Copilot** (`GitHub.copilot`) und **GitHub Copilot Chat** (`GitHub.copilot-chat`) – KI-Unterstützung beim Programmieren, falls noch nicht vorhanden.

### 3. Bei GitHub anmelden & Copilot Pro abonnieren

- In VS Code unten links auf das Account-Icon klicken und mit dem eigenen GitHub-Account anmelden.
- Für die Nutzung von Copilot Chat wird ein **GitHub Copilot Pro** Abo (ca. 10 USD/Monat) benötigt, abschließbar unter [github.com/settings/copilot](https://github.com/settings/copilot).

### 4. Repository klonen

1. Befehlspalette öffnen (`Strg+Shift+P`) → **"Git: Clone"** eingeben und auswählen.
2. Die URL dieses Repositorys einfügen.
3. Zielordner auf der Festplatte wählen.
4. Im Dialog auf **"Open"** klicken, um das geklonte Repository zu öffnen.

### 5. Feature Branch erstellen, arbeiten, Pull Request stellen

1. Unten links in der Statusleiste auf den Branch-Namen klicken → **"Create new branch..."** → z. B. `feature/my-new-thing` eingeben.
2. Änderungen an den Dateien vornehmen (z. B. mit Unterstützung von Copilot Chat).
3. Im **Source Control** Panel (Symbol in der Activity Bar) die geänderten Dateien stagen (`+`) und eine Commit-Nachricht eingeben, dann **"Commit"** klicken.
4. Über **"Publish Branch"** bzw. **"Sync Changes"** den Branch zu GitHub pushen.
5. Über das **GitHub Pull Requests** Icon in der Activity Bar auf **"Create Pull Request"** klicken, Titel und Beschreibung eingeben und den PR erstellen.
6. Jörg führt das Code Review durch und klickt nach Genehmigung auf GitHub (oder in der PR-Extension) auf **"Merge Pull Request"**. Das ist ein serverseitiger Merge auf GitHub – kein lokaler `git merge`-Befehl.
7. Lokal zu `main` wechseln (Branch-Auswahl unten links) und über **"Sync Changes"**/Pull die gemergten Änderungen herunterladen. Der alte Feature Branch kann danach gelöscht werden.

> **Hinweis:** Arbeitet ihr mit GitHub Copilot im Agent-Modus, kann Copilot dank der GitHub Pull Requests Extension Branch, Push und Pull-Request-Erstellung auch selbstständig übernehmen. Staging, Commit und das eigentliche Mergen des PRs erfolgen dabei weiterhin nur nach Rückfrage, und direkt auf `main` pushen darf ausschließlich Jörg – siehe [AGENTS.md](AGENTS.md) für die vollständigen Regeln.
