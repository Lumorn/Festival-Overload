# Changelog

## Unreleased
- Kompakte Phasenleiste im Spielmodus ergänzt (Aufdecken/Effekt/Countdown/Entscheidung).
- Catch-up-Bonus nur noch bei strikt hinter dem Leader und Abstand ≥2; max. 1× pro Spieler/Runde.
- Countdown startet sofort bei Overload ≥8, tickt im selben Zug und triggert Check vor der Camp-Entscheidung.
- Logger nutzt feste EffectIds, keine UNKNOWN_EFFECT-Einträge; Detail-Felder sind roh.
- ROUND_END-Logs sind entdoppelt (Summary eigenes ActionType).
- RNG nutzt numerischen Seed im State/Log, Debug-Helper für deterministische Engine-Checks.
- Crowd-Mood-Deck (−1/0/0/+1/+1/+2) modifiziert Push-Overload per Karte und wird geloggt.
- Stabilisieren liefert keinen Pool mehr; Bonus-Live nur bei Overload ≥9.
- Pool→Camp unterliegt dem Overload-Gate (0/1/2) und der Live-Schwelle (≥2/≥3 bei Richtungswechsel).
- Twist-Karten aktivieren Rundeneffekte (Pyro, Richtungswechsel, Afterparty) bis Rundenende.
- Afterparty startet Countdown sofort und erhöht den Tick auf +2.
- Endkarte Encore! gibt allen Aktiven +1 Live und erzwingt eine finale Camp-Entscheidung.
- Catch-up-Bonus: Letzte Camp-Stände erhalten bei Overload ≥8 +1 Camp beim Campen.
- Bots nutzen die neuen Camp-Regeln (Gate, Live-Schwelle, Finale Camp-Phase).
- Nach jeder Kartenauflösung werden Overload/Pool/Live/Camp geklammert.
