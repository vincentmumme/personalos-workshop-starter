# Ablauf & Prompts: Dein PersonalOS

**Umsetzungsworkshop AI Explorer Club · 27.11.2026 · Vincent Mumme (mummentum)**

> Alle Prompts funktionieren im Workshop genauso wie später beim Nacharbeiten. Du kannst sie direkt aus dem Anleitung-PDF oder hier kopieren.

---

## Vor dem Start (Schritt 0)

- **T3 Code** ([t3.codes/download](https://t3.codes/download)): Oberfläche für deine Coding-Agenten (Claude Code oder Codex einbinden).
- **Obsidian** ([obsidian.md/download](https://obsidian.md/download)): Lokaler Markdown-Viewer für deinen Ordner.
- **Composio** ([composio.dev](https://composio.dev)): Kostenlosen Account erstellen (zentrale Schnittstelle für deine Tools).
- **GitHub** ([github.com](https://github.com), optional): Kostenloser Account für dein privates Cloud-Backup.

1. **Ordner anlegen:** Erstelle direkt in deinem **Benutzerordner** einen neuen, leeren Ordner `PersonalOS` *(Mac: `/Users/deinname/PersonalOS`, Windows: `C:\Users\deinname\PersonalOS`, bewusst nicht in OneDrive/iCloud-Dokumente)*.
2. **T3 Code öffnen:** Füge den leeren Ordner `PersonalOS` als Projekt hinzu.
3. **Einstellungen prüfen:** Wähle deinen Agenten (Claude Code oder Codex), als Standard **Claude Opus 5.5 (Mittel)** oder Codex (Mittel) und erlaube lokalen Dateizugriff.

---

<a id="prompt-1"></a>
## Schritt 1: Fundament laden & Obsidian öffnen

Kopiere diesen Prompt in deinen ersten Chat in T3 Code:

```text
Richte diesen Ordner als mein PersonalOS ein.
Sicherheitsprüfung zuerst: Wenn dieser Ordner nicht leer ist (unsichtbare Systemdateien wie .DS_Store zählen nicht) oder nicht „PersonalOS“ heißt, stoppe kurz und frag mich.

Wenn alles passt:
1. Lade die Dateien aus dem öffentlichen GitHub-Repository https://github.com/vincentmumme/personalos-workshop-starter über einen temporären Ordner hierher (ohne .git, README.md und WORKSHOP.md). Ist git nicht installiert, lade stattdessen direkt die ZIP-Datei (https://github.com/vincentmumme/personalos-workshop-starter/archive/refs/heads/main.zip) und entpacke den Inhalt hierher.
2. Prüfe kurz, ob AGENTS.md, CLAUDE.md, INDEX.md, SOUL.md, USER.md, .gitignore, skills/, system/ (inkl. system/templates/) sowie die leeren Ordner (people/, companies/, projects/, decisions/, inbox/) vollständig da sind.
3. Lies AGENTS.md, INDEX.md und system/rules.md und erkläre mir in 5 kurzen Punkten, wie dieses System funktioniert und welche Pflegeaufgaben du darin für mich übernimmst.
```

**Danach (2 Min.):** Öffne **Obsidian** → **„Ordner als Vault öffnen“** → wähle `PersonalOS`. Schau kurz auf `AGENTS.md`, `INDEX.md`, `system/templates/` (Vorlagen für Personen, Organisationen, Projekte, Entscheidungen) und `skills/`.

---

<a id="prompt-2"></a>
## Schritt 2: Deine Basis (`USER.md` & `SOUL.md`)

```text
Lass uns die Basis für mein Profil in USER.md und unsere Zusammenarbeit in SOUL.md anlegen.
Stelle mir dafür nur 3 bis 4 kurze Basis-Fragen (1 bis 2 pro Nachricht): wer ich bin, woran ich aktuell arbeite, was mir wichtig ist und wie du mit mir kommunizieren sollst.

Danach schreibst du direkt USER.md und passt SOUL.md gezielt an mich an. Halte es bewusst kompakt: alles Weitere wächst gleich aus meinen echten Projektdateien und unserer Zusammenarbeit mit. Dauerhaftes Wissen über mich landet immer hier im Ordner, nie im Anbieter-Memory. Zeig mir am Ende kurz, was du geschrieben hast, damit ich es in Obsidian gegenlesen kann.
```

---

<a id="prompt-3"></a>
## Schritt 3: Dein erstes echtes Projekt einpflegen

Halte den **Pfad zu dem Ordner** bereit, in dem deine vorbereiteten Unterlagen liegen *(oder kopiere 3 bis 5 Dateien vorab in `inbox/`)*.

```text
Ich möchte jetzt mein erstes echtes Projekt in mein PersonalOS aufnehmen.
Schau zuerst in `inbox/`. Liegt dort nichts, frag mich kurz nach dem Ordnerpfad meiner vorbereiteten Projektunterlagen.

Sobald du die Unterlagen gefunden hast:
1. Lies sie mit deinen verfügbaren Mitteln ein und strukturiere den Inhalt sauber anhand von AGENTS.md und den Vorlagen in system/templates/:
   - eine Projektdatei in projects/ (Current Truth oben, Timeline unten),
   - wichtige Personen in people/ und Organisationen in companies/,
   - und falls sinnvoll eine erste Entscheidung in decisions/.
2. Verlinke zusammengehörende Dateien sauber mit Wikilinks im Pfadformat (z. B. [[people/vorname-nachname|Vorname Nachname]]).
3. Ergeben sich aus den Unterlagen wichtige Infos über mich oder meine Arbeit, ergänze auch direkt USER.md.
4. Zeig mir kurz deinen Plan und leg los, sobald ich nicke.
```

**Danach (1 Min.):** Öffne deine neue Projektdatei in **Obsidian** und schau dir den **lokalen Graphen** an *(Befehlspalette → „Lokalen Graphen öffnen“)*.

---

<a id="prompt-4a"></a>
## Schritt 4: Der Beweis & Learning-Loop (`retro` + `learnings.md`)

Starte in **T3 Code** einen **brandneuen Chat** im Projekt `PersonalOS`.  
*Wenn du zwei Abos hast (z. B. Claude Code und Codex): wechsle jetzt bewusst den Anbieter!*

```text
Lies dich in mein PersonalOS ein.
1. Was ist der aktuelle Stand bei meinem Projekt, welche Personen oder Entscheidungen hängen damit zusammen und was ist der sinnvollste nächste Schritt?
2. Erstelle direkt hier im Chat einen konkreten ersten Entwurf für diesen nächsten Schritt (z. B. eine E-Mail, eine Meeting-Agenda oder einen kurzen Umsetzungsplan).
Wichtig: Noch nichts extern senden, erst den Entwurf hier im Chat zeigen.
```

<a id="prompt-4b"></a>
Prüfe den Entwurf, gib deinem Agenten **eine echte Korrektur** (z. B. kürzerer Ton, geändertes Detail oder neues Datum) und schicke direkt danach:

```text
Halte meine Korrektur dauerhaft im PersonalOS fest (nicht im Anbieter-Memory) und mach eine Retro für diesen Chat mit skills/retro/SKILL.md. Schreib das Learning in system/learnings.md und prüfe direkt, welche Datei im System (z. B. SOUL.md, Projektdatei, Vorlage oder Regel) du dadurch verbessern solltest, damit jeder neue Chat ab sofort besser arbeitet.
```

*Hinweis:* Der Retro-Skill zeigt dir zuerst eine kurze Liste, was er wohin schreibt und verbessert. Antworte kurz mit **`ok`**, dann aktualisiert er dein System.

---

<a id="prompt-5"></a>
## Schritt 5: Zentrale Tool-Schicht (Composio CLI)

> **Ehrlicher Hinweis vorab:** „Lesen erlaubt, Schreiben nur mit Okay“ ist eine Verhaltensregel in `system/tools.md`. Die OAuth-Freigabe bei Google kann technisch auch Schreibrechte umfassen. Nutze deshalb ein privates Konto und starte mit einem reinen Lese-Test.  
> **Hinweis Windows ARM (Snapdragon / Copilot+):** Die native Composio CLI unterstützt aktuell nur Windows x64.

```text
Richte die Composio CLI als zentrale Tool-Schicht für mein PersonalOS ein (Details stehen in system/tools.md).

Ziel:
1. Prüfe zuerst, was schon erledigt ist (CLI installiert, eingeloggt, erstes Tool verbunden) und mach nur das Fehlende.
2. Installiere bei Bedarf die Composio CLI passend zu meinem Betriebssystem (macOS/Linux: offizielles Install-Skript; Windows x64: PowerShell-Installer irm https://raw.githubusercontent.com/ComposioHQ/composio/next/install.ps1 | iex) und trage den funktionierenden Aufrufpfad (z. B. ~/.local/bin/composio) in system/tools.md ein.
3. Verbinde mein Composio-Konto und ein erstes Tool (z. B. meinen privaten Google Calendar mit Slug googlecalendar, oder frag mich kurz nach meinem Wunsch-Tool).
4. Dokumentiere das verbundene Tool in system/tools.md und mache einen reinen Lese-Test (z. B. meine Termine der nächsten 7 Tage anzeigen).

Rahmen:
- Starte Login und Tool-Verbindung nicht-blockierend (--no-wait), gib mir den Link direkt hier im Chat, warte auf mein „fertig“ und prüfe danach mit --poll --timeout 60 bzw. composio connections list.
- Auf Windows kein WSL einrichten; klappt ein Schritt nach zwei Versuchen nicht, stoppe kurz und sag mir in zwei Sätzen, woran es liegt.
- Nichts extern schreiben, senden oder löschen.
```

**Wenn der Lese-Test klappt (Mini-Beweis):** Frag im selben oder in einem neuen Chat: *„Schau kurz über Composio in meinen Kalender: Welche Termine der nächsten 7 Tage haben Bezug zu meinem Projekt oder meiner Arbeit?“*

---

<a id="prompt-bonus-github"></a>
## Bonus: Privates GitHub-Backup & Versionierung

```text
Ich möchte mein PersonalOS jetzt mit einem privaten GitHub-Repository sichern und versionieren.
1. Prüfe zuerst .gitignore, damit keine lokalen Dateien, Roh-Inbox-Dateien oder Secrets (.env, Schlüssel, .DS_Store) hochgeladen werden.
2. Prüfe, was auf meinem Rechner für Git/GitHub bereits da ist und ob auf meinem GitHub-Account bereits ein Repo namens „personalos“ existiert (sonst schlage einen freien Namen vor, z. B. mein-personalos).
3. Führe mich passend zu meinem Betriebssystem durch das Anlegen eines privaten Repositories und den ersten Commit + Push.
4. Wenn eine Anmeldung im Browser nötig ist, blockiere nicht im Terminal: gib mir den klaren Schritt und warte auf mein „fertig“.
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
