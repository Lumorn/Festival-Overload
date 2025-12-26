# Changelog

## Unreleased
- Logging folgt nun strikt dem key=value-Schema mit Step-ID, State-Deltas und globalen Flag-Deltas.
- Debug-Snapshots werden pro Step erzeugt und der Export enthält zusätzlich strukturierte Logzeilen.
- Validatoren prüfen Log-Format und State-Invarianten; Verstöße erzeugen ASSERT_FAIL-Logs (Debug-Schalter).
- Encore-Logging wurde korrigiert (nur eine DRAW-Zeile für Encore!, danach Chain-Start und Chain-Draw).
- Countdown-Start loggt CountdownActive false->true und Countdown-Apply nutzt konsistente Change-Reasons.
- KNALL halbiert Live der aktiven Spieler, Pflaster rettet +1 Live nach der Halbierung (nur wenn Live vorher ≥1).
- Final-Push-Regel ersetzt Anti-Solo: letzter aktiver Spieler erhält 1 Extra-Event, danach normale Camp-Entscheidung.
- Stabilisieren belohnt Overload 4–7 mit +1 Pool, Overload 8+ mit +1 Live; Null-Stabi (0) bleibt exklusiv.
- Pool→Camp ist auf +1 pro Camper begrenzt (cap1), Verteilung folgt der Zugreihenfolge.
- Logging wurde auf Step-IDs, ActionTypes, Delta-Reasons und strukturierte Camp/Knall-Blöcke umgestellt.
- Debug-Export liefert JSON-Snapshots pro Turn und ist über UI/`window.exportDebug()` abrufbar.
- Selbsttests decken Pool-Cap, Knall-Halbierung, Stabilize-Rewards und Final-Push ab.
