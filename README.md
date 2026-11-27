# PersonalOS · Workshop-Starter

Minimaler, providerunabhängiger Startpunkt für dein eigenes **PersonalOS** – aus dem Umsetzungsworkshop **„Dein PersonalOS“** (Vincent Mumme / mummentum · AI Explorer Club).

> **Die Idee:** Dein Kontext gehört dir, nicht einem KI-Anbieter. Ein Ordner aus lesbaren Markdown-Dateien, kombiniert mit **Obsidian** (Ansicht), **T3 Code** (Agenten-Oberfläche) und der **Composio CLI** (zentrale Tool-Anbindung).

## So startest du

1. Lege auf deinem Rechner einen leeren Ordner `PersonalOS` an.
2. Öffne diesen Ordner als Projekt in **T3 Code** (oder deinem Coding-Agenten).
3. Gib deinem Agenten diesen Auftrag:

```text
Hol dir die Dateien aus https://github.com/vincentmumme/personalos-workshop-starter in diesen Ordner (ohne die Git-Historie der Vorlage). Lies danach AGENTS.md, INDEX.md und system/rules.md und erkläre mir in 5 kurzen Punkten, wie dieses System funktioniert.
```

*(Alternativ: oben rechts auf **Code → Download ZIP** klicken und den Inhalt in deinen Ordner `PersonalOS` entpacken.)*

## Was drin liegt

- `AGENTS.md` & `CLAUDE.md` – Einstieg und Grundprinzipien für jeden Agenten
- `INDEX.md` – die Karte: was wo liegt
- `USER.md` & `SOUL.md` – wer du bist und wie dein Agent mit dir arbeitet
- `people/`, `companies/`, `projects/`, `decisions/`, `inbox/` – deine leeren Inhaltsordner
- `skills/` – bewusst nur zwei Skills zum Start: `retro` (Standard) und `grill-me` (als einziges externes Beispiel – Skills entstehen aus deiner eigenen Arbeit, nicht durch Sammeln)
- `system/` – ausführliche Grundregeln, 4 Vorlagen, `tools.md` (Composio CLI) und `learnings.md`
