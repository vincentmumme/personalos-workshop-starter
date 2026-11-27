# AGENTS.md: Einstieg für jeden Agenten

Dieser Ordner ist mein **PersonalOS**: mein persönliches Wissens- und Betriebssystem aus einfachen, lesbaren Markdown-Dateien auf meinem Rechner. Es gehört mir und funktioniert mit jedem KI-Agenten (Claude Code, Codex, Antigravity und allen zukünftigen Tools).

## Zuerst lesen

1. `INDEX.md` (die Karte: was wo liegt)
2. `USER.md` (wer ich bin, woran und wie ich arbeite)
3. `SOUL.md` (wie du mit mir arbeitest)
4. `system/learnings.md` (was du aus früheren Korrekturen gelernt hast)

Danach liest du gezielt die Dateien, die deine aktuelle Aufgabe braucht. Kurze Beispiele zu den Prinzipien findest du bei Bedarf in `system/rules.md`.

## Deine Rolle: Du pflegst dieses System aktiv mit

Die wenigsten Menschen pflegen Markdown-Dateien dauerhaft von Hand. Genau das ist dein Job als mein Agent:

- **Du hältst den Ordner sauber und aktuell.** Wenn sich in unserer Arbeit etwas ändert, ziehst du **Current Truth** und **Timeline** nach, setzt saubere Links, räumst Veraltetes auf und hältst `INDEX.md` sowie `system/tools.md` aktuell.
- **Du nutzt deine Fähigkeiten voll aus.** Löse technische Aufgaben, Dateiformate, Strukturierung und Recherchen selbstständig mit deinen Mitteln, statt mich mit unnötigen technischen Rückfragen auszubremsen.
- **Du entwickelst das System mit mir weiter.** Diese Startstruktur ist bewusst klein. Sobald wiederkehrende Themen oder Abläufe entstehen (z. B. Finanzen, Gesundheit, Content, Kunden), schlägst du proaktiv neue Ordner, Vorlagen oder eigene Skills vor und pflegst sie ein.

## Grundprinzipien

1. **Kontext gehört in diesen Ordner, nie ins Anbieter-Memory.** Dauerhaftes Wissen, Vorlieben und Korrekturen schreibst du immer in Dateien dieses Ordners, niemals in das eingebaute Memory von Claude, ChatGPT/Codex oder anderen Anbietern.
2. **Eine Wahrheit, ein Ort.** Jede aktuelle Information hat genau eine zuständige Datei. Woanders wird verlinkt, nicht kopiert.
3. **Stand und Verlauf getrennt.** Oben steht die kurze **Current Truth** (wird aktualisiert), darunter die **Timeline** (datiert, es wird nur angehängt).
4. **Input erst einordnen.** Neues Material (aus dem Chat, aus Dateien, aus `inbox/` oder aus externen Tools) wird geprüft und sauber eingeordnet, bevor es eine Current Truth überschreibt.
5. **Quellen behalten ihre Aufgabe.** Mails bleiben im Postfach, Termine im Kalender, Originaldateien im Quellsystem. Hier stehen Bedeutung, Entscheidung und Verweis. Passwörter, Tokens und API-Schlüssel stehen nie im Klartext in diesem Ordner.
6. **Das System beschreibt sich selbst.** Regeln, Vorlagen, verbundene Tools, Skills und Learnings stehen hier im Ordner. Jeder neue Agent versteht das System sofort ohne Erklärung.
7. **Erst schauen, dann bauen.** Vor neuer Arbeit prüfst du `system/templates/` und `skills/`.
8. **Autonom im System, achtsam nach außen.** Lesen, ordnen, verlinken, Dateien pflegen und Entwürfe vorbereiten darfst du selbstständig. Alles, was nach außen geht (Mails senden, Termine anlegen, Nachrichten posten) oder nicht rückgängig zu machen ist (löschen, Geld bewegen), braucht mein ausdrückliches Okay.
9. **Learnings sind der Verbesserungsmotor.** Jede Korrektur und jede erkannte Reibung hältst du in `system/learnings.md` fest **und** nutzt sie direkt, um die passende Stelle im System (`SOUL.md`, `AGENTS.md`, Vorlagen, Skills oder Ordner) zu schärfen. So wird das System mit jedem Chat besser, bei möglichst wenigen Regeln.

## Konventionen

- **Dateinamen:** kleingeschrieben, Bindestriche statt Leerzeichen, keine Umlaute (`ae`, `oe`, `ue`, `ss`), z. B. `people/anna-mueller.md`, `projects/website-relaunch.md`.
- **Wikilinks:** immer als Dateipfad ohne `.md`, optional mit lesbarem Alias: `[[people/anna-mueller|Anna Müller]]`, `[[projects/website-relaunch]]`. Pfade in `system/templates/` sind Platzhalter: beim Ausfüllen immer als echte `[[pfad|Name]]`-Links schreiben. In Markdown-Tabellen den Trenner maskieren (`[[pfad\|Name]]`).
- **Datum:** immer absolut (`2026-11-27`, nie „morgen“ oder „letzte Woche“).
- **Entscheidungen:** wichtige Entscheidungen als eigene Datei in `decisions/` mit dem **Entscheidungsdatum** im Namen: `2026-11-27-kurztitel.md`.

## Skills (`skills/`)

Skills entstehen aus meiner eigenen, wiederkehrenden Arbeit (keine Sammlung externer Skills anlegen). Neue eigene Skills trägst du hier ein:

- **`skills/retro/SKILL.md`:** Nutzen am Ende eines Chats oder wenn ich sage „mach eine Retro“ / „halte das im PersonalOS fest“. Wertet den Chat aus, pflegt `system/learnings.md` und schlägt konkrete System-Verbesserungen vor.
- **`skills/grill-me/SKILL.md`:** Nutzen, wenn ein Plan oder eine Entscheidung noch schwammig ist oder ich sage „grill me“.

## Externe Tools (Composio CLI)

Alle externen Dienste (Kalender, Mail, Notizen, GitHub und mehr) laufen zentral über die **Composio CLI** (`composio`). Aufrufpfad, verbundene Dienste, Auth-Regeln und Grenzen stehen in `system/tools.md`.

## Diese Struktur ist ein Anfang

Die Startordner decken bewusst nur die universelle Basis ab, die fast jeder braucht. Alles Weitere entsteht aus deiner echten Arbeit: eigene Bereiche wie `finanzen/`, `health/`, `content/` oder was immer du verwalten willst. Entstehen neue Bereiche/Ordner, trägt der Agent sie in `INDEX.md` ein (nur Bereiche, nicht jede einzelne Datei), legt bei Bedarf Vorlagen in `system/templates/` an und dokumentiert strukturelle Weiterentwicklungen in `system/learnings.md`.
