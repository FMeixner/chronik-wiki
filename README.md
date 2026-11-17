# Chronik-Wiki

Destilliertes Wiki unserer Splittermond-Runde. Rohtext und Source of Truth ist die Chronik (Google Doc „Die Chronik") — sie wird ausschließlich gelesen.

## Web-Ansicht (GitHub Pages)

Beim Öffnen der Pages-URL erscheint direkt das gestaltete Wiki — kein Obsidian, kein Build-Schritt:

- `index.html` (Repo-Root) — eigenständige Wiki-App: rendert die Markdown-Dateien im Browser, löst `[[Wikilinks]]` auf, zeigt die Timeline als Session-Karten, Volltextsuche, Backlinks („Erwähnt in").
- `content/manifest.json` — Seitenverzeichnis (Pfad, Titel, Typ, Status, Kurzbeschreibung, Aliase, Helden-Flag). Wird bei jeder Destillation mit aktualisiert; die App nutzt es für Navigation, Link-Auflösung und Suche.
- `.nojekyll` — verhindert, dass GitHub Pages die Markdown-Dateien per Jekyll umwandelt; sie müssen roh auslieferbar bleiben.

Einmalige Aktivierung: Repo-Settings → Pages → Branch `main`, Ordner `/ (root)`. Hinweis: GitHub Pages auf persönlichen Accounts setzt ein öffentliches Repo voraus (oder GitHub Pro); der Inhalt der Pages-Seite ist dann grundsätzlich öffentlich erreichbar — unabhängig von der Repo-Sichtbarkeit.

## Struktur

- `content/` — Wiki-Inhalte (Markdown mit YAML-Frontmatter, Obsidian-kompatibel)
  - `index.md` — Übersicht und Status quo der Gruppe
  - `Timeline.md` — ein Abschnitt pro Session (parsebares Format, Grundlage für den Reiseatlas)
  - `Personen/`, `Orte/`, `Artefakte/`, `Fraktionen/`, `Kreaturen/`
  - `_Fortschritt.md` — Destillations-Fortschritt (interner Vermerk)
  - `manifest.json` — Seitenverzeichnis für die Web-App

## Workflow

- Dienstags wird gespielt, die Chronik wird in Google Drive aktualisiert.
- Mittwochs liest der Vibe-Task das Delta und stellt Vorschläge als Pull Request (inklusive aktualisiertem `manifest.json`).
- Merge = Absegnen — ohne Zwischenschritt bei euch.

## Regeln

- Chronik nur lesen, niemals bearbeiten.
- Wiki-Seiten nie umbenennen (Wikilinks, Web-Anker und Manifest brechen sonst).
- Heldenseiten: oben `## Steckbrief` (Fähigkeiten, Besitz, Ziele, Offene Fäden), darunter die Reise als knapper Fließtext pro Abschnitt — Details siehe `_Fortschritt.md`.
- Nichts erfinden: Was die Chronik nicht hergibt, bleibt „unbekannt".
