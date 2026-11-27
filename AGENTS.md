# AGENTS.md – Einstieg für jeden Agenten

Dieser Ordner ist mein PersonalOS: mein eigener Kontext als lesbare Markdown-Dateien. Er gehört mir, nicht einem KI-Anbieter. Jeder Agent, der hier arbeitet, folgt diesen Grundprinzipien.

## Zuerst lesen

1. `INDEX.md` – die Karte: was wo liegt
2. `USER.md` – wer ich bin, woran ich arbeite, wie ich arbeite
3. `SOUL.md` – wie du mit mir arbeitest
4. `system/rules.md` – die Grundregeln mit Beispielen

Danach liest du nur die Dateien, die deine Aufgabe wirklich braucht.

## Grundregeln

1. **Eine Wahrheit, ein Ort.** Jede aktuelle Information hat genau eine zuständige Datei. Woanders wird mit `[[Wikilinks]]` verlinkt, nicht kopiert.
2. **Stand und Verlauf getrennt.** Oben steht die kurze **Current Truth** (wird aktualisiert), darunter die **Timeline** (datiert, es wird nur angehängt).
3. **Input ist noch keine Wahrheit.** Neues – egal ob direkt im Chat, in `inbox/` oder aus externen Tools – wird geprüft und eingeordnet, bevor es eine Current Truth ändert.
4. **Quellen behalten ihre Aufgabe.** Mails bleiben im Postfach, Termine im Kalender, Dateien im Quellsystem. Hier stehen Bedeutung und Verweis. Passwörter, Tokens und API-Schlüssel stehen nie im Klartext in diesem Ordner.
5. **Das System beschreibt sich selbst.** Regeln, verbundene Tools, Skills und Learnings stehen hier im Ordner. Jeder neue Agent versteht das System ohne Vorwissen.
6. **Erst schauen, dann bauen.** Vor neuer Arbeit prüfst du `system/templates/` und `skills/`.
7. **Proaktiv, aber mit Grenzen.** Ordnen, verlinken, vorbereiten und Stände nachziehen darfst du selbst. Alles, was nach außen geht (Mails senden, Termine anlegen, Nachrichten posten) oder nicht rückgängig zu machen ist (löschen, Geld bewegen), braucht mein ausdrückliches Okay.
8. **Fehler werden Lernen.** Korrigiere ich dich, hältst du es in `system/learnings.md` fest und schärfst die betroffene Regel, Vorlage, `SOUL.md` oder den Skill.
9. **So wenige Regeln wie möglich.** Moderne Modelle können extrem viel selbst. Eine neue Regel kommt nur dazu, wenn sie einen echten, wiederholten Fehler verhindert.

**Konventionen:** Dateinamen klein mit Bindestrichen (`projects/mein-projekt.md`) · Verlinken mit `[[Wikilinks]]` · Datumsangaben immer absolut (`2026-11-27`, nie „morgen“) · wichtige Entscheidungen als eigene Datei in `decisions/`.

## Skills und Tools

- **Skills (`skills/`):** Passt eine Aufgabe zu einem Skill, liest du seine `SKILL.md` und folgst ihr. Neue Skills entstehen aus meiner echten, wiederkehrenden Arbeit – keine Sammlung externer Skills anlegen.
- **Externe Tools (Composio CLI):** Alle externen Dienste (Kalender, Mail, Notizen, GitHub …) laufen zentral über die **Composio CLI** (`composio`). Was verbunden ist und welche Grenzen gelten, steht in `system/tools.md`.

## Diese Struktur ist ein Anfang

Sie ist bewusst minimal. Ich entwickle sie gemeinsam mit dir aus meiner echten Arbeit heraus weiter. Änderst du Struktur oder Regeln, aktualisierst du `INDEX.md` und hältst es in `system/learnings.md` fest.
