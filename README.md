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
- Weiter-Button im Spielmodus, der je nach Status die nächste Aktion (Entscheidung/Abschluss) anstößt.
- Kompakte Phasenleiste im Spielmodus unter dem Overload-Track, synchron zum aktuellen Status.
- „Scorett“-Layout mit Top-Bar, 3-Spalten-Aufbau und klaren Chips für Overload/Pool/Deck/Ablage, damit der Spielfluss sofort sichtbar ist.
- Overload-Track als 0–12 Pills mit deutlicher Markierung von Gefahrenschwellen sowie Status-Chips (Countdown, Bühnenregel, Twist-Effekte, Endkarte).
- Spielerleisten als große Karten mit Live/Camp-Zahlenchips, Status-Badges und Wahl-Markern für simultane Entscheidungen.
- Simultane Bleib/Camp-Entscheidung als integriertes Entscheidungsfeld im Spielbereich inkl. Vorschau auf Pool-Bonus und Gesamtstand.
- Steuerungsmodi für Bots (Bots automatisch, Bots manuell, alles automatisch) und auswählbares Bot-Profil für modular erweiterbare KI.
- Bot-Anzahl vor Spielstart direkt in den Einstellungen per „Bot hinzufügen/entfernen“ anpassbar.
- Log als Drawer (per Button) und Kurzregeln im Spielmodus, Dev-Settings in der rechten Spalte, damit die Bühne frei bleibt und trotzdem alles erreichbar ist.
- Autoplay-Toggle im Spielmodus (Play-Drawer) für schnelles Ein/Aus mit Statusanzeige.
- Spielmodus: kontraststärkeres Farbschema, größere Schrift und klarer hervorgehobene Phasen für bessere Lesbarkeit.
- Spielmodus: Symbol-Legende in den Spielerleisten plus Tooltipps für Live/Camp.
- Spielmodus: Spielerleisten lassen sich im Play-Drawer ein- und ausblenden, damit die Eventkarte dynamisch mehr Platz nutzen kann.
- Spielmodus: Primär-Buttons sind visuell stärker hervorgehoben und eindeutig beschriftet.
- Regelerinnerung im rechten Panel ist jetzt einklappbar, damit sie den Log weniger überdeckt.
- Kurzregeln sind im Spielmodus zusätzlich oben rechts erreichbar, damit die Hilfe ohne Scrollen sichtbar bleibt.
- Kompakter Meta-Block im Spielmodus zeigt Aufdecker und Richtung direkt unter dem Overload-Track.
- Kompakter Statusbereich im Spielmodus zeigt Deck- und Ablage-Anzahl direkt in der Bühne.
- Fortschrittsblock bei den Spielerleisten zeigt Leader, Camp-Stand und Abstand zum Ziel.
- Overload-Änderungen im Log und in den Overlays berücksichtigen die tatsächliche Deckelung bei 0/12.
- Pool-Bonus bei simultanem Campen folgt dem Overload-Gate (0/1/2) und der Live-Schwelle (≥2, bei Richtungswechsel ≥3); Verteilung bleibt in Zugreihenfolge.
- Stabilisieren ist ein Safety-Tool ohne Pool-Ertrag; Bonus-Live gibt es nur bei Overload ≥9.
- Crowd-Mood-Deck macht Push-Erhöhungen pro Karte leicht unberechenbar (sichtbar geloggt).
- Twist-Karten setzen Rundeneffekte (Pyro, Richtungswechsel, Afterparty) bis Rundenende.
- Endkarte Encore! gibt allen Aktiven +1 Live und triggert eine finale Camp-Entscheidung.
- DecisionWindows öffnen nur, wenn eine sinnvolle Entscheidung möglich ist oder ein Zwangseffekt greift (sonst automatisches „alle bleiben“ mit Logeintrag).
- Final Push gewährt dem letzten aktiven Spieler 1 Gnaden-Bleib, danach folgt ein erzwungenes Camp (Last Call).
- Catch-up-Bonus: Nur bei Overload ≥8, **strict** hinter dem Leader und mindestens 2 Camp Abstand; maximal 1× pro Spieler und Runde (geloggt).
- Countdown startet sofort, sobald Overload erstmals ≥8 erreicht, tickt im selben Zug und führt ggf. den Check aus, bevor Camp-Entscheidungen öffnen.
- RNG nutzt einen numerischen Seed im State/Log; Debug-Helper prüft Catch-up/Countdown/EffectIds deterministisch.
- Stabilisieren- und Push-Logs nutzen feste Kartenwerte, zeigen Vorzeichen korrekt und markieren min 0/Cap 12 inklusive Statuswerte.
- Anti-Solo läuft als Final Push: letzter aktiver Spieler bekommt 1 Extra-Event mit 1 Gnaden-Bleib, danach erzwungenes Camp.
- KNALL halbiert Live der aktiven Spieler, Pflaster rettet +1 Live nach der Halbierung; Logs nutzen Step-IDs, ActionType und Delta-Reasons.
- Debug-Export liefert JSON-Snapshots pro Step inklusive Logzeilen für spätere Analyse.
- Log-Validator prüft State-Invarianten und schreibt ASSERT_FAIL-Events bei Verstößen (Debug-Schalter).
- Entscheidungs-Logs sind getrennt (Choices vs. Camp/Anti-Solo/Reset-Abwicklung).
- Feedback-Bühnenregel stapelt Level (max. 3) und erhöht Push entsprechend; Log/Chips zeigen den Level.
- Katastrophen-Checks und Countdown-Logs enthalten konsistente Overload/Pool-Hinweise samt Flag-Deltas.
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
