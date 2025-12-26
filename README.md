# Festival-Overload

## GitHub Pages Hosting

Dieses Repository ist so vorbereitet, dass GitHub Pages das Spiel direkt aus dem Repository-Root ausliefert.

1. In GitHub unter **Settings → Pages** gehen.
2. **Source** auf **Deploy from a branch** setzen.
3. Branch **main** (oder **master**) auswählen und den Ordner **/(root)** wählen.
4. Speichern und die angezeigte URL öffnen.

Wichtig: Die Startseite liegt in `index.html` im Repository-Root.

## UI-Highlights

- „Scorett“-Layout mit Top-Bar, 3-Spalten-Aufbau und klaren Chips für Overload/Pool/Deck/Ablage, damit der Spielfluss sofort sichtbar ist.
- Overload-Track als 0–12 Pills mit deutlicher Markierung von Gefahrenschwellen sowie Status-Chips (Countdown, Bühnenregel, Encore).
- Spielerleisten als große Karten mit Live/Camp-Zahlenchips, Status-Badges und Wahl-Markern für simultane Entscheidungen.
- Simultane Bleib/Camp-Entscheidung als Vollbild-Overlay inkl. Vorschau auf Pool-Bonus und Gesamtstand.
- Log als Drawer (per Button) und Settings in der rechten Spalte, damit die Bühne frei bleibt und trotzdem alles erreichbar ist.

## Feste Pflege-Regeln

Diese Regeln sind verbindlich und müssen bei jedem Start und jeder Bearbeitung eines Vorgangs eingehalten werden:

- Patchnotes **im Spiel** müssen immer aktualisiert werden.
- Wenn sich Spielregeln ändern, müssen sie **zusätzlich** in der Spielregeldatei `festival_overload_regelwerk_arbeitsversion_v_0.md` aktualisiert werden.
- Das README muss bei jeder Änderung immer mitgepflegt werden.
