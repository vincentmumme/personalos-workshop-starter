# AGENTS.md – Einstieg für jeden Agenten

Dieser Ordner ist mein PersonalOS: mein eigener Kontext als lesbare Markdown-Dateien. Er gehört mir, nicht einem KI-Anbieter. Jeder Agent, der hier arbeitet, folgt diesen Grundprinzipien.

## Zuerst lesen

1. `INDEX.md` – die Karte: was wo liegt
2. `USER.md` – wer ich bin, woran ich arbeite, wie ich arbeite
3. `SOUL.md` – wie du mit mir arbeitest

Danach liest du nur die Dateien, die deine aktuelle Aufgabe wirklich braucht. Beispiele und Begründungen zu den Regeln stehen bei Bedarf in `system/rules.md`.

## Grundprinzipien

1. **Kontext gehört in diesen Ordner – nie ins Anbieter-Memory.** Dauerhaftes Wissen, Vorlieben und Korrekturen schreibst du immer in Dateien dieses Ordners, niemals in das eingebaute Memory von Claude, ChatGPT/Codex oder anderen Anbietern.
2. **Eine Wahrheit, ein Ort.** Jede aktuelle Information hat genau eine zuständige Datei. Woanders wird verlinkt, nicht kopiert.
3. **Stand und Verlauf getrennt.** Oben steht die kurze **Current Truth** (wird aktualisiert), darunter die **Timeline** (datiert, es wird nur angehängt).
4. **Input ist noch keine Wahrheit.** Neues – egal ob direkt im Chat, über einen Dateipfad, in `inbox/` oder aus externen Tools – wird geprüft und eingeordnet, bevor es eine Current Truth ändert.
5. **Quellen behalten ihre Aufgabe.** Mails bleiben im Postfach, Termine im Kalender, Originaldateien im Quellsystem. Hier stehen Bedeutung und Verweis. Passwörter, Tokens und API-Schlüssel stehen nie im Klartext in diesem Ordner.
6. **Das System beschreibt sich selbst.** Regeln, verbundene Tools, Skills und Learnings stehen hier im Ordner. Jeder neue Agent versteht das System ohne Erklärung.
7. **Erst schauen, dann bauen.** Vor neuer Arbeit prüfst du `system/templates/` und `skills/`.
8. **Proaktiv, aber mit Grenzen.** Lesen, ordnen, verlinken, Entwürfe vorbereiten und Stände nachziehen darfst du selbst. Alles, was nach außen geht (Mails senden, Termine anlegen, Nachrichten posten) oder nicht rückgängig zu machen ist (löschen, Geld bewegen), braucht mein ausdrückliches Okay.
9. **Fehler werden Lernen – so wenige Regeln wie möglich.** Korrigiere ich dich, hältst du es in `system/learnings.md` fest und schärfst die betroffene Datei (`SOUL.md`, Regel, Vorlage oder Skill). Eine neue Regel kommt nur dazu, wenn sie einen echten, wiederholten Fehler verhindert.

## Konventionen

- **Dateinamen:** kleingeschrieben, Bindestriche statt Leerzeichen, keine Umlaute (`ae`, `oe`, `ue`, `ss`), z. B. `people/anna-mueller.md`, `projects/website-relaunch.md`.
- **Wikilinks:** immer als Dateipfad ohne `.md`, optional mit lesbarem Alias: `[[people/anna-mueller|Anna Müller]]`, `[[projects/website-relaunch]]`. Pfade in `system/templates/` sind Platzhalter – beim Ausfüllen immer als echte `[[pfad|Name]]`-Links schreiben. In Markdown-Tabellen den Trenner maskieren (`[[pfad\|Name]]`).
- **Datum:** immer absolut (`2026-11-27`, nie „morgen“ oder „letzte Woche“).
- **Entscheidungen:** wichtige Entscheidungen als eigene Datei in `decisions/` mit dem **Entscheidungsdatum** im Namen: `2026-11-27-kurztitel.md`.

## Skills (`skills/`)

Skills entstehen aus meiner eigenen, wiederkehrenden Arbeit – keine Sammlung externer Skills anlegen. Neue eigene Skills werden hier eingetragen:

- **`skills/retro/SKILL.md`** – nutzen am Ende eines Chats oder wenn ich sage „mach eine Retro“ / „halte das im PersonalOS fest“.
- **`skills/grill-me/SKILL.md`** – nutzen, wenn ein Plan oder eine Entscheidung noch schwammig ist oder ich sage „grill me“.

## Externe Tools (Composio CLI)

Alle externen Dienste (Kalender, Mail, Notizen, GitHub …) laufen zentral über die **Composio CLI** (`composio`). Aufrufpfad, verbundene Dienste, Auth-Regeln und Grenzen stehen in `system/tools.md`.

## Diese Struktur ist ein Anfang

Sie ist bewusst minimal. Ich entwickle sie gemeinsam mit dir aus meiner echten Arbeit weiter. Entstehen neue Bereiche/Ordner, trägt der Agent sie in `INDEX.md` ein (nur Bereiche, nicht jede einzelne Datei) und hält strukturelle Änderungen in `system/learnings.md` fest.
