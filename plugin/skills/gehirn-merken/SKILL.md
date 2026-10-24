---
name: gehirn-merken
description: Neues ins Firmengehirn von Neoclarity eintragen — von selbst, ohne Nachfrage, sobald im Gespräch eine Entscheidung, ein neuer Fakt, eine Zahl oder ein Ergebnis entsteht, das in drei Monaten noch wichtig ist. Außerdem bei „merk dir“, „trag das ein“, „fürs Gehirn“, „das hat sich geändert“, bei einem eingefügten Text (Mail vom Steuerberater, Mitschrift, Diktat), der bleiben soll, oder wenn im Gespräch eine Entscheidung fällt.
---

# Ins Firmengehirn eintragen

Die Hausordnung liefert `gehirn_uebersicht` — einmal lesen, bevor du schreibst.

1. **Wortlaut sichern:** `gehirn_quelle_ablegen` mit dem Originaltext (Diktat, Mail, was der
   Mensch gesagt hat). Nichts glätten.
2. **Suchen:** `gehirn_suchen` nach dem Thema und Synonymen. Gibt es eine passende Notiz →
   ergänzen (Schritt 3). Sonst neu anlegen unter `wiki/<bereich>/<name>.md` (Schritt 4).
3. **Ergänzen:** `gehirn_ergaenzen` mit Abschnitt (##-Überschrift) und Text — ändert nur diese
   Stelle, `gilt_seit` setzt der Server. Die Notiz nie komplett neu schicken, nur um etwas anzufügen.
4. **Neu anlegen:** `gehirn_schreiben` mit dem vollständigen Inhalt inkl. Kopf:
   `titel`, `gilt_seit`, `status`, `sicherheit`, `quelle: "[[<dateiname der quelle>]]"`,
   `auch_genannt`. Meldet der Server eine ähnliche Notiz, lieber die ergänzen.
5. **Geänderter Fakt:** `gehirn_ueberholen` (alte Notiz → überholt, neue Notiz mit Verweis, ein
   Commit). Nie löschen. **Entscheidung?** Zusätzlich `gehirn_entscheidung` — nicht
   `ENTSCHEIDUNGEN.md` selbst neu schreiben.
6. Kurz sagen, was eingetragen wurde (Notiz-Titel), nicht den ganzen Text wiederholen.

Eigene Schlüsse kennzeichnen: _(Einschätzung)_. Keine Passwörter, IBANs oder Zugangsdaten.
