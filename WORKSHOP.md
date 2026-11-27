# Workshop-Kopiervorlagen · Dein PersonalOS

**Umsetzungsworkshop AI Explorer Club · 27.11.2026 · Vincent Mumme (mummentum)**

> Hier findest du alle Prompts aus dem Workshop mit **1-Klick-Kopierfunktion** (oben rechts in jedem Codeblock).  
> **Chat-Checkpoints im Zoom:** Nach jedem Schritt einfach die Zahl posten (`1`, `2`, `3`, `4`, `5`). Bei Problemen kurz mit Fragezeichen melden, z. B. `?1 Win Codex …`, damit Jenny gezielt helfen kann.

---

## Vor dem Start (Schritt 0)

1. **Ordner anlegen:** Erstelle direkt in deinem **Benutzerordner** einen neuen, leeren Ordner `PersonalOS` *(z. B. `/Users/deinname/PersonalOS` auf Mac oder `C:\Users\deinname\PersonalOS` auf Windows – bewusst nicht in OneDrive/iCloud-Dokumente)*.
2. **T3 Code öffnen:** Füge den leeren Ordner `PersonalOS` als Projekt hinzu.
3. **Einstellungen prüfen:**
   - Wähle deinen verbundenen Agenten (Claude Code oder Codex) und ein **mittleres Modell** *(z. B. Claude Sonnet / Standard-Codex – schont dein Nutzungslimit über 3 Stunden)*.
   - Stelle den Freigabemodus so ein, dass der Agent lokal Dateien lesen und schreiben darf *(sonst musst du jeden einzelnen Klick bestätigen)*.

---

<a id="prompt-1"></a>
## Schritt 1 · Fundament laden & Obsidian öffnen · Checkpoint `1`

Kopiere diesen Prompt in deinen ersten Chat in T3 Code:

```text
Richte diesen Ordner als mein PersonalOS ein.
Sicherheitsprüfung zuerst: Wenn dieser Ordner nicht leer ist (unsichtbare Systemdateien wie .DS_Store zählen nicht) oder nicht „PersonalOS“ heißt, stoppe sofort und frag mich.

Wenn alles passt:
1. Lade die Dateien aus dem öffentlichen GitHub-Repository https://github.com/vincentmumme/personalos-workshop-starter über einen temporären Ordner hierher – ohne .git, README.md und WORKSHOP.md. Ist git nicht installiert, lade stattdessen die ZIP-Datei (https://github.com/vincentmumme/personalos-workshop-starter/archive/refs/heads/main.zip) und entpacke den Inhalt hierher – installiere nichts nach.
2. Prüfe danach kurz, ob AGENTS.md, CLAUDE.md, INDEX.md, SOUL.md, USER.md, .gitignore, skills/, system/ sowie die leeren Ordner (people/, companies/, projects/, decisions/, inbox/) vollständig vorhanden sind.
3. Lies AGENTS.md, INDEX.md und system/rules.md und erkläre mir in 5 kurzen, verständlichen Punkten, wie dieses System funktioniert.
```

**Danach (2 Min.):** Öffne **Obsidian** → **„Ordner als Vault öffnen“** → wähle deinen Ordner `PersonalOS`. Schau kurz durch: reine Textdateien, volle Transparenz.

---

<a id="prompt-2"></a>
## Schritt 2 · Du (`USER.md` & `SOUL.md`) · Checkpoint `2`

```text
Lass uns mein persönliches Profil in USER.md und unsere Zusammenarbeit in SOUL.md einrichten.
Führe ein kurzes, fokussiertes Interview mit mir:
- Stelle mir immer nur 1–2 Fragen pro Nachricht (insgesamt maximal 5–6 Fragen): wer ich bin, woran ich aktuell arbeite, meine wichtigsten Ziele, wie ich gern arbeite und wie du mit mir kommunizieren sollst.
- Erst wenn alle Fragen beantwortet sind, schreibst du USER.md und passt SOUL.md gezielt an mich an.
- Dauerhaftes Wissen über mich gehört immer in diesen Ordner, nie ins eingebaute Memory des Anbieters.
- Zeig mir danach kurz, was du geschrieben hast, damit ich in Obsidian gegenlesen und mindestens eine Sache schärfen kann.
```

