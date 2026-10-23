---
name: gehirn-merken
description: Neues ins Firmengehirn von Neoclarity eintragen — von selbst, ohne Nachfrage, sobald im Gespräch eine Entscheidung, ein neuer Fakt, eine Zahl oder ein Ergebnis entsteht, das in drei Monaten noch wichtig ist. Außerdem bei „merk dir“, „trag das ein“, „fürs Gehirn“, „das hat sich geändert“, bei einem eingefügten Text (Mail vom Steuerberater, Mitschrift, Diktat), der bleiben soll, oder wenn im Gespräch eine Entscheidung fällt.
---

# Ins Firmengehirn eintragen

Die Hausordnung liefert `gehirn_uebersicht` — einmal lesen, bevor du schreibst.

1. **Wortlaut sichern:** `gehirn_quelle_ablegen` mit dem Originaltext (Diktat, Mail, was der
   Mensch gesagt hat). Nichts glätten.
2. **Suchen:** `gehirn_suchen` nach dem Thema und Synonymen. Gibt es eine passende Notiz →
   `gehirn_lesen`, dann ergänzen. Sonst neu anlegen unter `wiki/<bereich>/<name>.md`.
3. **Schreiben:** `gehirn_schreiben` mit dem vollständigen Inhalt inkl. Kopf:
   `titel`, `gilt_seit`, `status`, `sicherheit`, `quelle: "[[<dateiname der quelle>]]"`,
   `auch_genannt`. Bei einer bestehenden Notiz den `sha` aus `gehirn_lesen` mitgeben.
4. **Geänderte Fakten:** Widerspricht das Neue einer Notiz, die alte NICHT löschen —
   `status: überholt` + `ersetzt_durch: "[[neu]]"`, die neue bekommt `ersetzt: "[[alt]]"`.
   Nur ein Detail anders → Notiz aktualisieren und `gilt_seit` neu setzen.
5. **Entscheidung?** Zusätzlich eine Zeile oben in `ENTSCHEIDUNGEN.md`.
6. Kurz sagen, was eingetragen wurde (Notiz-Titel), nicht den ganzen Text wiederholen.

Eigene Schlüsse kennzeichnen: _(Einschätzung)_. Keine Passwörter, IBANs oder Zugangsdaten.
