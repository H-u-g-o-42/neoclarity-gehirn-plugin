# Firmengehirn-Plugin für Claude Code

Verbindet Claude Code mit dem Firmengehirn von Neoclarity und bringt zwei Befehle mit:
`/gehirn` (nachschlagen) und `/gehirn-merken` (eintragen).

**Empfohlen — das Plugin (Verbindung + Befehle):**

```
/plugin marketplace add H-u-g-o-42/neoclarity-gehirn-plugin
/plugin install gehirn@neoclarity
```

Das Plugin bringt die Verbindung selbst mit. Bitte **nicht zusätzlich** `claude mcp add … gehirn`
ausführen — sonst ist das Gehirn doppelt verbunden und jedes Werkzeug erscheint zweimal.

**Oder — nur die Verbindung, ohne Befehle** (statt des Plugins):

```
claude mcp add --transport http --scope user gehirn https://neoclarity-brain.vercel.app/api/mcp
```

`--scope user` lässt die Verbindung in jedem Ordner gelten, nicht nur im aktuellen.

Beim ersten Aufruf öffnet sich die Anmeldung im Browser. Ohne eigenen Zugang zum Firmengehirn
(Einladung durch einen Admin) bekommt man nichts zu sehen. Dieses Repo enthält nur die Befehle
und die Connector-Adresse, kein Wissen. Anleitung für jede KI: https://neoclarity-brain.vercel.app/verbinden