---

<a id="prompt-3"></a>
## Schritt 3 · Dein erstes Projekt einpflegen · Checkpoint `3`

Halte den **Pfad zu dem Ordner** bereit, in dem deine 3–10 vorbereiteten Unterlagen liegen *(oder kopiere 3–5 Dateien vorab in `inbox/`)*.

```text
Ich möchte jetzt ein erstes echtes Projekt in mein PersonalOS aufnehmen.
Schau zuerst in `inbox/`. Wenn dort nichts liegt, frag mich kurz nach dem Ordnerpfad meiner vorbereiteten Projektunterlagen.

Sobald du die Unterlagen gefunden hast:
1. Lies sie in Ruhe durch. Wenn du ein Dateiformat nicht direkt lesen kannst, sag es mir kurz – installiere dafür nichts nach.
2. Schlage mir anhand von AGENTS.md und system/templates/ vor, welche Dateien du anlegen würdest:
   - eine Projektdatei in projects/ (mit Current Truth oben und Timeline unten),
   - die wichtigsten Personen (people/) und Organisationen (companies/),
   - und falls sinnvoll eine erste Entscheidung in decisions/.
3. Verlinke zusammengehörende Dateien sauber mit Wikilinks im Pfadformat (z. B. [[people/vorname-nachname|Vorname Nachname]]).
4. Warte auf mein Okay, bevor du die Dateien anlegst.
```

**Danach (1 Min.):** Öffne deine neue Projektdatei in **Obsidian** und schau dir den **lokalen Graphen** an *(Befehlspalette → „Lokalen Graphen öffnen“)* – deine ersten verbundenen Knoten!

---

<a id="prompt-4a"></a>
## Schritt 4 · Der Beweis & Learning-Loop (`retro`) · Checkpoint `4`

Starte in **T3 Code** einen **brandneuen Chat** im Projekt `PersonalOS`.  
*Wenn du zwei Abos hast (z. B. Claude Code und Codex): wechsle jetzt bewusst den Anbieter!*

```text
Lies dich in mein PersonalOS ein.
1. Was ist der aktuelle Stand bei meinem Projekt, welche Personen oder Entscheidungen hängen damit zusammen, und was ist der sinnvollste nächste Schritt?
2. Erstelle direkt hier im Chat einen konkreten ersten Entwurf für diesen nächsten Schritt (z. B. eine E-Mail, eine Meeting-Agenda oder einen kurzen Umsetzungsplan).
Wichtig: Nichts extern senden, nichts verändern – nur den Entwurf hier im Chat zeigen.
```

<a id="prompt-4b"></a>
Prüfe das Ergebnis, gib deinem Agenten **eine echte Korrektur** (z. B. kürzerer Ton, geändertes Detail oder neues Datum) und schicke direkt danach:

```text
Bitte halte meine Korrektur dauerhaft im PersonalOS fest (nicht im Anbieter-Memory) und mach eine Retro für diesen Chat mit skills/retro/SKILL.md.
```

*Hinweis:* Der Retro-Skill zeigt dir erst eine kurze Liste, was er wohin schreibt – antworte kurz mit **`ok`**, dann aktualisiert er dein System.

---

## Pause & Aufholfenster *(10 Minuten)*

---

<a id="prompt-5"></a>
## Schritt 5 · Zentrale Tool-Schicht: Composio CLI · Checkpoint `5`

> **Ehrlicher Hinweis vorab:** „Lesen erlaubt, Schreiben nur mit Okay“ ist eine Regel für den Agenten in `system/tools.md`. Die OAuth-Freigabe bei Google kann technisch auch Schreibrechte umfassen – nutze deshalb ein privates Konto und starte mit einem reinen Lese-Test.  
> **Hinweis Windows ARM (Snapdragon / Copilot+):** Die native Composio CLI unterstützt aktuell nur Windows x64 – schau bei Schritt 5 entspannt zu, wir klären den besten Weg für dein Gerät in Circle.

