# AGENTS.md – Die Hüttengemeinde

## Team

Dieses Repository wird von zwei Entwicklern gepflegt:

- **Jörg Bäuerle** (joerg.baeuerle@gmx.net)  
  GitHub: [@svdHero](https://github.com/svdHero)

- **Manuel Schick** (manu.schick85@googlemail.com)  
  GitHub: [@manu6006-ai](https://github.com/manu6006-ai)

## Git Workflow & Code Review

### Wichtige Regeln:

1. **Keine automatischen Git-Operationen**  
   Führe niemals automatisch folgende Operationen aus, ohne vorher zu fragen:
   - `git add` / Staging von Änderungen
   - `git commit`
   - `git merge` (lokales Zusammenführen von Branches)
   - Das Mergen eines Pull Requests auf GitHub (Klick auf "Merge Pull Request")

   `git push` und das Erstellen von Pull Requests sind hingegen automatisch erlaubt (ohne Nachfrage), solange dabei **nicht** direkt auf `main` gepusht wird.  
   **Direkt auf `main` pushen darf ausschließlich Jörg.**

2. **Code Review vor Merge auf `main`**  
   Bevor Manuel Änderungen auf den `main`-Branch mergen kann, **muss Jörg immer ein Code Review durchführen**.  
   Die bevorzugte Methode ist ein **GitHub Pull Request**, über den die Diskussion und der Review stattfinden kann. Das eigentliche Mergen erfolgt über den Merge-Button des Pull Requests (auf GitHub oder in der PR-Extension) – nicht per lokalem `git merge`.

### Empfohlener Workflow:

1. Feature Branch erstellen
2. Änderungen lokal vornehmen
3. Branch pushen
4. Pull Request auf GitHub erstellen
5. Jörg führt Code Review durch
6. Nach Genehmigung: Jörg mergt den Pull Request auf GitHub (Merge-Button)
7. Lokal zu `main` wechseln und pullen, um die gemergten Änderungen zu erhalten

---

## Code-Konventionen

- **Kein inline CSS**: Styles gehören immer in separate CSS-Dateien (z. B. `main.css`), nicht in `style`-Attribute oder `<style>`-Blöcke innerhalb von HTML-Dateien.
- **Kein JavaScript**: Die Seite bleibt reines, statisches HTML. Auf JavaScript wird bewusst verzichtet.

---

*Diese Instructions helfen Copilot, den richtigen Workflow für dieses Repository zu befolgen.*
