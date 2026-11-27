# Grundregeln

Die Kurzfassung steht in `AGENTS.md`. Hier steht kurz, warum es diese Prinzipien gibt.

## 1. Eine Wahrheit, ein Ort
Jede aktuelle Information hat genau eine zuständige Datei. Der Stand eines Projekts steht in der Projektdatei, nicht zusätzlich in einer Personendatei.
*Beispiel:* In `people/anna.md` steht „arbeitet mit mir an `[[projects/website-relaunch]]`“ – nicht der aktuelle Projektstand.

## 2. Stand und Verlauf getrennt
Jede Datei, die sich über die Zeit verändert, hat oben **Current Truth** (kurz, aktuell, wird überschrieben) und unten eine **Timeline** (datiert, es wird nur angehängt).
*Beispiel:* Verschiebt sich ein Termin, ändert sich die Current Truth. In die Timeline kommt: `- 2026-11-27 | Kickoff auf 04.12. verschoben.`

## 3. Input ist noch keine Wahrheit
Notizen, Dateien, Chat-Nachrichten oder Inhalte aus Mails/Terminen sind zuerst Rohmaterial. Der Agent prüft: Was ist neu, was hat sich geändert, wohin gehört es? Erst danach wird eine Current Truth angepasst. `inbox/` kannst du als Parkplatz nutzen – oder neuen Kontext direkt im Chat übergeben.

## 4. Quellen behalten ihre Aufgabe
Die Mail bleibt im Postfach, der Termin im Kalender, die Rechnung in der Buchhaltung. Im PersonalOS stehen Bedeutung, Zusammenhang und Verweis. Zugangsdaten, Passwörter und API-Schlüssel gehören niemals in diesen Ordner.

## 5. Das System beschreibt sich selbst
Regeln, Vorlagen, verbundene Tools, Skills und Learnings liegen im Ordner. Dadurch versteht jeder neue Chat – und jeder neue KI-Anbieter – dein System sofort ohne Erklärung.

## 6. Erst schauen, dann bauen
Bevor der Agent eine neue Datei oder einen neuen Ablauf anlegt, prüft er `system/templates/` und `skills/`. Was sich bewährt hat, wird wiederverwendet.

## 7. Proaktiv, aber mit Grenzen
Der Agent darf lesen, ordnen, verlinken, Entwürfe vorbereiten und Vorschläge machen. Mails senden, Termine erstellen, Nachrichten verschicken, Dateien löschen oder Geld bewegen darf er nur nach deinem ausdrücklichen Okay.

## 8. Fehler werden Lernen
Jede Korrektur ist wertvolles Signal. Der Agent trägt in `system/learnings.md` ein, was er gelernt hat, und passt die passende Regel, Vorlage, `SOUL.md` oder den Skill an. So wird dein System Woche für Woche besser.

## 9. So wenige Regeln wie möglich
Aktuelle Modelle sind extrem leistungsfähig und brauchen wenig Bürokratie. Füge eine neue Regel nur dann hinzu, wenn sie einen echten, wiederkehrenden Fehler verhindert.

## Konventionen
- Dateinamen klein mit Bindestrichen: `projects/mein-projekt.md`
- Verlinken mit `[[Wikilinks]]`
- Datumsangaben absolut: `2026-11-27`
- Wichtige Entscheidungen als eigene Datei in `decisions/`: `2026-11-27-kurztitel.md`