```text
Richte die Composio CLI als zentrale Tool-Schicht für mein PersonalOS ein (siehe system/tools.md).

Ziel:
1. Prüfe zuerst, was schon erledigt ist (CLI installiert? Eingeloggt? Erstes Tool verbunden?) und mach nur das Fehlende.
2. Installiere bei Bedarf die Composio CLI passend zu meinem Betriebssystem (macOS/Linux: offizielles Install-Skript; Windows x64: PowerShell-Installer irm https://raw.githubusercontent.com/ComposioHQ/composio/next/install.ps1 | iex) und trage den funktionierenden Aufrufpfad (z. B. ~/.local/bin/composio) in system/tools.md ein.
3. Verbinde mein Composio-Konto und danach mein erstes Tool (z. B. meinen privaten Google Calendar mit Slug googlecalendar – oder frag mich kurz, welches Tool ich verbinden will).
4. Dokumentiere das verbundene Tool in system/tools.md und mache einen kurzen, reinen Lese-Test (z. B. meine Termine der nächsten 7 Tage anzeigen).

Wichtige Grenzen:
- Starte Login und Tool-Verbindung nicht-blockierend (--no-wait), gib mir den Link direkt hier im Chat, warte auf mein „fertig“ und prüfe danach mit --poll --timeout 60 bzw. composio connections list.
- Installiere nichts außer der Composio CLI – keine Adminrechte, kein WSL.
- Klappt ein Schritt nach zwei Versuchen nicht: stoppe sofort und sag mir in zwei Sätzen, woran es liegt.
- Nichts schreiben, senden oder löschen.
```

**Wenn der Lese-Test klappt (Mini-Beweis):** Frag im selben oder in einem neuen Chat: *„Schau kurz über Composio in meinen Kalender: Welche Termine der nächsten 7 Tage haben Bezug zu meinem Projekt oder meiner Arbeit?“*

---

<a id="prompt-bonus-github"></a>
## Bonus · Privates GitHub-Backup & Versionierung

```text
Ich möchte mein PersonalOS jetzt mit einem privaten GitHub-Repository sichern und versionieren.
1. Prüfe zuerst .gitignore, damit keine lokalen Dateien, Roh-Inbox-Dateien oder Secrets (.env, Schlüssel, .DS_Store) hochgeladen werden.
2. Prüfe, was auf meinem Rechner für Git/GitHub bereits da ist und ob auf meinem GitHub-Account bereits ein Repo namens „personalos“ existiert (sonst schlage einen freien Namen vor, z. B. mein-personalos).
3. Führe mich passend zu meinem Betriebssystem durch das Anlegen eines privaten Repositories und den ersten Commit + Push.
4. Wenn eine Anmeldung im Browser nötig ist, blockiere nicht im Terminal – gib mir den klaren Schritt und warte auf mein „fertig“.
5. Prüfe vor dem Push ausdrücklich, dass das Repository auf „private“ steht, und warte auf mein Okay.
```

---

<a id="prompt-rettung"></a>
## Rettungs-Prompt (falls du irgendwo hängst)

Kopiere diesen Prompt einfach in einen neuen Chat in T3 Code und ersetze `N` durch deine aktuelle Schrittnummer (`1` bis `5` oder `Bonus`):

```text
Ich mache gerade den PersonalOS-Workshop mit und hänge bei Schritt N.
Lies https://raw.githubusercontent.com/vincentmumme/personalos-workshop-starter/main/WORKSHOP.md und prüfe, was in diesem Ordner schon da ist und was bis einschließlich Schritt N noch fehlt.
Sag mir in maximal 3 kurzen Sätzen, wo ich stehe, und führe mich mit dem kleinstmöglichen nächsten Schritt wieder auf den Stand.
```
