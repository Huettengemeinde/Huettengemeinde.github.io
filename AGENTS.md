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
   - `git merge`

2. **Code Review vor Merge auf `main`**  
   Bevor Manuel Änderungen auf den `main`-Branch mergen kann, **muss Jörg immer ein Code Review durchführen**.  
   Die bevorzugte Methode ist ein **GitHub Pull Request**, über den die Diskussion und der Review stattfinden kann.

### Empfohlener Workflow:

1. Feature Branch erstellen
2. Änderungen lokal vornehmen
3. Branch pushen
4. Pull Request auf GitHub erstellen
5. Jörg führt Code Review durch
6. Nach Genehmigung: Merge auf `main`

---

## Code-Konventionen

- **Kein inline CSS**: Styles gehören immer in separate CSS-Dateien (z. B. `main.css`), nicht in `style`-Attribute oder `<style>`-Blöcke innerhalb von HTML-Dateien.
- **Kein JavaScript**: Die Seite bleibt reines, statisches HTML. Auf JavaScript wird bewusst verzichtet.

---

*Diese Instructions helfen Copilot, den richtigen Workflow für dieses Repository zu befolgen.*
