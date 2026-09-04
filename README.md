# Gebäudedaten München Hbf (Übungs-Repository)

<!-- practice-repo-template: 4dcitygml Demo-Repo sample-munich-station README.
LOD2-CityGML rund um den Münchner Hauptbahnhof als bei Bedarf manuell zurückgesetzte
Übungsumgebung. Kein Produktivbetrieb einer Kommune, sondern Lernumgebung für
Werkzeuge, PR-Ablauf und kollaborative Datenpflege. -->

Gebäudedaten (CityGML, LOD2) rund um den Münchner Hauptbahnhof, gemeinschaftlich
gepflegt über Pull Requests. **Dieses Repository ist eine Übungs-Sandbox, die
bei Bedarf manuell zurückgesetzt wird** — hier lernen Sie die Bearbeitungswerkzeuge und den
PR-Ablauf kennen, bevor Sie zu produktiven Stadtdaten beitragen.

- **Loslegen (Übung):** das
  [Starter-Kit](https://github.com/4dcitygml/sample-munich-station/releases/download/starter-kit/munich-station-starter.zip)
  herunterladen, entpacken und `start-mac.command` (macOS) oder `start-windows.bat`
  (Windows) doppelklicken. Das gemeinsame Bearbeitungswerkzeug wird automatisch
  heruntergeladen und verbindet sich mit dieser Stadt; das Repository muss nicht geklont
  werden (Ihre eigene Kopie legt das Werkzeug an).
  Schritt für Schritt, auch für die direkte Arbeit mit Git: [Erste Schritte](docs/de/getting-started.md).
- **Datenquelle & Lizenz:** siehe `4dcitygml.json` (`attribution` / `license`).
  Datenquelle: Bayerische Vermessungsverwaltung – www.geodaten.bayern.de — CC BY 4.0.
- **Erscheinungsbild:** `theme.json` (nur deklarative Tokens; Änderungen laufen
  über den PR-Review).
- **Stadtlogo (optional):** In `4dcitygml.json` unter `logo` ein Rasterbild aus
  diesem Repository angeben (png / jpg / jpeg / webp, ≤ 1 MiB); es erscheint oben
  links in jedem Werkzeug. SVG wird nicht akzeptiert — direkt geöffnet kann ein
  SVG Skripte ausführen, was das mit den Themes geteilte Design „kein XSS durch
  Konstruktion“ brechen würde.

## Die Daten direkt in einem Viewer ansehen

Wer die CityGML-Daten nur ansehen möchte, ohne mitzuarbeiten, kann die
GML-Dateien in `lod2_citygml/` direkt mit dem kostenlosen Windows-Viewer
**[KITModelViewer](https://www.iai.kit.edu/english/4561.php)** des KIT
(Nachfolger des FZKViewer) öffnen. Auch der ältere
[FZKViewer](https://www.iai.kit.edu/english/1648.php) (Entwicklung mit 6.3
eingestellt) zeigt die Daten an. Die LoD2-Modelle enthalten keine Texturen;
einzelne Dateien können daher direkt heruntergeladen und geöffnet werden.

Zum Bearbeiten und Einreichen von Änderungen dient das gemeinsame
Bearbeitungswerkzeug (siehe „Loslegen" oben).

## Die Übungsumgebung

Der tägliche Reset und der automatische Merge sind derzeit **deaktiviert**.
Die Sandbox dient dazu, Werkzeuge und PR-Abläufe mit einer Prüfung durch den
Maintainer zu üben, ohne Produktivdaten zu berühren.

- **Manueller Reset:** Nur ein Maintainer kann nach Eingabe des Bestätigungsworts
  `RESET` den `main`-Branch auf `baseline` zurücksetzen. Offene Pull Requests
  erhalten dabei einen Hinweis.
- **Manueller Merge:** Jeder Pull Request wird vor dem Merge durch den Maintainer
  geprüft. Der Auto-Merge-Code bleibt für eine spätere Neubewertung erhalten,
  startet aber ohne die dafür vorgesehene Repository-Variable nicht.
- **Nach jedem Reset den Fork synchronisieren:** Wenn Sie dieses Repository
  geforkt haben, klicken Sie vor der nächsten Übung auf GitHub auf
  **Sync fork** → **Update branch**. Andernfalls geraten die beim Reset
  gelöschten Bearbeitungen von gestern in den Diff Ihres nächsten PRs und werden
  von der Commit-Umfang-Prüfung abgewiesen.
  - **Mit dem offiziellen Bearbeitungswerkzeug:** Die Synchronisierung geschieht
    bei jedem Start automatisch — kein manuelles Sync fork nötig.

## Hinweis zur Aufzeichnung

Übungs-PRs, Reviews und CI-Kommentare bleiben als normale öffentliche
GitHub-Historie erhalten. Eine zusätzliche Sammlung in einem separaten
Übungsprotokoll-Repository ist derzeit nicht aktiviert. Bitte veröffentlichen
Sie in PRs und Kommentaren nur Informationen, die öffentlich sein dürfen.

---

CityGML ist ein Standard des Open Geospatial Consortium (OGC). Dieses Projekt
ist nicht mit dem OGC verbunden und wird von ihm nicht unterstützt.
