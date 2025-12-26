# Festival Overload – Regelwerk (Arbeitsversion)

**Stand:** integrierte Push-your-Luck-Version (simultan „Bleib / Camp“), optimiert für schnelle, laute Festival-Runden ohne Verwaltungsphasen.

---

## 1) Spielziel

Du gewinnst **sofort**, sobald du **8 Camp-Punkte** erreicht hast.

* **Camp** ist permanent und sicher.
* **Live** gilt nur für die aktuelle Runde und kann jederzeit verloren gehen.
* Es wird **nichts notiert**: Alle Punkte liegen als **Punktekarten offen** vor den Spielern.

---

## 2) Kerngefühl

Jede Runde eskaliert sichtbar. Nach **jedem Event** steht dieselbe Frage im Raum:

> **Bleibst du drin und riskierst alles – oder campst du jetzt und sicherst deinen Gewinn?**

Diese Entscheidung treffen **alle aktiven Spieler gleichzeitig und offen**. Gruppendruck, Bluffen und Eskalation sind ausdrücklich gewollt.

---

## 3) Begriffe

* **Overload**: Gemeinsamer Gefahrenwert der Runde (0–12).
* **Live**: Unsichere Punktekarten eines Spielers für diese Runde (liegen **quer** vor ihm).
* **Camp**: Sichere Siegpunkte eines Spielers für das Spiel (liegen **gerade** vor ihm).
* **Aktiv**: Spieler ist noch in der Runde und entscheidet Bleib/Camp mit.
* **Gecampt**: Spieler ist ausgestiegen und ignoriert alle weiteren Events dieser Runde.
* **Knall**: Katastrophe. Beendet die Runde sofort.

---

## 4) Material

* 1 **Event-Deck** (siehe Kartentypen & Test-Deckliste)
* 1 **Overload-Anzeige** (0–12)
* **Punktekarten** (empfohlen: mindestens 80), genutzt für:
  * Live (quer vor Spielern)
  * Camp (gerade vor Spielern)
  * **Bühnen-Pool** (offen in der Tischmitte)

Weitere Komponenten werden nicht benötigt.

---

## 5) Setup

1. Mische das Event-Deck.
2. Lege den Overload-Marker auf **0**.
3. Lege einen offenen **Bühnen-Pool** in die Tischmitte (startet leer).
4. Jeder Spieler startet mit:
   * **0 Live**
   * **0 Camp**
5. Bestimme einen Startspieler.

---

## 6) Rundenablauf (Kurzfassung)

Eine Runde läuft in einer Schleife:

1. **Event aufdecken** (genau 1 Karte)
2. **Event vollständig ausführen** (inkl. Ketten, Overload-Check)
3. **Alle aktiven Spieler gleichzeitig: Bleib oder Camp**
4. Nächster aktiver Spieler deckt das nächste Event auf

Die Runde endet durch **Knall** oder wenn **alle Spieler gecampt** haben.

---

## 7) Wer deckt auf?

Der aktuell **aktive Spieler** deckt die oberste Karte des Event-Decks auf, führt sie vollständig aus und legt sie anschließend offen auf den Ablagestapel.

Danach geht das Aufdecken **im Uhrzeigersinn** an den nächsten **aktiven** Spieler weiter.

* Gecampte Spieler werden übersprungen.
* Ist das Deck leer, wird der Ablagestapel gemischt und als neues Deck verwendet.

---

## 8) Kartentypen

### A) Push (⚡)

Wenn eine Push-Karte aufgedeckt wird:

1. **Overload +X** (maximal 12)
2. Der aufdeckende Spieler erhält **+1 Live**
3. Lege **+1 Punktekarte** in den **Bühnen-Pool**
4. Führe danach sofort den **Overload-Check** aus (siehe Abschnitt 11)

---

### B) Stabilisieren (🛠️)

Wenn eine Stabilisieren-Karte aufgedeckt wird:

1. **Overload −X** (nicht unter 0).

**Ertrag (nur wenn es wirklich brenzlig ist):**

* War der Overload **vor dem Senken 8 oder höher**, erhält der aufdeckende Spieler **+1 Live** (aus dem Vorrat).
* War der Overload **unter 8**, gibt es **keinen Live-Ertrag**.

