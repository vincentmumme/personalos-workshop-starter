# Tools (Composio CLI)

Externe Dienste verbindet dieses System an **einer zentralen Stelle**: über die **Composio CLI** (`composio`).

Einmal in Composio verbunden, kann **jeder** Agent in deinem PersonalOS (Claude Code, Codex, Antigravity …) auf denselben Tool-Kontext zugreifen.

## Aufruf & Umgebung

- **CLI-Pfad:** *(wird bei der Einrichtung vom Agenten eingetragen, z. B. `~/.local/bin/composio` oder `composio` im PATH)*

## Regeln für den Agenten

- **Nicht blockierend anmelden & verbinden:** Interaktive Befehle wie `composio login` oder `composio link <dienst>` warten auf den Browser und können im Agenten-Subprozess ins Timeout laufen. Nutze deshalb nicht-blockierende Flags (`--no-wait`), gib mir den Link direkt im Chat, warte auf mein „fertig“ und prüfe den Status erst danach (`composio whoami`, `composio login --poll` bzw. `composio link <dienst> --list`). Nutze `--yes`, wo Rückfragen sonst hängen würden.
- **Keine System-Eingriffe erzwingen:** Keine Adminrechte, kein WSL nachinstallieren. Klappt ein Installations- oder Auth-Schritt nach zwei Versuchen nicht, stoppe und erkläre mir in zwei Sätzen, woran es liegt.
- **Suchen & ausführen:** `composio search "<aufgabe>"` und `composio execute <slug> -d '<json>'`.
- **Grenzen:** **Lesen** ist erlaubt. **Schreiben nach außen** (Mails senden, Termine anlegen/ändern, Nachrichten posten, Daten löschen) nur nach meinem ausdrücklichen Okay – auch wenn die OAuth-Freigabe technisch Schreibrechte umfasst.
- **Keine Secrets im Ordner:** Zugangsdaten und OAuth-Tokens bleiben ausschließlich in Composio.

## Verbundene Dienste

| Dienst | Wofür | Seit |
|---|---|---|
