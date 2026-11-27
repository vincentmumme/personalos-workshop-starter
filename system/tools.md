# Tools (Composio CLI)

Externe Dienste verbindet dieses System an **einer zentralen Stelle**: über die **Composio CLI** (`composio`).

Der Vorteil: Du verbindest deine Tools genau einmal in Composio. Ab diesem Moment kann **jeder** Agent in deinem PersonalOS (Claude Code, Codex, Antigravity …) auf denselben Tool-Kontext zugreifen – und wenn du morgen ein neues Tool in Composio verbindest, steht es sofort allen Agenten zur Verfügung.

## Regeln für den Agenten
- Nutze für externe Dienste die `composio` CLI (`composio search`, `composio execute`, `composio link`).
- Ist ein Dienst noch nicht verbunden, schlage vor, ihn über `composio link <dienst>` zu verbinden, und trage ihn danach unten ein.
- **Lesen** (Kalender prüfen, Mails lesen, Infos nachschlagen) ist erlaubt.
- **Schreiben nach außen** (Mails senden, Termine anlegen, Posts veröffentlichen, Daten löschen) nur nach ausdrücklichem Okay.
- Zugangsdaten und OAuth-Tokens bleiben ausschließlich in Composio – niemals in diesem Ordner.

## Verbundene Dienste

| Dienst | Wofür | Seit |
|---|---|---|