Stabilisieren ist damit **Rettung mit Risiko-Belohnung**, aber keine sichere Punktequelle bei niedrigem Overload.

---

---


### C) Twist (🌀)

Twists sind Chaos-Schalter. Es gibt zwei Arten:

1. **Sofort-Twist**: Effekt ausführen, danach Karte ablegen.
2. **Bühnenregel (🌀∞)**: Bleibt offen liegen und gilt bis zum Rundenende.

* Es kann immer nur **eine Bühnenregel gleichzeitig** aktiv sein.
* Wird eine neue Bühnenregel aufgedeckt, ersetzt sie die alte.

---

### D) Encore! (🎤) – Ketten-Event

Encore bedeutet: **Sofort ein weiteres Event**, bevor irgendwer campen darf.

* Der **aufdeckende Spieler** darf **1 Live zahlen**, um Encore zu stoppen.
* Zahlt er nicht (oder kann nicht), deckt er sofort die nächste Karte auf.
* Mehrere Encore können sich **ketten**.

**Wichtig:** Erst wenn keine Encore-Kette mehr läuft, kommt die Bleib/Camp-Entscheidung.

---

## 9) Bleib oder Camp (simultan)

Nach jedem abgeschlossenen Event (inkl. Encore-Ketten, Twist-Effekt und Overload-Check) entscheiden alle **aktiven Spieler gleichzeitig**:

### Bleib

* Du bleibst aktiv.
* Dein gesamtes Live bleibt im Risiko.

### Camp (nur mit Live erlaubt)

* Du darfst **nur campen, wenn du mindestens 1 Live** hast.

Wenn du campst:

1. Wandle dein gesamtes **Live → Camp** um.
2. Setze dein Live auf **0**.
3. Nimm den **Pool-Bonus** (siehe unten).
4. Du bist für den Rest der Runde **gecampt** und ignorierst alle weiteren Effekte.

**Merksatz:** Ohne Live gibt es keinen Cashout.

### Pool-Bonus beim Campen

Wenn du campst (nur mit mindestens 1 Live):

* **poolTake = min(Pool, 1 + dangerBonus)**
* **dangerBonus = 1**, wenn Overload **8 oder höher** ist, sonst **0**.

### Pool-Bonus bei simultanem Campen

* **Reihenfolge:** beginnend beim **aktuellen Aufdecker**, dann in der **aktuellen Richtung**.
* Jeder Camper nimmt seinen **Pool-Bonus sofort** gemäß `poolTake`.

**Wichtig:** Maßgeblich ist der **Overload nach dem Event** (inkl. Countdown und Overload-Checks), **direkt vor der Camp-Entscheidung**.

---


## 10) Kosten statt Zwang (No-Thanks-Grundregel)

Trifft dich ein **Zwangseffekt** (z. B. Twist oder Encore), darfst du:

* **1 Live zahlen**, um für diesen Effekt als **nicht betroffen** zu gelten.

**Grenzen:**

* Gilt nicht für Effekte, die ausdrücklich **alle aktiven Spieler** betreffen.
* Zahlen ist nur möglich, wenn du mindestens **1 Live** hast.

---

## 11) Overload, 12 und Knall

### Overload-Grenzen

* Overload liegt immer zwischen **0 und 12**.

### Overload-Check

Immer wenn Overload **12 erreicht**:

1. Decke die oberste Karte des Decks als **Katastrophen-Check** auf (nur Typ prüfen).
2. Ergebnis:
   * **Push (⚡)** → **Knall**
   * **kein Push** → Glück gehabt:
     * Lege die Karte ohne Effekt ab.
     * Setze Overload auf **10** (Rückstoß).

### Knall

Bei Knall:

* Alle **aktiven Spieler** verlieren ihr gesamtes Live.
* Gecampte Spieler sind nicht betroffen.
* Die Runde endet **sofort**.

**Optionale Frustbremse („Pflaster“):**

* Jeder aktive Spieler darf **1 Live als Camp retten**.

---

## 12) Countdown nach erstem Camper

Der Countdown wird **erst dann aktiv**, wenn in einer Runde **zum ersten Mal ein Spieler erfolgreich camped** (also mit mindestens 1 Live).

Solange der Countdown aktiv ist:

