# Firmengehirn-Plugin für Claude Code

Verbindet Claude Code mit dem Firmengehirn von Neoclarity und bringt zwei Befehle mit:
`/gehirn` (nachschlagen) und `/gehirn-merken` (eintragen).

**Entweder das Plugin (Verbindung + Befehle, empfohlen):**

```
/plugin marketplace add H-u-g-o-42/neoclarity-gehirn-plugin
/plugin install gehirn@neoclarity
```

**Oder nur die Verbindung, ohne Befehle:**

```
claude mcp add --transport http --scope user gehirn https://neoclarity-brain.vercel.app/api/mcp
```

**Nicht beides** — das Plugin bringt die Verbindung selbst mit. Wer zusätzlich `claude mcp add`
ausführt, hat das Gehirn doppelt verbunden, und jedes Werkzeug erscheint zweimal.
`--scope user` lässt die Verbindung in jedem Ordner gelten, nicht nur im aktuellen.

Beim ersten Aufruf öffnet sich die Anmeldung im Browser. Ohne eigenen Zugang zum Firmengehirn
(Einladung durch einen Admin) bekommt man nichts zu sehen. Dieses Repo enthält nur die Befehle
und die Connector-Adresse, kein Wissen. Anleitung für jede KI: https://neoclarity-brain.vercel.app/verbinden

Eine andere Firma baut ihr eigenes Plugin aus der Vorlage der Firmengehirn-App
(`vorlage/plugin/`, angelegt von `scripts/einrichten.mjs` mit der eigenen Adresse) — dieses hier
zeigt nur auf das Gehirn von Neoclarity.
