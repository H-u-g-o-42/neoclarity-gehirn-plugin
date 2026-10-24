---
name: gehirn-merken
description: Neues ins Firmengehirn von Neoclarity eintragen (nur mit Schreibrecht) — von selbst, ohne Nachfrage, sobald im Gespräch eine Entscheidung, ein neuer Fakt, eine Zahl oder ein Ergebnis entsteht, das in drei Monaten noch wichtig ist. Außerdem bei „merk dir“, „trag das ein“, „fürs Gehirn“, „das hat sich geändert“, bei einem eingefügten Text (Mail vom Steuerberater, Mitschrift, Diktat), der bleiben soll, oder wenn im Gespräch eine Entscheidung fällt.
---

# Ins Firmengehirn eintragen

Fehlen die Schreib-Werkzeuge, darfst du nur lesen — sag das.

Die Hausordnung liefert `gehirn_uebersicht` — einmal lesen, bevor du schreibst.

1. **Suchen:** `gehirn_suchen` nach dem Thema und Synonymen. Gibt es eine passende Notiz →
   Schritt 2, sonst Schritt 3.
2. **Bestehende Notiz — EIN Aufruf:** `gehirn_ergaenzen` mit `pfad`, `abschnitt`
   (##-Überschrift), `text`, `aenderung` und `quelle_text` = der Wortlaut, den der Mensch gesagt
   oder eingefügt hat (nichts glätten, nichts kürzen). Der Server legt die Quelle ab, verlinkt sie
   im Kopf und ändert nur diesen Abschnitt — kein eigenes `gehirn_quelle_ablegen` vorher.
   Ändert sich nur eine Zahl oder ein Wort: `modus: "stelle"` mit `alt` (der genaue bisherige
   Wortlaut) und `neu` — nicht den ganzen Abschnitt neu schicken.
   `gilt_seit` wird bei `modus: "ersetzen"` und `"stelle"` heute, beim Anhängen bleibt es — oder du
   gibst `gilt_seit` mit (z. B. 2027-01-01 bei „ab Januar“). Die Notiz nie komplett neu schicken.
3. **Neues Thema:** erst `gehirn_quelle_ablegen` mit dem Wortlaut, dann `gehirn_schreiben` unter
   `wiki/<bereich>/<name>.md` mit dem vollständigen Inhalt inkl. Kopf: `titel`, `gilt_seit`,
   `status`, `sicherheit`, `quelle: "[[<dateiname der quelle>]]"`, `auch_genannt`. Der erste Satz
   unter `## Kern` sagt, worum es geht (keine Verneinung). Meldet der Server eine ähnliche Notiz,
   lieber die ergänzen (Schritt 2).
4. **Entscheidung?** Zusätzlich `gehirn_entscheidung` mit `quelle_text` (Quelle und Entscheidung
   in einem Schritt) — nicht `ENTSCHEIDUNGEN.md` selbst neu schreiben.
5. **Offener Punkt erledigt?** `gehirn_erledigt` mit dem Titel aus `gehirn_offen` und dem Ergebnis
   — nicht von Hand in der Tabelle abhaken.
6. **Geändertes Detail:** Ändert sich ein Detail (eine Zahl, ein Datum, eine Zuständigkeit),
   ersetzt oder ergänzt du es in der bestehenden Notiz mit gehirn_ergaenzen — Git behält den alten
   Wortlaut. gehirn_ueberholen nur, wenn die Notiz als Ganzes nicht mehr gilt und ein ganz neues
   Thema an ihre Stelle tritt. Nie löschen.
7. Kurz sagen, was eingetragen wurde (Notiz-Titel, Link zum Ansehen), nicht den ganzen Text
   wiederholen. Nennt die Bestätigung Stellen, an denen der alte Wert noch steht, prüf sie.
   Will der Mensch die Änderung nicht: Link „Änderung“ aus der Bestätigung öffnen und
   „Zurückdrehen“ tippen.

Was sich zuletzt geändert hat, zeigt `gehirn_verlauf`. Eigene Schlüsse kennzeichnen:
_(Einschätzung)_. Keine Passwörter, IBANs oder Zugangsdaten.