* Nach **jedem weiteren Event** steigt der Overload automatisch um **+1**.
* **Optionaler Eskalations-Boost:** Liegen **mindestens 3 Karten im Bühnen-Pool**, steigt der Overload stattdessen um **+2**.
* Jeder Anstieg kann einen Overload-Check auslösen.

---


## 13) Rundenende & Neustart

Eine Runde endet, wenn:

* ein **Knall** passiert, oder
* **alle Spieler gecampt** haben.

### 13a) Anti-Solo-Downtime (letzter aktiver Spieler)

Sobald nur noch **1 Spieler aktiv** ist:

* Die Runde endet **sofort**.
* Der letzte aktive Spieler **camped sofort** (Live → Camp).
* Er nimmt **Pool-Bonus** gemäß `poolTake` (Regel aus Abschnitt 9).
* Falls sein Live **0** ist, erhält er **+1 Trostpunkt** aus dem Vorrat.

**Ziel:** Keine Solo-Downtime und trotzdem ein fairer Abschluss ohne „0-Punkte“-Ende.

### Neustart

1. Overload auf **0** setzen.
2. Bühnenregel entfernen.
3. Bühnen-Pool leeren (Karten zurück in den Vorrat).
4. Startspieler im Uhrzeigersinn weitergeben.
5. Neue Runde beginnen.

---

## 14) Spielende

Sobald ein Spieler **8 Camp-Punkte** erreicht:

* endet das Spiel sofort,
* dieser Spieler gewinnt.

---

## 15) Kartendesign – Leitlinien

**Icon-Legende:**

* ⚡ Push: Overload hoch, +1 Live, +1 Pool
* 🛠️ Stabilisieren: Overload runter
* 🌀 Twist: Chaos (Sofort oder Bühnenregel 🌀∞)
* 🎤 Encore: Ketten-Event

**Festival-UX:**

* Maximal **1–2 Textzeilen pro Karte**.
* Dauerhafte Effekte immer als **offene Bühnenregel**.
* Keine Effekte, die gezählt oder gemerkt werden müssen.

---

## 16) Test-Deckliste (Startpunkt, 60 Karten)

**Push (⚡) – 26**

* Soundcheck ×10 – ⚡ Overload +1
* Crowd Surf ×10 – ⚡ Overload +2
* Bassdrop ×6 – ⚡ Overload +3

**Stabilisieren (🛠️) – 14**

* Atem holen ×8 – 🛠️ Overload −2
* Security greift ein ×6 – 🛠️ Overload −3

**Twist (🌀) – 14**

* Richtungswechsel ×2 – 🌀 Drehe die Aufdeck-Reihenfolge um
* Feedback ×4 – 🌀∞ Bis Rundenende: Jeder ⚡ gibt zusätzlich +1 Overload
* Pyro ×3 – 🌀 Overload +2
* Stage Dive ×3 – 🌀 Wähle einen aktiven Spieler: Er zahlt 1 Live oder bleibt beim nächsten Camp automatisch drin. Ist er bereits betroffen, greift ein Ersatz-Effekt (Overload +1, cap 12).
* Setwechsel ×2 – 🌀 Der nächste Event wird vom gleichen Spieler aufgedeckt

**Encore! (🎤) – 6**

* Encore! ×6 – 🎤 Ketten-Event (1 Live zahlen, um zu stoppen)

---

## 17) Spielerzahl-Tuning

* **3 Spieler**: Siegziel optional **7 Camp**.
* **7–8 Spieler**:
  * Overload-Max optional **10 statt 12**, oder
  * Countdown steigt um **+2** pro Event.

---

## 18) Erweiterungsregeln (Skalierung)

**Do:**

* Neue Karten klar einem Typ zuordnen (⚡ / 🛠️ / 🌀 / 🎤).
* Dauerhafte Effekte immer als Bühnenregel.

**Don’t:**

* Keine Handkarten-Mechaniken.
* Keine „Du darfst nie campen“-Locks ohne Bezahl-Ausweg.
* Keine Effekte, die im Kopf mitgezählt werden müssen.

---

## 19) Changelog

Diese Version ersetzt frühere Verwaltungsmechaniken vollständig durch:

* simultanes **Bleib / Camp**
* sichtbaren **Bühnen-Pool**
* **Encore-Ketten**
* Overload-Check bei 12 mit Rückstoß auf 10
* Countdown nach erstem Camper
