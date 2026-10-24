---
name: gehirn-merken
description: Neues ins Firmengehirn von Neoclarity eintragen — von selbst, ohne Nachfrage, sobald im Gespräch eine Entscheidung, ein neuer Fakt, eine Zahl oder ein Ergebnis entsteht, das in drei Monaten noch wichtig ist. Außerdem bei „merk dir“, „trag das ein“, „fürs Gehirn“, „das hat sich geändert“, bei einem eingefügten Text (Mail vom Steuerberater, Mitschrift, Diktat), der bleiben soll, oder wenn im Gespräch eine Entscheidung fällt.
---

# Ins Firmengehirn eintragen

Die Hausordnung liefert `gehirn_uebersicht` — einmal lesen, bevor du schreibst.

1. **Suchen:** `gehirn_suchen` nach dem Thema und Synonymen. Gibt es eine passende Notiz →
   Schritt 2, sonst Schritt 3.
2. **Bestehende Notiz — EIN Aufruf:** `gehirn_ergaenzen` mit `pfad`, `abschnitt`
   (##-Überschrift), `text`, `aenderung` und `quelle_text` = der Wortlaut, den der Mensch gesagt
   oder eingefügt hat (nichts glätten, nichts kürzen). Der Server legt die Quelle ab, verlinkt sie
   im Kopf und ändert nur diesen Abschnitt — kein eigenes `gehirn_quelle_ablegen` vorher.
   `gilt_seit` ändert sich nur bei `modus: "ersetzen"` (dann heute) oder wenn du `gilt_seit`
   mitgibst (z. B. 2027-01-01 bei „ab Januar“). Die Notiz nie komplett neu schicken.
3. **Neues Thema:** erst `gehirn_quelle_ablegen` mit dem Wortlaut, dann `gehirn_schreiben` unter
   `wiki/<bereich>/<name>.md` mit dem vollständigen Inhalt inkl. Kopf: `titel`, `gilt_seit`,
   `status`, `sicherheit`, `quelle: "[[<dateiname der quelle>]]"`, `auch_genannt`. Meldet der
   Server eine ähnliche Notiz, lieber die ergänzen (Schritt 2).
4. **Entscheidung?** Zusätzlich `gehirn_entscheidung` — nicht `ENTSCHEIDUNGEN.md` selbst neu
   schreiben.
5. **Geändertes Detail:** Ändert sich ein Detail (eine Zahl, ein Datum, eine Zuständigkeit),
   ersetzt oder ergänzt du es in der bestehenden Notiz mit gehirn_ergaenzen — Git behält den alten
   Wortlaut. gehirn_ueberholen nur, wenn die Notiz als Ganzes nicht mehr gilt und ein ganz neues
   Thema an ihre Stelle tritt. Nie löschen.
6. Kurz sagen, was eingetragen wurde (Notiz-Titel), nicht den ganzen Text wiederholen.

Eigene Schlüsse kennzeichnen: _(Einschätzung)_. Keine Passwörter, IBANs oder Zugangsdaten.
