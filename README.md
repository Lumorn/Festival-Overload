# Festival-Overload

## GitHub Pages Hosting

Dieses Repository ist so vorbereitet, dass GitHub Pages das Spiel direkt aus dem Repository-Root ausliefert.

1. In GitHub unter **Settings → Pages** gehen.
2. **Source** auf **Deploy from a branch** setzen.
3. Branch **main** (oder **master**) auswählen und den Ordner **/(root)** wählen.
4. Speichern und die angezeigte URL öffnen.

Wichtig: Die Startseite liegt in `index.html` im Repository-Root.

## UI-Highlights

- Neuer Spielmodus (minimal) mit großem Phasen-Status, Fokus auf Overload/Pool/Karte und Vollbild-Entscheidung Bleib/Camp.
- „Scorett“-Layout mit Top-Bar, 3-Spalten-Aufbau und klaren Chips für Overload/Pool/Deck/Ablage, damit der Spielfluss sofort sichtbar ist.
- Overload-Track als 0–12 Pills mit deutlicher Markierung von Gefahrenschwellen sowie Status-Chips (Countdown, Bühnenregel, Encore).
- Spielerleisten als große Karten mit Live/Camp-Zahlenchips, Status-Badges und Wahl-Markern für simultane Entscheidungen.
- Simultane Bleib/Camp-Entscheidung als Vollbild-Overlay inkl. Vorschau auf Pool-Bonus und Gesamtstand.
- Steuerungsmodi für Bots (Bots automatisch, Bots manuell, alles automatisch) und auswählbares Bot-Profil für modular erweiterbare KI.
- Bot-Anzahl vor Spielstart direkt in den Einstellungen per „Bot hinzufügen/entfernen“ anpassbar.
- Log als Drawer (per Button) und Kurzregeln im Spielmodus, Dev-Settings in der rechten Spalte, damit die Bühne frei bleibt und trotzdem alles erreichbar ist.
- Overload-Änderungen im Log und in den Overlays berücksichtigen die tatsächliche Deckelung bei 0/12.
- Pool-Bonus wird deterministisch pro Camper verteilt (Reihenfolge ab Aufdecker, aktuelle Richtung), Logs zeigen Live→Camp und Pool→Camp pro Spieler.
- Stabilisieren- und Push-Logs nutzen feste Kartenwerte, zeigen Vorzeichen korrekt und markieren min 0/Cap 12 inklusive Statuswerte.
- Anti-Solo camped den letzten Spieler inkl. Pool-Bonus und Trostpunkt bei 0 Live; Stage Dive stapelt keinen „Muss bleiben“-Zwang.
- KNALL-Phase loggt Pflaster (1 Live → +1 Camp) pro Spieler, RoundReset blockt Entscheidungen ohne Event und Logs nutzen die Reihenfolge Overload → Pool → Live → Camp.
- Entscheidungs-Logs sind getrennt (Choices vs. Camp/Anti-Solo/Reset-Abwicklung).
- Feedback-Bühnenregel stapelt Level (max. 3) und erhöht Push entsprechend; Log/Chips zeigen den Level.
- Katastrophen-Checks und Countdown-Logs enthalten konsistente Overload/Pool-Hinweise.
- Stage Dive wählt nie den Aufdecker selbst als Ziel; ungültige Bot-Anzahlen werden abgefangen.
- Bot-Anzahl wird auf eine ganze Zahl gerundet, um inkonsistente Zustände zu vermeiden.
- Selbsttests laufen nur noch bei `?selftest=1`, damit der normale Spielstart keine Test-Logs erzeugt.
- Der Aufdecker-Index wird vor dem Event normalisiert; bei fehlender Spielerliste wird sicher neu gestartet.
- Leere Spielerliste wird bei Entscheidung/Rundenende abgefangen, Bot-Autopump läuft dann nicht.
- Aufdecker-Index wird auch vor der Entscheidungsreihenfolge und im Bot-Autopump normalisiert.
- Event-Handler in den Einstellungen werden nur gebunden, wenn die UI-Elemente vorhanden sind.
- Status-Chips werden nur aktualisiert, wenn die UI-Elemente vorhanden sind.
- Zentrale UI-Labels werden nur aktualisiert, wenn die Elemente vorhanden sind.

## Feste Pflege-Regeln

Diese Regeln sind verbindlich und müssen bei jedem Start und jeder Bearbeitung eines Vorgangs eingehalten werden:

- Patchnotes **im Spiel** müssen immer aktualisiert werden.
- Wenn sich Spielregeln ändern, müssen sie **zusätzlich** in der Spielregeldatei `festival_overload_regelwerk_arbeitsversion_v_0.md` aktualisiert werden.
- Das README muss bei jeder Änderung immer mitgepflegt werden.
