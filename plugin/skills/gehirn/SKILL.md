---
name: gehirn
description: Firmengehirn von Neoclarity befragen. Nutzen bei allem, was Neoclarity als Firma betrifft (Abläufe, Regeln, Zahlen, Preise, Zuständigkeiten, Entscheidungen — in jedem Bereich der Firma) oder wenn jemand „schau im Gehirn nach“ sagt.
---

# Im Firmengehirn nachschlagen

1. `gehirn_suchen` mit 2–4 Stichworten statt der ganzen Frage, dazu zwei, drei Synonyme (eigener
   Aufruf je Begriff, wenn der erste nichts findet — „Honorar“ findet „Preise“ nicht immer).
2. Die besten Treffer mit `gehirn_lesen` ganz lesen. Notizen mit `status: überholt` nur als
   Vorgeschichte nennen; maßgeblich ist die Notiz in `ersetzt_durch`. Meldet `gehirn_lesen`
   „Meintest du …“, die genannte Notiz lesen.
3. Antworten mit Quelle: Notiz-Titel und `gilt_seit`, und die Notiz verlinken (Link aus dem
   Treffer), damit der Mensch nachlesen kann. Steht nichts im Gehirn, sag das klar — nicht aus dem
   eigenen Wissen auffüllen, ohne es als solches zu kennzeichnen.
4. „⚠ umstritten“ heißt: Angaben widersprechen sich — das dazusagen und den Widerspruch nennen.
   „⚠ Vermutung“ (`sicherheit: vermutung`) heißt: nur vermutet — das dazusagen. Meldet die Suche
   oben, dass ein Stichwort nichts fand, nicht aus den übrigen Treffern antworten.

Was ist offen, welche Fristen stehen an? → `gehirn_offen` (bei mir: `zustaendig: "ich"`).
Was hat sich geändert? → `gehirn_verlauf` (für „diese Woche“ mit `seit`).
