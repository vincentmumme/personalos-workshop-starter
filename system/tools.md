# Tools (Composio CLI)

Externe Dienste verbindet dieses System an **einer zentralen Stelle**: über die **Composio CLI** (`composio`).

Einmal in Composio verbunden, kann **jeder** Agent in deinem PersonalOS (Claude Code, Codex, Antigravity …) auf denselben Tool-Kontext zugreifen.

## Aufruf & Umgebung

- **CLI-Pfad:** *(wird bei der Einrichtung vom Agenten eingetragen, z. B. `~/.local/bin/composio` oder der konkrete Pfad unter Windows – wichtig, da ein frisch gesetzter `PATH` oft erst im nächsten Terminal greift)*

## Regeln für den Agenten

- **Installation je Betriebssystem:**
  - macOS / Linux: offizielles Installationsskript (`curl -fsSL https://composio.dev/install | bash`).
  - Windows (x64): nativer PowerShell-Installer (`irm https://raw.githubusercontent.com/ComposioHQ/composio/next/install.ps1 | iex`, experimentell). Auf Windows ARM64 nicht unterstützt.
  - Keine Adminrechte, kein WSL nachinstallieren. Klappt ein Schritt nach zwei Versuchen nicht, stoppe und erkläre mir in zwei Sätzen, woran es liegt.
- **Nicht blockierend anmelden & verbinden:**
  - Login starten: `composio login --no-wait --yes` (gibt den Browser-Link direkt aus, ohne zu blockieren; Sitzung ist ca. 10 Minuten gültig).
  - Gib mir den Link im Chat und warte auf mein „fertig“. Prüfe danach mit `composio login --poll --timeout 60` (oder `composio whoami`). Falls abgelaufen, neu mit `--no-wait` starten.
  - Tool verbinden (z. B. Kalender-Slug `googlecalendar`): `composio link <dienst> --no-wait` → Link im Chat geben → auf „fertig“ warten → danach `composio link <dienst> --list` oder `composio connections list` prüfen.
- **Suchen & ausführen:** `composio search "<aufgabe>"` und `composio execute <slug> -d '<json>'`.
- **Grenzen:** **Lesen** ist erlaubt. **Schreiben nach außen** (Mails senden, Termine anlegen/ändern, Nachrichten posten, Daten löschen) nur nach meinem ausdrücklichen Okay – auch wenn die OAuth-Freigabe technisch Schreibrechte umfasst oder eine CLI-Ausgabe zum direkten Fortfahren auffordert.
- **Keine Secrets im Ordner:** Zugangsdaten, OAuth-Tokens und Login-/Link-URLs mit Sitzungsschlüssel niemals in diesem Ordner speichern oder im Screenshare teilen.

## Verbundene Dienste

| Dienst | Wofür | Seit |
|---|---|---|
