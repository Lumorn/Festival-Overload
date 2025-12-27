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
- Modus-Umschalter erklärt jetzt Spielmodus und Dev per Tooltip und zeigt Hinweistext, falls eine Ansicht fehlt.
- Weiter-Button im Spielmodus, der je nach Status die nächste Aktion (Entscheidung/Abschluss) anstößt.
- Kompakte Phasenleiste im Spielmodus unter dem Overload-Track, synchron zum aktuellen Status.
- Phasen-Pills sind lokalisiert und die aktive Phase ist farbkräftig als gefülltes Pill hervorgehoben.
- Kleine Phasen-Fortschrittsleiste oberhalb der Kartenflächen für schnelle Orientierung.
- „Scorett“-Layout mit Top-Bar, 3-Spalten-Aufbau und klaren Chips für Overload/Pool/Deck/Ablage, damit der Spielfluss sofort sichtbar ist.
- Overload-Track als segmentierte Balkenleiste (grün/gelb/rot) mit klar abgegrenzten Farbzonen, größeren Segmenten/Zahlen und betontem Marker-Glow.
- Overload-Track: dauerhafte Legende oberhalb der Leiste für sichere/warnende/gefährliche Zonen.
- Overload-Track: zusätzliche Mini-Legende direkt oberhalb der Leiste für schnelle Farborientierung.
- Spielerleisten als große Karten mit Live/Camp-Zahlenchips, Status-Badges und Wahl-Markern für simultane Entscheidungen.
- Simultane Bleib/Camp-Entscheidung als zentriertes Modal-Overlay mit dunklem Hintergrund, Countdown und klaren Aktionskarten.
- Entscheidungsfenster im Spielmodus erscheint als fokussiertes Overlay, damit Bleib/Camp zentral ausgerichtet sind.
- Spielmodus skaliert Entscheidungspanel, Kartenhöhe und Abstände dynamisch mit der Viewport-Größe, inklusive Scrollbarkeit auf kleinen Screens.
- Zusätzliche Responsive-Optimierungen für niedrige Viewports: engere Abstände, reduzierte Mindesthöhen und scrollbare Nebenbereiche im Dev-Modus.
- Steuerungsmodi für Bots (Bots automatisch, Bots manuell, alles automatisch) und auswählbares Bot-Profil für modular erweiterbare KI.
- Bot-Anzahl vor Spielstart direkt in den Einstellungen per „Bot hinzufügen/entfernen“ anpassbar.
- Log als Drawer (per Button) und Kurzregeln im Spielmodus, Dev-Settings in der rechten Spalte, damit die Bühne frei bleibt und trotzdem alles erreichbar ist.
- Spielmodus: einblendbare Anleitung als rechter Drawer mit Ziel, Ablauf, Regeln, Beispielrunde und Symbol-Legende.
- Autoplay-Toggle im Spielmodus (Play-Drawer) für schnelles Ein/Aus mit Statusanzeige.
- Spielmodus: kontraststärkeres Farbschema, größere Schrift und klarer hervorgehobene Phasen für bessere Lesbarkeit.
- Panels und Kartenflächen sind heller abgestimmt, Text/Chips/Buttons nutzen einheitliche Schriftgrößen für konsistenten Kontrast.
- Hintergrundverlauf und Kartenflächen sind vereinfacht, mit größerer Karten-Typografie, stärkerem Textkontrast und mehr Innenabstand.
- Spielmodus: Symbol-Legende in den Spielerleisten plus Tooltipps für Live/Camp.
- Spielerleisten: kompakte Symbol-Legenden direkt im Bereich platziert, mit dezenteren Chips.
- Spielmodus: Spielerleisten-Legende und Werte-Icons sind größer, farblich stärker differenziert und mit klaren Tooltipps/Labels versehen.
- Spielmodus: Status- und Aufdecker-Hinweise in den Spielerleisten haben eigene Tooltips für bessere Verständlichkeit.
- Info-Icons markieren Pool-Bonus, Gate und Camp direkt im UI und zeigen kurze Tooltips.
- Spielmodus: Live/Camp-Zahlen in den Spielerleisten sind größer und klarer farbcodiert.
- Spielmodus: Spielerleisten lassen sich im Play-Drawer ein- und ausblenden, damit die Eventkarte dynamisch mehr Platz nutzen kann.
- Spielmodus: Spielerleisten erscheinen auf kleinen Screens als Drawer und lassen sich über den Play-Drawer öffnen/schließen.
- Spielmodus: Grid-Layout erlaubt der Spielerleiste auf großen Screens mehr Breite, während die Bühne stabil bleibt.
- Spielmodus: Spielerleisten werden auf mittleren Viewports gedeckelt, damit Eventkarte und Aktionsbuttons priorisiert bleiben.
- Breite Screens: Grid-Layouts und Kartenflächen skalieren kompakter, damit mehr Luft im Layout bleibt.
- Spielmodus: Primär-Buttons sind visuell stärker hervorgehoben und eindeutig beschriftet.
- Buttons haben jetzt deutlichere Hover-Effekte und klarere Active-Zustände für bessere Interaktion.
- Button-Zustände für „Warten…“, „Weiter“ und „Event aufdecken“ sind visuell klarer hervorgehoben und mit Tooltips ergänzt.
- Spielmodus: Aktive Aktionsbuttons füllen ihre Farbakzente deutlicher aus, Disabled-States sind klar ausgegraut.
- Spielmodus: Bot-Hinweis ist prominent oberhalb der Aktionsbuttons platziert.
- Disabled-States sind stärker ausgegraut, aktive Aktionen farblich betont.
- Zusätzliche Hilfetexte erklären, wann Bots automatisch oder manuell entscheiden.
- Top-Bar: Anleitung/Spielmodus/Dev mit klaren Icons, deutlicherem Hover-Feedback und aktivem Zustand; Spielmodus zeigt einen Dropdown-Hinweis.
- Entscheidungsübersicht zeigt Bot-Namen ausgeschrieben (Bot A/B/C), damit Auswahl-Chips eindeutiger sind.
- Entscheidungs-Chips zeigen vollständige Namen und kennzeichnen bereits gewählte Spieler per Tooltip.
- Bleib/Camp-Auswahl ist visuell deutlicher markiert (farbiger Hintergrund, Rahmen, Glow).
- Regelerinnerung im rechten Panel ist jetzt einklappbar, damit sie den Log weniger überdeckt.
- Kurzregeln sind im Spielmodus zusätzlich oben rechts erreichbar, damit die Hilfe ohne Scrollen sichtbar bleibt.
- Kompakter Meta-Block im Spielmodus zeigt Aufdecker und Richtung direkt unter dem Overload-Track.
- Kompakter Statusbereich im Spielmodus zeigt Deck- und Ablage-Anzahl direkt in der Bühne.
- Aktuelle Eventkarte im Spielmodus ist kompakter (geringere Höhe, kleinere Typo, engeres Padding), damit Inhalte dichter wirken.
- Spielmodus-Eventkarte ist jetzt kompakter und erhält einen veredelten Kartenrahmen mit Innen-Schatten.
- Effekte sind als integrierte Liste in der Eventkarte dargestellt, inklusive Label „Effekte“ und kompakter Variante im Spielmodus.
- Eventkarten nutzen größere Typografie mit optimierter Zeilenhöhe sowie zentrierte Inhalte für weniger Leerraum.
- Kartenflächen sind ruhiger gestaltet (weniger Textur, sanfter Verlauf) und die Karten-Typografie ist größer für bessere Lesbarkeit.
- Schmale Viewports: Buttons/Chips sind enger gesetzt, Karten behalten ihr Seitenverhältnis bei geringerer Mindesthöhe.
- Eventkarten wirken papierartiger dank doppeltem Rahmen, feiner Textur, Eckornamenten und abgerundeten Farbbändern.
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
