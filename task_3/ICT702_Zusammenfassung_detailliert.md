# ICT702 Data Visualisation – Ausführliche Zusammenfassung (Module 2–10)

Prüfungsvorbereitung Task 3 · Basis: Lehrbuch Camm, Cochran, Fry & Ohlmann (2021) *Data Visualization – Exploring and Explaining with Data*, Folien, Canvas-Seiten und Workshop-Activities

> **Hinweis zur Nummerierung:** Die Canvas-Module heißen **Module 2–10**, die Foliensätze sind aber **Module 1–9** nummeriert (immer um eins versetzt). In dieser Zusammenfassung gilt die **Canvas-Nummerierung** (= Ordnernamen, = Nummern der Workshop-Activities).
>
> **Sprache:** Erklärungen auf Deutsch, Fachbegriffe auf Englisch. Die **Antwort-Skizzen (EN)** sind bewusst auf Englisch, weil die Prüfung auf Englisch beantwortet wird. Nicht kopieren (ist ja Papier), sondern in eigenen Worten tippen.

---

## Inhaltsverzeichnis

0. Prüfungsinfos & Strategie
1. Modul 2 – Introducing Data Visualisation
2. Modul 3 – Selecting a Chart Type
3. Modul 4 – Data Visualisation and Design
4. Modul 5 – Purposeful Use of Colour
5. Modul 6 – Visualising Variability
6. Modul 7 – Exploring Data Visually
7. Modul 8 – Explaining Visually to Influence with Data
8. Modul 9 – Data Dashboards
9. Modul 10 – Telling the Truth with Data Visualisation
10. Anhang A – Excel-Anleitungen (inkl. Mac-Hinweise)
11. Anhang B – Formeln & Excel-Funktionen
12. Anhang C – Antwort-Frameworks für Essay-Fragen
13. Anhang D – Glossar EN → DE

---

## 0. Prüfungsinfos & Strategie

### Rahmenbedingungen
- **Gewichtung:** 40 % der Gesamtnote · Canvas-Prüfung im Week-12-Workshop (Start 15 Min. nach Workshopbeginn)
- **Dauer:** 90 Minuten, automatische Abgabe danach
- **5 Fragen** (Short Essay oder File Upload), aus Fragenpools zufällig gezogen
- **Punkte laut deinen Notizen:** Q1 = 4 · Q2 = 8 · Q3 = 10 · Q4 = 12 · Q5 = 6 → **40 Punkte**
- **Kein Zurückspringen** → jede Frage vollständig beantworten (inkl. Datei-Upload!), bevor du weitergehst
- **Erlaubt:** Papiernotizen (getippt/ausgedruckt oder handschriftlich). **Nicht erlaubt:** digitale Ressourcen, Handy, GenAI
- **Kein Copy & Paste** aus irgendeiner Quelle → 0 Punkte für die Antwort
- Ausweis (Student ID) mitbringen, Passwort für den Login bekommst du im Workshop
- Inhalt: **Module 2–10** (Power-Platform/PL-900 ist **nicht** prüfungsrelevant)
- Tipp der Dozentin: **Alle Workshop-Activities wiederholen**, die Prüfungsfragen sind ähnlich (z. B. Activity 1 oder 2 aus Modul 10, „create a scatter chart and trendline")

### Zeitplan (≈ 2,2 Min. pro Punkt)

| Frage | Punkte | Zeitbudget | Uhrzeit (Start 12:15) |
|---|---|---|---|
| Q1 | 4 | ~8 Min. | bis ~12:23 |
| Q2 | 8 | ~17 Min. | bis ~12:40 |
| Q3 | 10 | ~22 Min. | bis ~13:02 |
| Q4 | 12 | ~26 Min. | bis ~13:28 |
| Q5 | 6 | ~13 Min. | bis ~13:41 |
| Puffer | – | ~4 Min. | Ende 13:45 |

### Strategie
- **Punkte = Anzahl der erwarteten Argumente.** 4 Punkte → mind. 4 klare Aussagen; 12 Punkte → Definition + mehrere begründete Punkte + Beispiel/Bezug auf die Daten.
- **Struktur jeder Antwort:** (1) direkte Antwort, (2) Begründung mit Fachbegriff, (3) konkreter Bezug auf das Beispiel / die Daten, (4) ggf. Verbesserungsvorschlag.
- **Datei-Fragen:** Datei herunterladen → bearbeiten → **speichern als .xlsx** → **umbenennen** (z. B. `Nachname_StudentID_Q3.xlsx`) → hochladen → prüfen, dass der Upload angekommen ist → erst dann weiter. Bei Datei-Fragen fast immer auch eine kurze **Interpretation** im Textfeld schreiben, wenn danach gefragt wird.
- Bei technischen Problemen **Screenshot mit sichtbarer Uhrzeit** machen.

<div style="page-break-after: always;"></div>

## 1. Modul 2 – Introducing Data Visualisation

### 1.1 Analytics
- **Analytics** = wissenschaftlicher Prozess, Daten in **Insights für bessere Entscheidungen** zu verwandeln (Muster entdecken, interpretieren, kommunizieren).
- **Gründe für das starke Wachstum von Analytics:** technologische Entwicklungen, methodische Entwicklungen, enorm gestiegene Rechenleistung und Speicherkapazität.

| Typ | Frage | Beispiele |
|---|---|---|
| **Descriptive** | Was ist passiert? | Data queries, Standard-Reports, deskriptive Statistik, **Data Visualisation**, Dashboards, Cluster-Analyse, What-if-Spreadsheet-Modelle |
| **Diagnostic** | Warum ist es passiert? | Ursachenanalyse, Drill-down (nur Canvas-Seite, nicht in den Folien) |
| **Predictive** | Was wird passieren? | Lineare Regression, Time-Series-Analyse, Predictive Data Mining, Forecasts |
| **Prescriptive** | Was sollen wir tun? | Optimierung, Simulation, Decision Analysis |

- **Data Visualisation gehört zu Descriptive Analytics**, wird aber auch genutzt, um Ergebnisse von predictive/prescriptive Modellen zu erklären.
- Beispiel Wetter-App: Die Vorhersage ist **predictive**. Wenn sie eine Handlungsempfehlung gibt („Regenschirm mitnehmen"), wäre das **prescriptive**.

### 1.2 Warum visualisieren?
1. **Exploring data**: Muster (z. B. Saisonalität bei der Zoo-Attendance) und Beziehungen zwischen Variablen erkennen
2. **Explaining / Communicating**: Erkenntnisse und Modellergebnisse einem Publikum vermitteln
- **Anscombe's Quartet:** Datensätze mit identischer Regressionsgleichung (y = 0,5x + 3) und R² = 0,67 sehen grafisch völlig verschieden aus. Daraus folgt: **immer visualisieren, nie nur Kennzahlen betrachten.**

### 1.3 Datentypen

| Begriff | Bedeutung | Beispiel |
|---|---|---|
| **Quantitative data** | Zahlen geben eine **Größe/Magnitude** an, Rechenoperationen möglich | Preis, Volumen, Umsatz |
| **Categorical data** | **Labels/Namen** für Gruppen, keine Rechenoperationen | Firma, Branche, Symbol |
| **Cross-sectional data** | Mehrere Einheiten zum **gleichen Zeitpunkt** | Hauspreise von 75 Häusern am 03.01.2021 |
| **Time series data** | Beobachtungen über **mehrere Zeitpunkte** (meist regelmäßig) | Dow Jones 2010–2020, Netflix-Abonnenten pro Jahr |

- Achtung: **Zahlen können kategorial sein** (z. B. Postleitzahl, Jahr als Label, Rating 1–4 = ordinal).
- **Big Data**: Daten, die zu groß/komplex für einen Desktop-Computer bzw. Standardverfahren sind. **Die 4 V's:**
  - **Volume** – Datenmenge
  - **Velocity** – Geschwindigkeit der Datenentstehung
  - **Variety** – Vielfalt von Typen und Strukturen
  - **Veracity** – Verlässlichkeit/Qualität der Daten
- **Word Cloud**: häufiges Diagramm zur Zusammenfassung großer Textmengen.

### 1.4 Visualisierungen nach Funktionsbereich (Beispiele aus den Folien)

| Bereich | Chart | Zweck |
|---|---|---|
| Accounting | Clustered column: **Benford's Law** vs. Ist-Daten | Betrugserkennung (First-Digit Law) |
| Finance | **High-low-close stock chart** | Schlusskurs-Verlauf + tägliche Volatilität |
| HR | **Stacked column** (Zu-/Abgänge pro Monat) | Part-to-whole über die Zeit |
| Marketing | **Funnel chart** | Konversion von groß nach klein (Website-Besucher → Käufer) |
| Operations | **Line chart** | Trend, wiederkehrende Muster, Forecast |
| Engineering | **Control chart** (mit Upper/Lower Control Limits) | Ist der Prozess „in control"? |
| Science | **Spaghetti chart** auf Karte | Viele mögliche Pfade (z. B. Hurrikan-Modelle) |
| Sports | **Shot chart** | Wurfpositionen; Symbol/Farbe = Treffer/Fehlwurf |

### 1.5 Benford's Law (First-Digit Law)
- Erwarteter Anteil der ersten Ziffer in vielen realen Datensätzen:

| Ziffer | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |
|---|---|---|---|---|---|---|---|---|---|
| Benford | 30,1 % | 17,6 % | 12,5 % | 9,7 % | 7,9 % | 6,7 % | 5,8 % | 5,1 % | 4,6 % |

- Weichen die Daten deutlich ab, sollte man **Betrug untersuchen** (ist aber kein Beweis).

### 1.6 Cognitive Load & Chart-Überarbeitung (Zoo-Beispiel)
- **Cognitive load** = mentaler Aufwand, um eine Visualisierung zu verstehen. Ziel: so gering wie möglich.
- Typische Verbesserungen des Excel-Standarddiagramms (Activity 5): Gridlines entfernen, aussagekräftigen Titel linksbündig über der y-Achse, Achsentitel hinzufügen (y-Achsentitel **horizontal** über der Achse), Achsenlinien schwarz, Tick marks „Inside", einheitliche Schrift (Calibri 10,5 / Titel 16), Chart-Rahmen entfernen.

### 1.7 Workshop-Activities Modul 2 – Lösungen

**Activity 1 – Types of Analytics**
1. Data dashboard → **descriptive**
2. Modell, das den Produktionsplan mit minimalen Überstunden findet → **prescriptive** (Optimierung)
3. Modell, das den Umsatz des nächsten Quartals vorhersagt → **predictive**
4. Bar chart → **descriptive**
5. Modell, das Investments so verteilt, dass ein finanzielles Ziel erreicht wird → **prescriptive**

**Activity 2 – House Price & Square Footage (75 Häuser, 03.01.2021)**
1. **Quantitative** (Preis und Fläche sind Messwerte)
2. **Cross-sectional** (ein Zeitpunkt, viele Häuser)
3. **Scatter chart**, weil die Beziehung zwischen zwei quantitativen Variablen gezeigt werden soll; jeder Punkt = ein Haus. Bar-/Column-Charts vergleichen Kategorien und sind hier ungeeignet.

**Activity 3 – Netflix Subscribers 2010–2019**
1. **Quantitative** (Anzahl der Abonnenten in Mio.)
2. **Time series** (jährliche Werte)
3. **Column chart** mit Data Labels (Alternative für Trend: Line chart)

**Activity 6 – Benford vs. Tucker Software (aus dem Diagramm abgelesen)**

| Ziffer | Benford | Tucker (ca.) | Abweichung |
|---|---|---|---|
| 1 | 0,301 | 0,255 | −0,046 (≈ −15 %) → **unterrepräsentiert, größte absolute Abweichung** |
| 3 | 0,125 | 0,100 | −0,025 (≈ −20 %) |
| 4 | 0,097 | 0,080 | −0,017 (≈ −18 %) |
| 5 | 0,079 | 0,150 | **+0,071 (≈ fast doppelt)** → überrepräsentiert |
| 7 | 0,058 | 0,040 | −0,018 (≈ **−31 %, größte relative Abweichung**) |
| 9 | 0,046 | 0,100 | **+0,054 (≈ doppelt)** → überrepräsentiert |

- **Antwort-Skizze (EN):** *"The data do not fully conform to Benford's Law. Digits 5 and 9 are clearly over-represented (roughly double the expected probability), while digit 1 is under-represented by the largest absolute amount (about 4.6 percentage points) and digit 7 by the largest relative amount (about 30 % below expectation). These deviations do not prove fraud but warrant further investigation of the accounts payable entries."*

### 1.8 Mögliche Prüfungsfragen Modul 2
- Ordne Beispiele den Analytics-Typen zu (descriptive/predictive/prescriptive) und begründe.
- Bestimme für einen Datensatz: quantitative/categorical **und** cross-sectional/time series; empfiehl einen Chart-Typ mit Begründung.
- Erkläre die 4 V's von Big Data.
- Erkläre die zwei Gründe, warum man Daten visualisiert (explore vs. explain); Anscombe als Beispiel.
- Interpretiere ein Benford-Diagramm (über-/unterrepräsentierte Ziffern, absolute vs. relative Abweichung).
- **Datei:** Erstelle aus Zoo-Daten ein Column Chart und verbessere es (Declutter-Schritte).

<div style="page-break-after: always;"></div>

## 2. Modul 3 – Selecting a Chart Type

### 2.1 Ziel der Visualisierung definieren
- Vor der Chart-Wahl: **Daten kennen, Publikum kennen, Chart-Typen kennen.**
- Kommunizieren → Wahl hängt von der **Botschaft** ab. Explorieren → Wahl hängt von der **Fragestellung** ab. Zusätzlich spielt der **Datentyp** eine Rolle.
- **Vier typische Ziele:**
  - **Composition** – Woraus besteht das Ganze? (Bestandteile)
  - **Ranking / Comparison** – Wie ist die Reihenfolge? (Ordnung)
  - **Relationship** – Wie hängen zwei Variablen zusammen? (Muster)
  - **Distribution** – Wie sind die Werte verteilt? (Streuung)

### 2.2 Guidelines for Selecting a Chart (Folie, wichtig!)

| Chart | Relationship | Distribution | Composition | Ranking |
|---|:-:|:-:|:-:|:-:|
| Scatter | ✓ | ✓ | | |
| Bubble | ✓ | ✓ | | |
| Line | ✓ | | | |
| Stock | ✓ | | | |
| Column | ✓ | ✓ | | ✓ |
| Bar | ✓ | ✓ | ✓ | ✓ |
| Heat map | ✓ | | | |
| Choropleth map | | ✓ | | |
| Stacked bar | | | ✓ | |
| Stacked column | | | ✓ | |
| Treemap | | | ✓ | |
| Waterfall | | | ✓ | |
| Funnel | | | | ✓ |

(Canvas-Quiz-Variante: Scatter = Relationship + Distribution · Bubble = Relationship · Histogram = Distribution · Stacked column/area = Composition + Comparison · Pie/Waterfall = Composition · Table/Line/Spider/Column = Comparison)

### 2.3 Chart-Typen im Detail
- **Column chart**: Vergleich von Kategorien, Verteilung über diskrete Kategorien oder Zeitperioden. Für Zeit besser als Bar (Zeit läuft natürlich von links nach rechts).
- **Bar chart**: wie Column, aber horizontal. Besser bei **langen Kategorienamen**. **Sortiert** gut für Rankings.
- **Clustered column/bar**: mehrere Serien nebeneinander. Wird bei vielen Serien schnell unübersichtlich.
- **Stacked column/bar**: **Part-to-whole**; die Gesamthöhe zeigt die Summe (z. B. Ost + West = Total Sales).
- **Line chart**: Zeitreihen. Verbundene Punkte suggerieren **Kontinuität** und zeigen Trends/Veränderungen. Multiple-line chart zum Vergleich mehrerer Serien (oft weniger überladen als clustered column).
- **Scatter chart**: Beziehung zwischen **zwei quantitativen Variablen**; jeder Punkt = ein Paar von Messwerten (z. B. Tiefsttemperatur vs. Schneefall in 51 US-Städten). „Among the most useful charts for exploring pairs of quantitative data."
- **Bubble chart**: Scatter + **dritte quantitative Variable als Blasengröße** (Airports: x = Wartezeit TSA, y = günstigster Parkpreis, Größe = Passagiere). Schwäche: Größen werden schlecht geschätzt.
- **Choropleth map**: Werte (quantitativ oder kategorial) über geografische Flächen eingefärbt (z. B. Bevölkerung pro Bundesstaat, Amazon-Fulfillment-Center ja/nein).
- **Heat map**: 2D-Tabelle, in der **Farbschattierungen die Magnitude** zeigen; gut für Muster zwischen Kategorien.
- **Treemap**: **hierarchische** Daten. Rechteckgröße = Wert, Farbe = übergeordnete Kategorie (z. B. Branche → Marke → Markenwert).
- **Waterfall chart**: kumulativer Effekt positiver und negativer Veränderungen (Composition über Zeit/Kategorien, z. B. Gross Profit pro Monat → Total).
- **Stock chart (High-Low-Close)**: Höchst-, Tiefst- und Schlusskurs pro Tag.
- **Funnel chart**: Fortschritt von großen zu kleinen Werten über Stufen (Bewerber → Eingestellte). Kann auch Composition (Drill-down) zeigen.
- **Tables** statt Charts, wenn:
  - genaue Zahlenwerte benötigt werden
  - präzise Vergleiche zwischen Werten nötig sind
  - Werte unterschiedliche Einheiten oder sehr unterschiedliche Größenordnungen haben
- **Table + Chart kombiniert** (z. B. Line chart mit Datentabelle darunter) ist ebenfalls möglich.

### 2.4 Charts, die man vermeiden sollte (+ Alternative)

| Vermeiden | Warum | Besser |
|---|---|---|
| **Pie chart** (bei mehr als wenigen Kategorien) | Menschen schätzen **Länge** besser als **Winkel/Fläche**; viele Farben erhöhen den Cognitive Load; Labels/Legende → Eye travel | (sortiertes) **Bar chart** |
| **Radar/Spider chart** | schwer zu interpretieren | **Clustered column chart** |
| **Area chart** (vor allem simple/stacked) | überladen, verdeckte Flächen, schwer lesbar | **(Multiple) line chart** |
| **Combo / dual-axis chart** | überladen, verleitet zu falschen Vergleichen | **zwei separate Charts** |
| **3D charts** | dritte Dimension = Clutter, verzerrt Proportionen | **2D-Version** |

### 2.5 Excel-Besonderheiten
- Excel nimmt meist die **linke Spalte als horizontale Achse**; Zuordnung lässt sich tauschen („Switch Row/Column").
- **Problem „Jahr als Zahl":** Wählt man Year + Sales aus, plottet Excel das Jahr als eigene Datenreihe. **Lösung:** Rechtsklick → *Change Chart Type* → Variante mit einer Serie wählen (oder Year als Text/Achsenbeschriftung über *Select Data → Horizontal (Category) Axis Labels* setzen).
- Line chart aus Zahlen-x-Werten: *Insert → Scatter → Scatter with Straight Lines and Markers*.
- **Recommended Charts**-Tool: liefert Vorschläge, ersetzt aber nicht das eigene Urteil.

### 2.6 Workshop-Activities Modul 3 – Lösungen

**Activity 1 – Cheetah Sports (Column, Clustered, Stacked)**
- *Warum ist das stacked column chart besser als clustered?* Es zeigt **gleichzeitig den Beitrag jeder Region und den Gesamtumsatz** (Gesamthöhe der Säule). Man sieht also Composition und Total Sales über die Zeit, mit nur einer Säule pro Jahr und weniger Clutter.
- *Zwei Beispiele, wann das Publikum lieber welches Chart sieht:*
  - **Line chart**: Regionalmanager wollen die **Entwicklung/Trends beider Regionen direkt vergleichen** (z. B. West wächst in den letzten drei Jahren, Ost fällt seit Jahr 7). Line chart zeigt Trendrichtung und Wendepunkte klar.
  - **Stacked column chart**: Geschäftsführung interessiert sich für den **Gesamtumsatz pro Jahr und wie viel jede Region dazu beiträgt** (Part-to-whole).

**Activity 2 – Line Chart (Cheetah)** → Scatter with Straight Lines and Markers; Linien suggerieren Kontinuität.

**Activity 3 – New York City Budget**
1. Zwei Gründe für Bar statt Pie:
   - Menschen vergleichen **Längen** genauer als **Winkel/Flächen** (preattentive attribute length).
   - Viele Kategorien brauchen beim Pie viele Farben + Legende → höherer **Cognitive Load** und Eye travel. Beim Bar chart kann man **sortieren** und direkt beschriften.
2. Bar statt Column: Die **langen Kategorienamen** (Budgetposten) sind horizontal gut lesbar. Ein sortiertes horizontales Ranking ist leicht von oben nach unten zu lesen.

**Activity 4 – Anscombe & Trendlinien**
- Gleiche Regressionsgleichung (y = 0,5x + 3) und R² = 0,67, aber: **Datensatz 1** streut zufällig um eine Gerade → lineare Trendlinie sinnvoll. **Datensatz 2** zeigt einen klar **gekrümmten (nichtlinearen) Verlauf** → lineare Trendlinie unpassend, ein Polynom (2. Ordnung) passt.
- **Antwort-Skizze (EN):** *"Identical summary statistics can hide very different patterns. A linear fit is appropriate for data set 1, but data set 2 follows a curved pattern, so a straight line misrepresents the relationship. This is why data should always be visualised before fitting a model."*

### 2.7 Mögliche Prüfungsfragen Modul 3
- Welches Chart für Ziel X (composition/ranking/relationship/distribution) und Datentyp Y? Begründen.
- Warum Bar statt Pie (2–3 Gründe)? Warum Bar statt Column?
- Welche Charts sollte man vermeiden, warum, und was ist die Alternative?
- Clustered vs. stacked column vs. multiple line: Wann welches?
- Wann Tabelle statt Chart?
- **Datei:** Column/clustered/stacked column chart aus CheetahRegion; Jahr-als-Zahl-Problem lösen; Data Labels hinzufügen.
- **Datei:** Scatter chart + Trendline erstellen und beurteilen, ob linear passt.

<div style="page-break-after: always;"></div>

## 3. Modul 4 – Data Visualisation and Design

### 3.1 Visual Perception & Preattentive Attributes
- **Visual perception**: Prozess im Gehirn, der das ins Auge fallende Licht interpretiert. Drei Gedächtnisformen beeinflussen ihn: **iconic memory**, **short-term memory**, **long-term memory**.
- **Preattentive attributes** = Merkmale, die vom **iconic memory** verarbeitet werden, also **ohne bewusste Anstrengung** in Sekundenbruchteilen erkannt.
- **Cognitive load** = Aufwand, Informationen korrekt und effizient zu verarbeiten. Richtiger Einsatz von preattentive attributes **senkt** ihn.

| Kategorie | Attribute | Hinweise |
|---|---|---|
| **Colour** | Hue, Saturation, Luminance | Hervorhebung, Gruppierung |
| **Form** | Orientation, Size, Shape, Length, Width | Orientation: Steigung in Line charts. **Size wird schlecht geschätzt.** Length: Bar/Column. Width: Sankey chart (Linienbreite = Flussmenge) |
| **Spatial positioning** | Position im 2D-Raum | z. B. Punkte im Scatter chart |
| **Movement** | Flicker (Blinken), Motion (gerichtete Bewegung) | In statischen Charts meist nicht möglich |

- Kombination von Attributen (z. B. Farbe × Form) erzeugt mehr Gruppen (3 Farben × 3 Formen = 9 Gruppen), aber auch mehr Cognitive Load.
- **Überbenutzung** von preattentive attributes → Clutter: „Wenn alles hervorgehoben ist, ist nichts hervorgehoben."

### 3.2 Gestalt Principles
Wie Menschen Ordnung und Bedeutung in das Gesehene bringen. Die **vier Hauptprinzipien für Data Vis:**

| Prinzip | Bedeutung | Anwendung |
|---|---|---|
| **Similarity** | Gleiche Merkmale (Farbe, Form) → gleiche Gruppe | Gleiche Farbe für dieselbe Kategorie in allen Charts |
| **Proximity** | Nahe beieinander → gehört zusammen | Labels direkt neben die Datenreihe; Abstände zwischen Gruppen |
| **Enclosure** | Gemeinsam eingerahmt/schattiert → gehört zusammen | Schattierte Fläche für Prognosezeitraum, Rahmen um eine Gruppe im Scatter |
| **Connection** | Verbundene Objekte → gehören zusammen | Linien in Zeitreihen; gestrichelte Linie für Forecast vs. durchgezogen für Ist |

(Weitere aus dem Canvas-Quiz: **Closure, Continuation, Symmetry, Good Figure/Prägnanz**.)

### 3.3 Data-Ink Ratio & Decluttering
- **Data-ink ratio** = Anteil der „Tinte", die tatsächlich Daten darstellt, an der gesamten Tinte eines Charts/einer Tabelle (Konzept von Edward Tufte).
  - **Data-ink**: notwendig, um die Bedeutung der Daten zu vermitteln
  - **Non-data-ink**: erfüllt keinen Zweck (z. B. dicke Gridlines, Rahmen, 3D-Effekte, Hintergrundfarben, redundante Legenden, Logos)
- **Decluttering** = Data-ink ratio erhöhen. **White space** hat den gleichen Effekt.
- **Typische Declutter-Schritte:** Gridlines entfernen/aufhellen, Rahmen entfernen, Legende entfernen (bei einer Serie) bzw. durch direkte Labels ersetzen, Hintergrundfarbe entfernen, unnötige Dezimalstellen entfernen, 3D entfernen, Achsen dezent, Data Labels statt Achse (wenn wenige Werte).
- **Tabellen-Regeln:**
  - Zahlen **rechtsbündig**, Text **linksbündig**
  - In einer Spalte überall **gleich viele Dezimalstellen**, aber nur so viele wie nötig
  - Große Zahlen runden (Tausend, Million)
  - Wenig Linien, viel White space

### 3.4 Minimizing Eye Travel
Cognitive Load wird gesenkt durch: preattentive attributes, Gestalt-Prinzipien, höhere Data-ink ratio und **minimale Augenbewegung**:
- Chart-Titel und y-Achsentitel **linksbündig an der y-Achse** ausrichten
- **Line labels direkt rechts neben die Linien** setzen (statt Legende)
- x-Achsenbeschriftung am Ende der Achse, auf Höhe der Line labels

### 3.5 Schrift
- **Sans-serif** (Arial, Calibri, Verdana, Myriad Pro) → **bevorzugt für Data Vis**, auch klein gut lesbar
- **Serif** (Times New Roman, Courier) → für gedruckten Fließtext; hat Endstriche, ist klein schlechter lesbar
- **Konsistent und zurückhaltend:** möglichst **eine** Schriftart; x- und y-Achsentitel gleiche Schrift und Größe. Größe, **bold**, *italic* und Farbe gezielt zur Hervorhebung einsetzen.

### 3.6 Häufige Design-Fehler
1. **Falscher Chart-Typ** (z. B. Clustered column statt Line chart für Zeitvergleich)
2. **Zu viel Information** auf einem Chart (z. B. OEM + Aftermarket für viele Regionen). **Lösung:** stacked clustered column oder **separate Charts**
3. **Excel-Standardeinstellungen** unverändert übernehmen
4. **Zu viele Attribute** (Farbe + Form + Größe gleichzeitig)
5. **Unnötiges 3D**
6. Logos/Bilder statt Säulen (Fast-Food-Makeover): verzerrt die Wahrnehmung

### 3.7 Workshop-Activities Modul 4 – Lösungen

**Activity 1 – Aussagen diskutieren**
- *Preattentive attributes lenken die Aufmerksamkeit:* richtig. Eine Kontrastfarbe für den wichtigsten Balken lenkt den Blick sofort dorthin.
- *Überbenutzung führt zu Clutter:* richtig. Viele Farben/Formen/Größen konkurrieren um Aufmerksamkeit, nichts sticht mehr hervor, der Cognitive Load steigt.

**Activity 2 – Siebener in einer 16×10-Zahlenmatrix zählen** (neben Hue und Size)
- **Shape/Form:** 7er in anderer Schriftart oder als anderes Symbol
- **Orientation:** 7er schräg/gedreht darstellen
- **Width:** 7er **fett** (dickere Strichstärke)
- **Enclosure:** Kasten/Kreis um jede 7 (Gestalt) oder **Hintergrundschattierung** der Zelle
- **Luminance/Saturation:** alle anderen Ziffern hellgrau, 7er schwarz
- **Spatial positioning:** 7er leicht versetzt (höher/tiefer)
- **Movement (digital):** 7er blinken lassen (flicker)

**Activity 3 – Scarf Sales: Data-ink ratio erhöhen**
1. *Entfernen:* Gridlines, Legende (nur eine Serie), Chart-Rahmen, ggf. unnötige Dezimalstellen/Achsenlinie, Standardtitel „Chart Title".
2. *Hinzufügen für Lesbarkeit:* aussagekräftigen Titel (linksbündig), Achsentitel (y-Titel horizontal oben an der Achse), passende Achsenskalierung/Einheiten, ggf. Data Labels für Schlüsselpunkte, einheitliche Schrift.

**Activity 4 – Scatter chart Snow (51 Städte)**
- Je **höher die durchschnittliche Tiefsttemperatur**, desto **weniger Schneefall** (negativer, **nichtlinearer** Zusammenhang). Für warme Städte geht der Schneefall gegen **null und flacht ab**, in kalten Städten ist die Streuung groß.

**Activity 5 – Bubble chart Airports**
- Schlussfolgerungen formulieren: Gibt es einen Zusammenhang zwischen Wartezeit (x) und Parkpreis (y)? Haben große Flughäfen (große Blasen) höhere Parkpreise/Wartezeiten? Welche Ausreißer gibt es?
- Achsen tauschen über *Select Data → Edit*: Series X values / Y values / bubble size neu zuordnen. Dann beurteilen, ob die neue Zuordnung die wichtigste Beziehung besser zeigt (am besten kommen die zwei Variablen mit der wichtigsten Beziehung auf die Achsen, weil Bubble-Größen schwer zu vergleichen sind).

**Activity 6 – NYC: % College Graduates vs. Median Monthly Rent**
1. Preattentive attribute: **spatial positioning** (2D-Position der Punkte)
2. **Positiver Zusammenhang:** Sub-Boroughs mit höherem Anteil an College-Absolventen haben tendenziell höhere Medianmieten. Korrelation ≠ Kausalität (z. B. Einkommen als Lurking variable).

### 3.8 Mögliche Prüfungsfragen Modul 4
- Definiere preattentive attributes und nenne die 4 Kategorien mit Beispielen.
- Nenne/erkläre die 4 Gestalt-Prinzipien mit je einem Anwendungsbeispiel in einem Chart.
- Was ist die Data-ink ratio? Wie erhöht man sie (Liste von Schritten)?
- Wie minimiert man Eye travel?
- Serif vs. sans-serif, welche für Data Vis und warum?
- Gegebenes Chart kritisieren: Was ist schlecht, wie verbessern?
- **Datei:** Default-Chart entrümpeln (Scarf Sales), Scatter (Snow) oder Bubble chart (Airport) erstellen und interpretieren.

<div style="page-break-after: always;"></div>

## 4. Modul 5 – Purposeful Use of Colour

### 4.1 Die drei Attribute von Farbe
- **Colour** = Eigenschaft eines Objekts, die daraus entsteht, wie es Licht reflektiert oder aussendet.

| Attribut | Bedeutung | Extreme |
|---|---|---|
| **Hue** (Farbton) | „Basis" der Farbe, Position im Lichtspektrum. Primary hues (Folie: **RGB = Red, Green, Blue**; Canvas-Text: Red, Yellow, Blue) lassen sich nicht mischen; Kombinationen ergeben secondary/tertiary colours (Farbkreis) | – |
| **Saturation** (Sättigung) | Anteil **Grau**, also Intensität/Reinheit | 100 % = reiner Farbton · 0 % = Grau |
| **Luminance** (Helligkeit) | Anteil **Schwarz vs. Weiß** | 100 % = Weiß · 0 % = Schwarz; erzeugt Kontrast und **Hierarchie** |

### 4.2 Colour Psychology vs. Colour Symbolism
- **Colour psychology**: **angeborene** Beziehung zwischen Farbe und Verhalten (eher universell)
  - **Cool hues** (Lila, Blau, Grün) → beruhigend, vertrauensvoll; wirken **weiter entfernt**
  - **Warm hues** (Gelb, Orange, Rot) → Energie, Leidenschaft, Gefahr
- **Colour symbolism**: **kulturelle** Bedeutung (z. B. Weiß = Trauer in Teilen Asiens). Variiert stärker zwischen Kulturen und **ändert sich über die Zeit**.
- **Perceived colour**: Farbe wird **relativ zur Umgebung/zum Hintergrund** wahrgenommen (gleiche Farbe wirkt auf verschiedenen Hintergründen unterschiedlich).
- **Complementary colours** (gegenüber im Farbkreis) → **Dissonanz**, starker Kontrast, gut zum Hervorheben; Überbenutzung lenkt ab.
- **Analogous colours** (benachbart im Farbkreis) → weich, harmonisch, weniger Kontrast.
- Bunte Hintergründe lenken ab.

### 4.3 Colour Schemes (je nach Datentyp)

| Scheme | Datentyp | Aufbau | Beispiel |
|---|---|---|---|
| **Categorical** | Kategorial, **ohne Ordnung** | Unterschiedliche, gut unterscheidbare Hues; **max. ca. 6 Farben** | Branchen im Treemap |
| **Sequential** | Geordnet / quantitativ (aufsteigend) | **Ein Hue**, Gradient der **Luminance** (häufiger) oder Saturation; hell = niedrig, dunkel = hoch | Choropleth Bevölkerung, Durchschnittstemperatur (Braun = Wärme) |
| **Diverging** | Quantitativ **mit sinnvollem Referenzwert** (z. B. 0, Durchschnitt) | **Zwei** sequentielle Schemes mit **gemeinsamem Mittelpunkt**; zwei unterschiedliche Hues; Luminance zeigt Stärke der Abweichung | Heat map Same-store sales (Rot = Rückgang, Weiß = 0, Blau = Wachstum) |
| **Highlight** | Ein Element hervorheben | Alles grau, ein Element in Akzentfarbe | Eine Linie unter vielen |

### 4.4 HSL in Excel
- *Format → Fill → More Colors → Custom → Colour model HSL*
- Werte 0–255: **Hue** (Farbton, Regler links → rechts), **Sat** (0 = Grau, 255 = rein), **Lum** (0 = Schwarz, 255 = Weiß; **128 = reiner Farbton**)
- **Eyedropper** zum Übernehmen einer Farbe (z. B. Firmenlogo); **Transparency** 0–100 %. Alternativ RGB-Modell.

### 4.5 Häufige Fehler beim Einsatz von Farbe
1. **Unnecessary colour**: Farbe ohne Informationsgehalt (z. B. jede Säule anders gefärbt + Legende). **Lösung:** eine Farbe, Kategorien direkt an der Achse beschriften.
2. **Excessive colour**: zu viele Farben (51 Bundesstaaten = 51 Farben). **Lösung:** Fokusgruppe farbig, Rest **grau**, Legende durch direkte Labels ersetzen.
3. **Insufficient contrast**: Farben zu ähnlich. **Lösung:** Luminance-Unterschied vergrößern.
4. **Inconsistency across related charts**: gleiche Kategorie in verschiedenen Charts unterschiedlich gefärbt. **Lösung:** konsistente Farbcodierung (z. B. Erwachsene immer Orange, Kinder immer Blau).
5. **Neglecting colour-blindness**: am häufigsten **Rot-Grün-Schwäche** (Männer häufiger betroffen); auch Blau-Gelb; selten totale Farbenblindheit. **Lösung:** Rot-Grün vermeiden, Blau-Orange/Blau-Rot nutzen, zusätzlich Luminance-Unterschiede, Labels und Formen.
6. **Not considering mode of delivery**:
   - **Projektion:** dicke Linien, scharfe Konturen, hoher Kontrast, **hohe** Saturation und Luminance
   - **Druck:** weichere Konturen, **weniger** Saturation, niedrigere Luminance, weniger Kontrast
   - Farben variieren je nach Monitor/Beamer/Drucker → **vorher testen**

### 4.6 Workshop-Activities Modul 5 – Lösungen

**Activity 1 – Hue, Saturation oder Luminance?** (deine Lösungen)
a) **Saturation** · b) **Luminance** · c) **Luminance** · d) **Hue** · e) **Saturation** · f) **Luminance**
- Begründungslogik: Gleicher Farbton, aber einer „gräulich/stumpf" → Saturation. Gleicher Farbton, aber heller/dunkler → Luminance. Komplett anderer Farbton (Pink vs. Blau) → Hue.

**Activity 2 – Choropleth map StatePopulation**
- Dunkel = hohe Bevölkerung: **California, Texas, Florida, New York** am bevölkerungsreichsten. Dünn besiedelte Bundesstaaten (z. B. Wyoming, Alaska, Vermont) hell.
- Kritische Ergänzung: **absolute Zahlen** bevorzugen große Staaten; für faire Vergleiche **relative Werte** (z. B. Bevölkerungsdichte) nutzen (siehe Modul 10).

**Activity 3 – Farbschema wählen**
- *Median family income by state* → **Sequential colour scheme**: **ein Hue** (z. B. Grün oder Blau), **Luminance-Gradient**: hell = niedriges, dunkel = hohes Einkommen. Grund: geordnete quantitative Variable ohne natürlichen Mittelpunkt.
- *Veränderung des Einkommens 2010 vs. 2020* → **Diverging colour scheme**: **Referenzwert 0 % Veränderung** = Weiß/hellgrau. **Zwei Hues**, z. B. **Rot/Orange** für Rückgang und **Blau** für Anstieg; je dunkler (niedrigere Luminance), desto größer die Veränderung. Rot-Grün vermeiden (Farbenblindheit).

**Activity 4 – Heat map SameStoreSales** (Conditional Formatting → Color Scales → Blue-White-Red)
- Rot = Rückgang, Blau = Anstieg gegenüber Vorjahresmonat. Leicht erkennbar: z. B. **Austin** durchgehend stark positiv. **Phoenix/Seattle** starten positiv und werden im Jahresverlauf negativ. **Cincinnati/St. Louis** umgekehrt (negativ → positiv). **Albany** fast durchgehend negativ.
- Schwierigkeit: exakte Werte schwer ablesbar (Lösung: Zahlen in Zellen lassen). Feine Abstufungen sind schwer zu unterscheiden; Rot/Weiß/Blau ist aber farbenblind-freundlicher als Rot/Grün.

**Activity 5 – Treemap BrandValues** → zuerst nach Industry sortieren, dann *Insert → Hierarchy Chart → Treemap*; Werte über *Format Data Labels → Value*. Farbe = Branche, Rechteckgröße = Markenwert.

**Activity 6 – ManagementTop25 Treemap** (Sector → Company → Score; vorher nach Sector sortieren)
- Sektor mit den meisten Firmen: **Technology (12 von 25)**; höchster Score in Technology: **Amazon (120,2)** (nachgerechnet aus der Datei).

### 4.7 Mögliche Prüfungsfragen Modul 5
- Definiere Hue, Saturation, Luminance und unterscheide Farbpaare danach.
- Colour psychology vs. colour symbolism mit Beispielen.
- Welches Farbschema (categorical/sequential/diverging) für Szenario X? Hues und Luminance definieren!
- Nenne und erkläre häufige Farbfehler und wie man sie vermeidet (Farbenblindheit, Projektion vs. Druck …).
- Complementary vs. analogous colours.
- **Datei:** Choropleth (Filled Map), Heat map (Conditional Formatting), Treemap erstellen und interpretieren.

<div style="page-break-after: always;"></div>

## 5. Modul 6 – Visualising Variability

### 5.1 Grundbegriffe
- **Random variable**: Größe, deren Wert nicht mit Sicherheit bekannt ist
- **Variation**: Unterschied der Werte einer Variable über Beobachtungen (Zeit, Kunde, Produkt …) → erzeugt **Unsicherheit**
- **Sample**: Teilmenge der **Population**; wenn repräsentativ, kann man auf die Population schließen
- **Frequency distribution**: Welche Werte kommen wie oft vor?

### 5.2 Frequency Distribution – kategoriale Daten
- Daten in nicht überlappende **Bins/Classes** einteilen → Häufigkeit zählen (PivotTable oder `COUNTIF`)
- **Relative frequency** = Häufigkeit des Bins / n
- **Percent frequency** = Relative frequency × 100 → **schätzt die Wahrscheinlichkeitsverteilung** (probability distribution)
- Darstellung: Column/Bar chart, **sortiert** (größte zuerst). **Ausnahme: ordinale Daten** (z. B. Zufriedenheit 1–5) → natürliche Reihenfolge **beibehalten**!

### 5.3 Frequency Distribution – quantitative Daten (Histogram)
Drei Festlegungen:
1. **Anzahl nicht überlappender Bins**: **5–20** (abhängig von n). Zu wenige → Variation verschwimmt (zu aggregiert). Zu viele → keine generalisierbaren Muster.
2. **Bin width**: für alle Bins **gleich**; Näherung: **(größter Wert − kleinster Wert) / Anzahl Bins**
3. **Range spanned by bins**: erster Bin muss den kleinsten, letzter den größten Wert enthalten; **jeder Wert in genau einem Bin**
- **Notation (17, 25]**: runde Klammer = Wert **nicht** enthalten, eckige Klammer = Wert **enthalten**
- **Histogram** = Column chart **ohne Lücken**, Höhe = Häufigkeit; zeigt die **Form** der Verteilung
- **Kernel density chart**: geglättete Kurve der Verteilung

### 5.4 Skewness (Schiefe)
| Form | Erkennung | Lage-Maße | Beispiele |
|---|---|---|---|
| **Left-skewed (negativ)** | langer Schwanz nach **links** | **Mean < Median** | Sterbealter, Punkte in leichter Prüfung |
| **Symmetric** | glockenförmig | Mean ≈ Median | Körpergröße erwachsener Männer |
| **Right-skewed (positiv)** | langer Schwanz nach **rechts** | **Mean > Median** | Hauspreise, Einkommen, Lieferzeit |
- Im Box plot: **längerer Whisker / größerer Abstand Median–Quartil** auf der Seite des Schwanzes.

### 5.5 Verteilungen vergleichen
- **Frequency polygon**: wie Histogram, aber **Linien** verbinden die Bin-Häufigkeiten → mehrere Verteilungen übereinander vergleichbar (Excel: Line chart). Weniger Clutter als clustered columns.
- **Trellis display**: mehrere **gleich große Charts mit gleichen Skalen** nebeneinander/untereinander (Small multiples), z. B. Aufenthaltsdauer in 3 Krankenhäusern.
- **Strip chart**: jeder **Einzelwert** als Punkt auf einer Achse (z. B. Halbmarathon-Zeiten nach Geschlecht). Problem **Occlusion**: Punkte überdecken sich.
  - **Lösungen:** hohle Marker (No fill) und **Jittering** (zufälliger vertikaler Versatz, `=C2+RAND()`)
- **Box and whisker chart** (siehe 5.7), **Violin chart** = Box plot + gespiegelte Kernel-Density-Kurve.

### 5.6 Lage- und Streuungsmaße

| Maß | Definition | Excel | Hinweis |
|---|---|---|---|
| **Mean** | Summe / n | `AVERAGE` | von Ausreißern beeinflusst |
| **Median** | mittlerer Wert der sortierten Daten (bei geradem n: Mittel der zwei mittleren) | `MEDIAN` | robust, **bei Schiefe bevorzugen** |
| **Mode** | häufigster Wert (kann mehrere/keinen geben) | `MODE.SNGL` / `MODE.MULT` | bei wenigen diskreten Werten nützlich; im Histogram = höchste Säule |
| **Range** | Max − Min | `MAX` − `MIN` | nur 2 Werte, anfällig für Extreme |
| **Standard deviation (SD)** = Standardabweichung | durchschnittliche Abweichung vom Mean | `STDEV.S` | zuverlässig bei symmetrischen/glockenförmigen Daten; **nicht** bei Schiefe |
| **Percentile (p-th)** | Wert, der p % der Beobachtungen übersteigt | `PERCENTILE.EXC` | robust |
| **Quartiles** | Q1 = 25. · Q2 = 50. (= Median) · Q3 = 75. Perzentil | `QUARTILE.EXC` | teilen Daten in 4 Teile |
| **IQR** | **Q3 − Q1** (mittlere 50 %) | – | robust, keine Glockenform nötig |

- **Empirical rule** (glockenförmige, symmetrische Verteilung): ≈ **68 %** innerhalb ±1 SD, ≈ **95 %** innerhalb ±2 SD, ≈ **99,7 %** innerhalb ±3 SD.

### 5.7 Box and Whisker Chart
- **Box** von **Q1 bis Q3**, **Linie = Median**, **X = Mean**
- **Whiskers** bis zum kleinsten/größten Wert **innerhalb der Grenzen**
- **Outliers** (Punkte): Werte außerhalb **[Q1 − 1,5 × IQR ; Q3 + 1,5 × IQR]**
- Ideal zum **Vergleich mehrerer Verteilungen** (z. B. Hauspreise in 5 Vororten: Shadyside am höchsten, Hamilton am niedrigsten; Irving und Groton gleicher Median, Irving größere Streuung)

### 5.8 Uncertainty – Statistical Inference
- **Statistical inference**: Schlüsse über die Population aus einer Stichprobe. Es gibt immer **Sampling error**, deshalb Schätzungen als **Intervalle** zeigen (sonst überschätzt das Publikum die Genauigkeit).
- **Confidence interval (CI)** = Punktschätzung **± Margin of error**. Sagt, wie nah der Stichproben-Mittelwert/-Anteil am Populationswert liegen dürfte (üblich 95 % oder 99 %).
- **Margin of error (Mean)** hängt ab von:
  - **Stichprobengröße n** ↑ → MoE **kleiner**
  - **Streuung (s)** ↑ → MoE **größer**
  - **Konfidenzniveau** ↑ → MoE **größer** (breiteres Intervall)
- **Margin of error (Proportion)** hängt ab von n, dem Stichprobenanteil und dem Konfidenzniveau.
- Formeln (Zusatzwissen): Mean: `t × s/√n`, in Excel **`=CONFIDENCE.T(0.05; s; n)`**. Proportion: `z × √(p(1−p)/n)` mit z = 1,96 bei 95 %.
- **Visualisierung:** Column chart mit **Error bars** (Custom: positiver und negativer Wert = MoE) + Textfeld „95 % confidence interval".
- **Interpretation:** Liegt das **gesamte** 95 %-CI über 0, kann man mit 95 % Konfidenz sagen, dass der Mittelwert positiv ist. **Enthält das CI die 0**, kann man das nicht schließen.

### 5.9 Uncertainty in Predictive Models
- **Prediction interval (PI)**: Bereich, in dem eine **zukünftige Einzelbeobachtung** mit bestimmter Wahrscheinlichkeit liegt (breiter als ein CI, weil Einzelwerte stärker streuen).
- **Simple linear regression**: nähert die Beziehung zwischen **independent variable (x)** (Ursache, erklärend, horizontale Achse) und **dependent variable (y)** (Wirkung, vorhergesagt, vertikale Achse) mit einer Geraden an.
- **Time series**: Je **weiter in der Zukunft**, desto **breiter** das Prediction interval (mehr Unsicherheit). In der Regression wird das PI breiter, je weiter x vom Mittelwert entfernt ist.
- Darstellung: Beobachtungen als Punkte, Point prediction als Linie, untere/obere PI-Grenze als (gestrichelte) Linien.

### 5.10 Workshop-Activities Modul 6 – Lösungen

**Activity 1 – Pop (500 Softdrinks): Count vs. % of Grand Total**
- **% (percent frequency)** ist meist nützlicher: Man kann direkt Anteile vergleichen, unabhängig von der Stichprobengröße, und es schätzt die Wahrscheinlichkeitsverteilung (Marktanteile). Counts sind nützlich, wenn absolute Mengen wichtig sind. Die Form des Charts ist identisch, nur die Achse ändert sich.

**Activity 2 – Histogram Death (700 Personen)**
- **Linksschief**: Die meisten sterben im höheren Alter (ca. 70–90), wenige jung. Modus im hohen Altersbereich, langer Schwanz zu jungen Altern. Mean < Median.

**Activity 3 – Skewness**
1. **Age of death → left-skewed**: die meisten sterben alt, wenige früh
2. **Scores in easy exam → left-skewed**: die meisten erreichen hohe Punkte, wenige niedrige
3. **Housing prices → right-skewed**: die meisten moderat, wenige sehr teure Häuser
4. **Adult male height → symmetric**: glockenförmig um den Durchschnitt

**Activity 4 – Frequency polygon DeathTwo**
- `=COUNTIF(B2:B701;"Female")`, Bins 0, 7, 14, … 105 / 7, 14, … 112
- `=FREQUENCY(A2:A328;E6:E21)/$F$3` (dynamisches Array → relative Häufigkeit)
- Labels: `=CONCAT("(";D6;",";E6;"]")`
- Clustered column chart → dann Line chart = Frequency polygon

**Activity 5 – Frequency polygon considerations**
1. Linksschiefe erkennen: **Mean < Median**; **Median − Q1 > Q3 − Median**; im Box plot ist der **untere Whisker länger**.
2. Alternative Darstellung: **Box and whisker charts** (Male/Female nebeneinander), Trellis von Histogrammen, Violin chart, Kernel density.
3. Ausreißer: Werte unter **Q1 − 1,5 × IQR** bzw. über Q3 + 1,5 × IQR zählen (im Box plot als Punkte sichtbar).

**Activity 6 – Strip chart & Jittered strip chart (HalfMarathon)**
- Sortieren (Sex Z→A, dann Time), Male = 10 und Female = 20 als y-Wert, Scatter chart mit 2 Serien, Marker **No fill**, Jitter `=C2+RAND()`, Legende durch Textfelder ersetzen.

**Activity 7 – CEO time in meetings**: Strip chart mit Jitter, `MEDIAN`, `AVERAGE`, `MODE.SNGL` (häufigster Wert).

**Activity 8 – Box & Whisker SalesComparison**: *Insert → Statistic Chart → Box and Whisker*. Insights: Vergleich von Median (Lage), Boxbreite/IQR (Streuung), Whisker-Länge (Schiefe), Ausreißer.

**Activity 9 – XFL viewership (Friday vs. Saturday)**: Beide Box plots in einem Chart. Vergleich von Median, IQR, Spannweite, Schiefe und Ausreißern formulieren („Saturday games have a higher/lower median viewership …").

**Activity 10 – Confidence-interval error bars**: *Chart Elements → Error Bars → More Options → Custom → Specify Value*, positive & negative = Zellen mit Margin of error.

**Activity 11 – FedTaxErrors (n = 10 001)**
1. Mean: `=AVERAGE(...)` · 2. SD: `=STDEV.S(...)` · 3. MoE: `=CONFIDENCE.T(0.05; s; n)`
4. Column chart mit Error bars ±MoE
5. Liegt die **untere CI-Grenze > 0**, kann man mit 95 % Konfidenz auf durchschnittliche **Unterzahlung** schließen. Enthält das CI die 0, kann man es nicht.

**Activity 12 – Prediction intervals regression (Yourier)**
- Mit steigender Anzahl an Requests steigt die Travel time (positiver linearer Zusammenhang). Die meisten Beobachtungen liegen im 95 %-PI-Band. Das Band ist breiter für Werte weiter weg vom Mittelwert von x, also sind Vorhersagen dort unsicherer.

**Activity 13 – Prediction intervals time series (Bundaberg root beer)**
- Point forecasts setzen Trend und **Saisonalität** fort. Das 95 %-PI **wird breiter, je weiter die Prognose in die Zukunft reicht** → Planung sollte die Unsicherheit berücksichtigen.

### 5.11 Mögliche Prüfungsfragen Modul 6
- Mean, Median, Mode, Range, SD, Percentile, Quartile, IQR definieren; wann Median statt Mean?
- Skewness für Beispiele bestimmen und begründen (Activity 3!).
- Box plot lesen: Median, IQR, Ausreißer, Schiefe; zwei Verteilungen vergleichen.
- Ausreißergrenzen berechnen (Q1 − 1,5 IQR, Q3 + 1,5 IQR).
- Bins festlegen (Anzahl, Breite, Range); Notation (a, b].
- Was ist Occlusion und wie behebt man sie (Jitter, hohle Marker)?
- Confidence interval vs. prediction interval; was beeinflusst die Margin of error?
- **Datei:** Histogram, Box & whisker, Strip chart, Column chart mit Error bars, Frequency polygon erstellen.

<div style="page-break-after: always;"></div>

## 6. Modul 7 – Exploring Data Visually

### 6.1 Exploratory Data Analysis (EDA)
- Daten verstehen durch **deskriptive Statistik und Visualisierung**, **bevor** man analysiert/präsentiert.
- **Ziele:**
  1. **Fehler, fehlende Werte und ungewöhnliche Beobachtungen** finden
  2. **Verteilung einzelner Variablen** charakterisieren (univariate)
  3. **Muster und Beziehungen** zwischen Variablen identifizieren (multivariate)
- **Structural dimensions:** **Tall data** = viele Zeilen (Records). **Wide data** = viele Spalten (Variablen). Je größer, desto wahrscheinlicher sind Fehler/Lücken. Wide data ist schwerer zu explorieren (viele Variablenkombinationen).
- Excel-Werkzeuge: **Excel Table** (Format as Table), **Filter & Sort** (alphabetisch, chronologisch, nach Größe), **Calculated fields** (z. B. Time to Deliver = Delivered − Ordered), Year/Month/Day-Variablen ableiten, **Total Row**, **Conditional formatting** für fehlende Werte.

### 6.2 Univariate Analyse
- Eine Variable nach der anderen. **Kategorial** → PivotTable/PivotChart (Frequency distribution), ordinal **nicht umsortieren**. **Quantitativ** → Histogram, Box plot.
- **PivotTable**: berechnet, fasst zusammen und analysiert Daten (Vergleiche, Muster, Trends). **PivotChart**: interaktive Visualisierung dazu.
- **Outliers im Box plot** untersuchen: Wenn fehlerhaft → ggf. entfernen. **Aber nicht ohne guten Grund entfernen**, sonst wird die Variabilität künstlich reduziert und die Analyse verzerrt.

### 6.3 Multivariate Analyse – Beziehungen
- **Crosstabulation**: Tabelle mit der Beziehung zwischen **zwei oder mehr (meist kategorialen) Variablen** (bei quantitativen: Bins bilden). In Excel als PivotTable, interaktiv mit **Slicers** filtern.
- **Scatter chart** für zwei quantitative Variablen:
  - **Aspect ratio**: möglichst **quadratisch** (Höhe = Breite), damit keine Variable bevorzugt wird
  - **Achsenskalen**: knapp **unter dem Minimum** beginnen und knapp **über dem Maximum** enden
  - **Trendline**: positive Steigung = positive Korrelation, negative = negative
- **Correlation (r)**: Stärke des **linearen** Zusammenhangs, **−1 bis +1**. Nahe 0 = kein linearer Zusammenhang (aber evtl. **nichtlinear**!). Visuell: Je enger die Punkte an der Trendline, desto stärker die Korrelation.
- **Spurious relationship** (Scheinkorrelation), möglich wenn:
  - eine **dritte Variable (lurking variable)** beide beeinflusst
  - die Daten **verzerrt/nicht repräsentativ** sind
  - die Datenmenge zu klein ist, um Zufall auszuschließen
- **Correlation ≠ Causation!**
- **Nichtlineare Trendline** (z. B. Polynom) kann einen Zusammenhang zeigen, den eine lineare Trendline nicht erkennt.
- **Kategoriale Variable im Scatter:** Farbe pro Kategorie (eigene Datenreihen) oder **eine Kategorie hervorheben** (Rest grau, ohne Füllung) + eigene Trendline.
- **Scatter-chart matrix**: alle paarweisen Scatter charts aller quantitativen Variablen in einem Raster.
- **Table lens**: Tabelle mit horizontalen **Balken proportional zu den Werten**. Gut für **wide und tall data**. Nach einer Variable **absteigend sortieren**, dann gilt:
  - Muster groß → klein in einer anderen Spalte = **positive** Beziehung
  - Muster klein → groß = **negative** Beziehung
  - kein Muster = **keine** Beziehung

### 6.4 Missing Data
- **Legitimately missing**: natürlicherweise fehlend (Frage nicht relevant, z. B. nach „N/A")
- **Illegitimately missing**: Befragte antworten nicht, brechen ab, Sensor fällt aus
- **3 Optionen** bei illegitim fehlenden Daten:
  1. Beobachtungen/Zeilen mit fehlenden Werten **entfernen**
  2. Fehlende Werte mit **Schätzwerten füllen** (Imputation)
  3. Fehlende Werte als **eigene Kategorie** behandeln (nur bei kategorialen Variablen)
- **Zuerst** versuchen, den echten Wert zu finden (Quelle prüfen, logisch herleiten).

| Typ | Bedeutung | Beispiel | Umgang (Faustregel) |
|---|---|---|---|
| **MCAR** – Missing Completely At Random | Fehlen hat **nichts** mit dem Wert oder anderen Variablen zu tun | Datei beschädigt, zufälliger Sensor-Ausfall | Entfernen erzeugt keine Verzerrung (nur weniger Daten); einfache Imputation ok |
| **MAR** – Missing At Random | Fehlen hängt mit **einer anderen Variable** zusammen | Männer geben seltener ihren Job-Titel an | Mit den anderen Variablen schätzen (z. B. Gruppenmittelwerte); einfaches Entfernen kann verzerren |
| **MNAR** – Missing Not At Random | Fehlen hängt mit **dem fehlenden Wert selbst** zusammen | Geringe Bildung → Bildungsfrage leer gelassen | Am problematischsten: Entfernen/Imputation verzerrt; eigene Kategorie, Ursache untersuchen, offen kommunizieren |

- **Muster fehlender Daten** erkunden: z. B. Häufigkeiten nach Distribution Center **mit vs. ohne** Rating vergleichen.

### 6.5 Time Series Data
- **Line chart** zeigt:
  - **Trend**: langfristiges Muster über mehrere Perioden
  - **Variability**: Unterschied von Periode zu Periode
  - **Seasonality**: regelmäßig wiederkehrendes Muster (stündlich, täglich, monatlich, quartalsweise …)
- **Temporal frequency**: Rate, mit der Daten auf der x-Achse dargestellt werden (jährlich/quartalsweise/monatlich). **Niedrigere Frequenz glättet** (versteckt Saisonalität), höhere zeigt mehr Variabilität.
- **Seasonality erkennen**: **eine Linie pro Jahr** (x = Monat/Quartal) übereinanderlegen.
- **Trendline** (linear) nutzt **alle** Daten. Für Zeitreihen besser **Moving average**: Mittelwert der letzten x Perioden; nutzt nur Daten **bis zum aktuellen Zeitpunkt** und **keine aus ferner Vergangenheit**.
- **Trellis display**: gleiche Größe/Skalen/Formatierung, nur Daten unterscheiden sich (z. B. 3-, 6-, 12-Monats-Moving-Average).
- **Stacked data** (alle Werte in **einer** Spalte, eine weitere Spalte gibt die Gruppe an) vs. **Unstacked data** (jede Gruppe in **eigener Spalte**). Je nach Chart umformen.
- **Sparklines**: Mini-Line-Charts **in einer Zelle**; zeigen den **Trend, nicht die Magnitude**; keine Achsen/Labels; neben die Daten platzieren. *Insert → Sparklines → Line*.
- Box plots auch für Zeitreihen (aus unstacked Daten, z. B. pro Jahr).

### 6.6 Geospatial Data

| | Choropleth map | Cartogram | Equal-area cartogram |
|---|---|---|---|
| **Was** | Flächen nach Wert eingefärbt (Farbe/Schattierung/Symbole) | Flächen **verzerrt proportional zur Variable** | Alle Flächen **gleich groß**, Farbe = Wert |
| **Stärken** | High-level-Muster nach Region; **relative** Vergleiche; vertraut (Wetterkarte) | Nutzt Geografie-Wissen des Publikums; vermeidet, dass große, dünn besiedelte Flächen dominieren | Ausgewogen, jede Region gleich sichtbar, Position bleibt erkennbar |
| **Schwächen** | Große Flächen dominieren visuell; zu grobe **Granularität** versteckt Variation innerhalb und erzeugt abrupte Sprünge zwischen Regionen; **absolute Werte** irreführend | Starke Verzerrung macht die Karte unkenntlich | Fläche ohne Bedeutung |
| **Gut, wenn** | Variable innerhalb der Regionen relativ konstant; **dichte-/rate-basierte** Werte; Regionen etwa gleich groß | – | Viele kleine und große Regionen |

### 6.7 Workshop-Activities Modul 7 – Lösungen

**Activity 1 – PivotChart mit Slicers (EJB)**: $ Sales → Values, Distribution Centre + Year Ordered → Rows, New Customer? → Columns, Stacked Column, Slicers einfügen, Field Buttons verstecken, Achse in Thousands. Fragen per Slicer beantworten; prozentuale Veränderung = **(neu − alt) / alt**.

**Activity 2 – Rotwein-Studie (Kopenhagen)**
- **Nein**, man kann keine Kausalität ableiten: Es ist eine **Beobachtungsstudie**, die nur eine **Korrelation** zeigt. **Lurking variables** wie **Einkommen und Bildung** (Weintrinker waren reicher und gebildeter) beeinflussen vermutlich sowohl den Weinkonsum als auch die Gesundheit (Ernährung, Sport, Gesundheitsversorgung).
- **Verbesserung:** **randomisiertes kontrolliertes Experiment** (zufällige Zuteilung zu Wein/kein Wein), oder für Confounder kontrollieren (nach Einkommen/Bildung stratifizieren und vergleichen), größere und repräsentative Stichprobe.

**Activity 3 – Körperfett % vs. Exertion level (1–4, ordinal)**
- Exertion ist **ordinal mit nur 4 Werten**, deshalb ist ein Scatter chart schlecht (Occlusion, Punkte in 4 Reihen). Besser: **Box and whisker chart des Körperfetts pro Exertion level** (Verteilung je Gruppe vergleichbar) oder **jittered strip chart**; einfacher: Column chart des durchschnittlichen Körperfetts je Level (in natürlicher Reihenfolge 1–4).

**Activity 4 – Correlation analysis of wide data (Dutzende Variablen)**
- **Scatter-chart matrix**: zeigt alle paarweisen Beziehungen, wird bei Dutzenden Variablen aber sehr groß/unübersichtlich.
- **Table lens**: gut für **wide und tall** data, nach Variable sortieren und Muster lesen; bleibt auch herausgezoomt lesbar.
- Empfehlung: Table lens (oder Correlation heat map) zum Screening, dann Scatter charts für die interessantesten Paare.

**Activity 5 – Types of missing data**
- a) Bildungsangabe fehlt häufiger bei niedriger Bildung → **MNAR** (Fehlen hängt vom fehlenden Wert selbst ab)
- b) Job-Titel fehlt häufiger bei Männern → **MAR** (Fehlen hängt mit einer **anderen** Variable, dem Geschlecht, zusammen)

**Activity 6 – Univariate EJB**: PivotChart mit „% of Grand Total" für Category bzw. New Customer (Labels „Existing"/„New" umbenennen) und Ergebnisse beschreiben.

**Activity 7/8 – NYC Scatter mit Borough-Serien & Queens hervorheben**
- Nach Borough sortieren, jede Borough als eigene Serie (*Select Data → Add*). Dann alle außer Queens **grau, no fill**, Trendline **nur für Queens**.
- Interpretation: In **Queens ist der positive Zusammenhang** zwischen % College-Absolventen und Median Rent **schwächer** (flachere Trendline, Punkte streuen stärker) als über alle Boroughs.

**Activity 9 – Table lens Bravman**: absteigend nach Purchase Amount sortieren, Data bars (*Conditional Formatting → Data Bars*) auf jede Spalte, dann für Wait time, Age und Credit score jeweils positive/negative/keine Beziehung ablesen.

**Activity 10 – Smartphone sales (annual/quarterly/monthly)**
- **Annual**: langfristiger Trend klar, Saisonalität unsichtbar (geglättet)
- **Quarterly**: Saisonalität (z. B. Q4-Peaks) erkennbar, Trend noch sichtbar
- **Monthly**: maximale Variabilität/Details, aber mehr „Rauschen"; Monatsmuster erkennbar
- Fazit: Verschiedene Temporal frequencies zeigen verschiedene Muster, also mehrere Ansichten prüfen.

**Activity 11 – Moving average trendline (Pear Juice)**: Rechtsklick Datenreihe → *Add Trendline → Moving Average, Period 3* (dann 6, 12) → Trellis display. Längere Periode = glatter, reagiert aber langsamer.

**Activity 12 – Umbrella sales**: Line chart + **4-period moving average** (Quartalsdaten → glättet die Saisonalität eines Jahres). Saisonalität: 5 Linien (eine pro Jahr, x = Q1–Q4). Wiederholen sich Hoch-/Tiefpunkte in denselben Quartalen jedes Jahr, liegt Saisonalität vor.

### 6.8 Mögliche Prüfungsfragen Modul 7
- Ziele der EDA; tall vs. wide data.
- MCAR/MAR/MNAR anhand von Beispielen zuordnen und begründen (sehr wahrscheinlich!).
- Optionen für fehlende Daten nennen.
- Korrelation vs. Kausalität; Lurking variable; Studie kritisieren (Rotwein).
- Welche Visualisierung für Beziehung X (ordinal vs. quantitativ, wide data)?
- Table lens interpretieren.
- Trend/Variability/Seasonality; Temporal frequency; Moving average vs. lineare Trendline.
- Choropleth vs. Cartogram: Stärken/Schwächen.
- **Datei:** PivotChart + Slicers; Scatter mit Kategorien + Trendline; Moving average; Sparklines.

<div style="page-break-after: always;"></div>

## 7. Modul 8 – Explaining Visually to Influence with Data

### 7.1 Know your Audience
- **Storytelling** = aus Daten eine bedeutsame, einprägsame Erzählung bauen, die das Publikum beeinflusst.
- Zwei Dimensionen:
  1. **Insight needs**: **High-level understanding** (einfache Charts, Hauptbotschaft) vs. **detailed understanding** (komplexere Visualisierungen, regt Diskussion an)
  2. **Analytical comfort**: **low** (einfache Charts, eine Kernaussage, geringe Cognitive Load) vs. **high** (detailreiche, statistische Charts)
- Beispiele:
  - **Chan Life Insurance:** **Sales agents** brauchen High-level (Line chart der Gesamt-Antwortzeit, Prognosen gestrichelt). **Underwriters** brauchen Details (Clustered column nach einzelnen Tasks).
  - **General Hospital:** **Niedriger** Komfort → Column chart der durchschnittlichen Zufriedenheit. **Hoher** Komfort → Box and whisker chart.
- **Chart-Matrix** (eigene Zuordnung nach Kurslogik, Lehrbuch S. 292; Hinweis: Scatter = detailed + high comfort):

| | Low analytical comfort | High analytical comfort |
|---|---|---|
| **Only high-level insights** | Simple bar/column charts, line charts, pie charts (wenige Kategorien), summary tables, dot matrix charts, BANs | Slope charts, bubble charts, geographic information systems (maps, choropleths), tree maps |
| **Detailed insights** | Clustered & stacked bar/column charts, cross-tabulation tables | Scatter charts, scatter-chart matrix, box & whisker, histograms, strip charts, violin charts, Sankey charts |

### 7.2 Know your Message – Was hilft dem Decision maker?
- Daten genau kennen: was sie für das Publikum bedeuten, welche **Limitationen** sie haben und wie diese die Insights beeinflussen.
- Decision maker müssen oft: viele quantitative + qualitative Faktoren abwägen, **Stakeholder-Auswirkungen** beachten, mit **unvollständigen Informationen** und unter **Zeitdruck** entscheiden.
- Daher: **klar, schnell interpretierbar, hohe Data-ink ratio, kein Chart junk.**

### 7.3 Empathising with Data
- **Empathy** = Gefühle anderer verstehen und teilen; Daten repräsentieren oft **echte Menschen**.
- **Zwei Herausforderungen + Strategien:**
  1. **Große Zahlen** verlieren Bedeutung (Menschen können sich nur Gruppen bis ca. 100 vorstellen):
     - in etwas **Vertrautes umrechnen** ($357 Mio. Lotto = $171.000 pro Woche für 40 Jahre)
     - **keine wissenschaftliche Notation** (Millionen/Milliarden statt 10⁶/10⁹)
     - **Kontext** geben, z. B. **Dot matrix chart** (40 Mio. verlorene Jobs ≈ 7 × Arbeitskräfte in Ohio)
  2. **Aggregierte Statistiken** verdecken Einzelfälle:
     - **Einzelfall/Persona** mit Namen und Eigenschaften, **Bilder** (Tierheimhund im Stacked column chart), Cluster-Ergebnisse als Personas darstellen
- **BAN – Big Associated Number**: eine Zahl in sehr großer Schrift (preattentive attribute **size**) zur Betonung.

### 7.4 Storytelling mit Charts
- **Den richtigen Chart wählen**: z. B. **Slope chart** statt clustered column, wenn die **Veränderung zwischen zwei Zeitpunkten** pro Entität die Botschaft ist (Opening Horizons: Durango ↑, Salida ↓ wird sofort sichtbar).
  - **Slope chart** = Line chart mit verbundenen Punktpaaren für mehrere Entitäten. Excel: Line with markers → **Switch Row/Column** → Gridlines/Legende/y-Achse entfernen, Labels links (Name + Wert) und rechts (Wert).
- **Preattentive attributes** für die Story: **Farbe** hebt eine Linie hervor (Florida im Subprime-Crash, Rest grau), **Größe** über BAN.
- **Drei Elemente einer Story** (HBR-Video): **Set-up → Conflict → Resolution**.

### 7.5 Aristotle's Rhetorical Triangle

| Element | Bedeutung | In Data Vis |
|---|---|---|
| **Ethos** | **Glaubwürdigkeit** | Korrekte Daten, nichts verzerren/verstecken, Datenquelle, Annahmen und Datenmanipulation offenlegen, alternative Interpretationen zeigen |
| **Pathos** | **Emotion** | Empathie erzeugen: Einzelfälle, Personas, Bilder |
| **Logos** | **Logik** | Klare, logische Argumentation: wie Daten und Analyse zu den Insights führen und warum diese bessere Entscheidungen ermöglichen |

### 7.6 Freytag's Pyramid (5 Teile)
1. **Introduction (Exposition)**: Problem, Kontext, warum wichtig; Protagonist/Persona einführen
2. **Rising action**: Spannung/Probleme bauen sich auf (Daten zeigen das Problem)
3. **Climax**: Höhepunkt des Konflikts, die zentrale Erkenntnis
4. **Falling action**: Empfehlungen/Lösungsweg
5. **Conclusion (Resolution)**: Kosten/Nutzen der Empfehlungen, Annahmen, Limitationen
- **Fehler** (Hawaiian Bell): Präsentation **chronologisch nach Analyseschritten** (Data cleaning → EDA → Ergebnisse). Das ist langweilig, die Botschaft kommt zu spät.
- **SCQA-Framework** (Video): **Situation, Complication, Question, Answer** + Pyramid principle (Kernaussage zuerst).

### 7.7 Storyboarding
- Visuelle Gliederung der Hauptpunkte einer Story; **modular**, Abschnitte lassen sich umsortieren.
1. **Low-tech: Sticky notes (Post-its)**: leicht hinzufügen/umsortieren/entfernen, zwingt zu methodischem Vorgehen, man springt nicht zu früh zu fertigen Folien
2. **High-tech: PowerPoint**: Folien entlang der Story-Phasen (Freytag) anlegen, **Slide sorter view** zum Umsortieren und für den Überblick. Storyboard **getrennt** von der finalen Präsentation entwickeln.

### 7.8 Spezielle Charts in Modul 8
- **Funnel chart** (*Insert → Waterfall, Funnel, Stock, Surface or Radar → Funnel*)
- **Stock chart High-Low-Close** (Datum + High, Low, Close auswählen; Close-Labels behalten, High/Low-Labels löschen, Close-Marker schwarz 3 pt)
- **Waterfall chart** (Total-Säule: *Format Data Point → **Set as total***)
- **Dot matrix chart** (Symbol ● in Zellen kopieren, Spaltenbreite verkleinern, Gridlines aus, Kontext per Zellfarbe = **Enclosure**)
- **Slope chart**, **BAN**

### 7.9 Workshop-Activities Modul 8 – Lösungen

**Activity 1 – Chan Life Underwriters**
- Problem: Clustered column mit vielen Tasks × 6 Zeitpunkten ist überladen, Augen springen zwischen Legende und Säulen.
- Alternative: **Multiple line chart** (eine Linie pro Task, x = Monat) mit **Labels direkt am Linienende** (keine Legende), **Prognosen gestrichelt oder heller** (Gestalt Connection/Similarity), ggf. eine Linie hervorheben. Oder **stacked column** für Gesamtzeit + Zusammensetzung, oder Small multiples.

**Activity 2 – Funnel chart (Data Science Hiring: 51 → 37 → 12 → 7 → 4)**
- Weitere Einsatzbereiche: **Sales pipeline** (Leads → Opportunities → Abschlüsse), **Website-/E-Commerce-Conversion** (Besuch → Warenkorb → Kauf), Marketing-Kampagnen, Uni-Bewerbungen, Onboarding-Prozesse, Ticket-/Support-Eskalation.

**Activity 3 – Slope chart Opening Horizons** (Previous → Current Year)

| Standort | Vorjahr | Aktuell | Veränderung |
|---|---|---|---|
| Durango | 341 | 432 | **+91 (+26,7 %)**, jetzt größter Standort |
| Salida | 395 | 360 | **−35 (−8,9 %)**, verliert Platz 1 |
| Pagosa Springs | 302 | 298 | −4 (−1,3 %) |
| Montrose | 198 | 202 | +4 (+2,0 %) |
| Gunnison | 164 | 150 | −14 (−8,5 %) |

- Insight: Durango und Salida entwickeln sich **gegenläufig**. Durango überholt Salida, die übrigen bleiben weitgehend stabil.

**Activity 4 – ESU Engineering Salaries (Slope chart)**

| Major | Start | 5 Jahre | Zuwachs |
|---|---|---|---|
| Chemical | $72.500 | $91.400 | +$18.900 (+26 %), **bleibt am höchsten** |
| Electrical | $64.800 | $87.400 | **+$22.600 (+35 %), stärkster Anstieg**, überholt Computer |
| Computer | $68.400 | $83.600 | +$15.200 (+22 %) |
| Mechanical | $62.900 | $77.100 | +$14.200 (+23 %) |
| Industrial | $57.400 | $74.000 | +$16.600 (+29 %), überholt Civil |
| Civil | $61.000 | $70.300 | **+$9.300 (+15 %), schwächster Anstieg**, wird zum niedrigsten |

- Insight: Alle Gehälter steigen. Die Rangfolge ändert sich (Linien kreuzen sich): Electrical und Industrial holen auf, Civil fällt zurück.

**Activity 5 – Dot matrix (40 Mio. Jobs)**: 20 × 20 = 400 Punkte, **1 Punkt = 100.000 Jobs**. Ohio-Arbeitskräfte ≈ 58 Punkte (≈ 5,8 Mio.) blau eingefärbt. Text: „almost 7 times larger than the total labour force in Ohio".

**Activity 6 – Drinking water (663 Mio. Menschen)**
- a) **BAN** „663 million" groß neben/über das Bar chart
- b) Dot matrix: **25 × 26 = 650 + 13 = 663 Punkte**, ● = 1 Mio.
- c) Farben nach Region + Legende (categorical colour scheme)
- d) **330 Punkte** (≈ US-Bevölkerung) per Fill colour hinterlegen = **Gestalt-Prinzip Enclosure**, beschriften („≈ population of the USA")

**Activity 7 – Stock chart Verizon**: zeigt Schlusskurs-Trend und tägliche **Volatilität** (Länge der High-Low-Linie).

**Activity 8 – Waterfall Gossamer**: Total-Säule als **Set as total** markieren. Zeigt, wie sich die monatlichen Gross Profits zum Gesamtwert aufsummieren (positive vs. negative Monate).

**Activity 9 – Air Transat Storyboard (Freytag)**
1. **Introduction**: Juli 2017, zwei Air-Transat-Flüge wegen Wetter nach Ottawa umgeleitet. Persona einführen (z. B. Familie mit Kleinkind an Bord).
2. **Rising action**: Passagiere **über 4 Stunden auf dem Rollfeld**, auf einem Flug ohne Essen, Wasser, Klimaanlage. Frust und Gesundheitsrisiko steigen (Daten: Wartezeit, Temperatur, Anzahl Betroffener).
3. **Climax**: Ein Passagier ruft den **Notruf 911**, damit die Airline handelt. Medien berichten.
4. **Falling action**: CTA-Untersuchung; Airline und Flughafen **schieben sich gegenseitig die Verantwortung zu**; Airline wird **bestraft/haftbar gemacht**.
5. **Conclusion**: Empfehlungen (klare Tarmac-Delay-Protokolle, Versorgung nach X Stunden, klare Verantwortlichkeiten, Kommunikation) mit Kosten/Nutzen, Annahmen und Limitationen.
- Im PowerPoint-Slide-Sorter je Phase 1–2 Folien. Ethos/Pathos/Logos einbauen.

### 7.10 Mögliche Prüfungsfragen Modul 8
- Wie beeinflussen Audience needs und analytical comfort die Chart-Wahl? Beispiele zuordnen.
- Zwei Herausforderungen beim Erzeugen von Empathie + Strategien.
- Was ist ein BAN / Dot matrix chart / Slope chart, und wann setzt man sie ein?
- Rhetorical triangle (Ethos, Pathos, Logos) erklären und auf einen Fall anwenden.
- Freytag's Pyramid: 5 Phasen, Storyboard für einen Fall (Air Transat!) entwerfen.
- Storyboarding: Sticky notes vs. PowerPoint.
- **Datei:** Slope chart (Opening Horizons / ESU), Funnel, Waterfall (Set as total), Stock chart, Dot matrix + BAN.

<div style="page-break-after: always;"></div>

## 8. Modul 9 – Data Dashboards

### 8.1 Was ist ein Data Dashboard?
- Visualisierungstool, das **mehrere Outputs** liefert und sich ggf. **in Echtzeit** aktualisiert. Es gibt Entscheidern rechtzeitig Informationen zu **KPIs (Key Performance Indicators)**, also zum **„moment of value"**, an dem entschieden wird.
- KPIs sind an den **Unternehmenszielen** ausgerichtet und je nach Organisation unterschiedlich (z. B. Finanzlage, Lagerbestand, offene Bestellungen, Projektfortschritt, Kundenservice-Kennzahlen).

### 8.2 Principles of Effective Dashboards
1. **Alle KPIs** zu einem Aspekt auf **einem Bildschirm** („at a glance")
2. Lieber **mehrere Dashboards** mit zusammengehörigen KPIs als Scrollen
3. KPIs müssen **schnell und klar Bedeutung vermitteln** und zu den **Entscheidungen des Users** passen
4. Alle Komponenten folgen den **Prinzipien guter Data Vis** (Data-ink, Gestalt, preattentive …)
5. **Farbe sparsam**: um Werte hervorzuheben und Kategorien zu unterscheiden

### 8.3 Anwendungsbereiche (mit typischen KPIs)
- **Investment**: aktueller Kurs, Rendite, relatives Risiko vs. Markt, Anteil je Branche
- **Manufacturing**: produzierte Menge, Qualität, Produktionsgeschwindigkeit, Häufigkeit von Problemen (Maschinenausfall, Retouren, Zielverfehlung)
- **Marketing**: verkaufte/gelieferte Menge, Erfolgsquote von Sales calls, Umsatz/Preise, Werbeausgaben, Reichweite/Response, Kundenzufriedenheit
- **Human Resources**: Mitarbeiterzahl, Fluktuation (churn), Betriebszugehörigkeit, Leistung/Zufriedenheit, Fehlzeiten, Trainings, Kündigungsgründe
- **Technical support**: Problemtyp, Reaktions-/Lösungszeit, offene/wiederkehrende Probleme, Downtime, Wartung
- **Personal fitness/health**: Puls, Blutdruck, Gewicht/BMI, Schritte, Kalorien, Blutzucker
- **Donor**: Anzahl/Wert der Spenden, Kontakte, Ausgaben, Conversion rate, Cash flow, Kampagnenstatus
- Weitere: Crime, School performance

### 8.4 Dashboard Taxonomies

| Kriterium | Typ | Merkmale |
|---|---|---|
| **Data updates** | **Static** | günstig und einfach zu bauen, **manuell** und selten aktualisiert (aufwendig), gut bei **langsam** ändernden KPIs |
| | **Dynamic** | aufwendiger zu bauen, aktualisiert sich **automatisch** und häufig, gut bei **schnell** ändernden KPIs |
| **User interaction** | **Non-interactive** | keine Anpassung durch den User, gut bei selten ändernden Daten |
| | **Interactive** | User filtert/passt an: **Drill-down** (mehr Detail zu einem Element), **Hierarchical filtering** (verschachtelte Filter, z. B. Land → Region → Filiale), **Time-interval widget** (Zeitraum wählen), **Customisation tools** (Variablen/Kategorien ein-/ausblenden) |
| **Organisational function** | **Operational** | **untere Manager**, schnell ändernde kritische Bedingungen, **Echtzeit**-Updates |
| | **Tactical** | **mittleres Management**, Stärken/Schwächen analysieren, Strategieentwicklung, seltenere Updates |
| | **Strategic** | **Executives**, Status der KPIs zu übergeordneten Zielen, regelmäßig, aber seltener |
| | **Analytical** | **Analysten**, Trends untersuchen, Vorhersagen, Insights in großen Datenmengen |

### 8.5 Dashboard Design & Development
- **Purpose**: Operations, Entscheidungen und strategische Planung unterstützen. Mögliche Ziele: KPIs tracken/Prozesse überwachen, Zielerreichung bewerten, Insights entwickeln, Informationen teilen, Performance messen, Forecasting/Exploration.
- **Users' needs**: Dashboard für **bestimmte User und Aufgaben** designen. Team muss verstehen, was die User brauchen und wie das die Unternehmensziele unterstützt → bestimmt **welche Infos** und **wie** dargestellt. **User von Anfang an einbeziehen.**
- **Display**: passende Chart-Typen, preattentive attributes/Gestalt/Farbe, **praktisches Layout** (zusammengehörige Charts nebeneinander), Überfüllung vermeiden (Teilmengen, interaktive Tools), **Gerät, Umgebungslicht, Bildschirmgröße und Auflösung** beachten.
- **Context** für KPIs: Verlauf über die Zeit, Vergleich mit **Zielwert**, Vergleich **intern** (Abteilungen, Regionen) oder **extern** (Kunden, Wettbewerber, Branche).
- **Engineering**: Charts so anordnen, dass **Eye travel** minimal ist; Wartung und Wirksamkeitsprüfung; künftige Ziele/KPIs/Datenquellen einplanen.
- **Organisation (Excel)**:
  - Datenquelle in **eigenem Worksheet**
  - Dashboard **nicht direkt** aus den Quelldaten speisen; benötigte Daten in **separates** Worksheet extrahieren (PivotTables)
  - User dürfen **keine dauerhaften Änderungen** machen (Blatt schützen, Hilfsblätter ausblenden)
- **Testing**: in jedem Schritt testen. Sonst: fehlerhaftes Produkt mit schlechten Entscheidungen, teure Überarbeitungen, Glaubwürdigkeitsverlust. **Final review**: alle Slicer-Kombinationen testen, User testen lassen (benutzerfreundlich, erwartete Funktion und Outputs), laufenden Monitoring-/Revisionsprozess aufsetzen.

### 8.6 Common Mistakes in Dashboard Design
1. Ziele/Bedürfnisse der Organisation ignorieren (Wichtiges fehlt, Unwichtiges dominiert, **User nicht einbezogen**)
2. **Nutzungsumgebung** ignorieren (Gerät, Licht, Touch/Beamer)
3. Charts/Tabellen **falsch positioniert** (zusammengehörige nicht nebeneinander)
4. **Ungeeignete Chart-Typen**
5. Design-Prinzipien bei einzelnen Komponenten ignoriert
6. **Zu überladen oder zu leer** (cluttered/sparse)
7. **Unattraktives** Design (z. B. grelle Hintergrundfarbe, Schnörkelschrift)
8. **Künftige Bedürfnisse** nicht berücksichtigt

### 8.7 Excel-Werkzeuge für Dashboards
- **PivotTables** (Filter), **PivotCharts** (interaktive Charts), **Slicers** (Buttons zum Filtern)
- **Connected slicers**: Ein Slicer steuert mehrere PivotCharts. *Slicer auswählen → Slicer-Tab → **Report Connections** → PivotTables anhaken*
- Field Buttons verstecken (*Hide All Field Buttons*), Achse in Thousands, **Don't move or size with cells**, Autofit column widths deaktivieren, Gridlines aus, **einheitliche Farbcodierung** (*File → Options → Advanced → Properties follow chart data point*)
- **Schutz**: Slicer „Disable resizing and moving" + nicht locked; *Review → Allow Edit Ranges*; *Protect Sheet* mit „Use PivotTable & PivotChart" + Passwort; Hilfsblätter ausblenden (*Hide*)
- **EJB-Dashboard** (mid-level operations, also **tactical**, **dynamic & interactive**): KPIs = **total $ sales** und **average delivery time**. Charts: (1) Stacked column Sales nach DC × Jahr × Neu/Bestand, (2) Line chart Sales nach Jahr/Monat × Category, (3) Clustered column Sales nach Jahr × Flavour × Category, (4) Clustered bar Ø Lieferzeit nach DC × Jahr, (5) PivotTable Sales nach Category/Flavour/DC/Datum. Layout: Charts 1 + 3 (Sales nach Jahr), 1 + 4 (DC-Ebene), 2 + 3 (Category-Ebene) jeweils nebeneinander; Tabelle oben.

### 8.8 Workshop-Activities Modul 9 – Lösungen

**Activity 1 – Alternatives EJB-Dashboard verbessern** (Bild: grell gelber Hintergrund, Schnörkel-Titel, kleine Charts unten, große Slicer-Fläche)
- **Hintergrund** neutral/dunkel statt grellem Gelb (Kontrast, weniger Ablenkung)
- **Titel** in Sans-serif statt Script-Schrift (Lesbarkeit)
- **Charts größer**, Slicer kompakter/kleiner und **neben die zugehörigen Charts** (Proximity, weniger Eye travel); ggf. **Connected slicers**, damit weniger Slicer nötig sind
- Zusammengehörige Charts nebeneinander, Tabelle oben
- **Konsistente Farbcodierung** (Neu/Bestand, Juice/Smoothie, Jahre) über alle Charts
- Überfüllte x-Achsen vereinfachen (z. B. Quartale statt Tage), Data-ink ratio erhöhen

**Activity 2 – Service vs. Product Satisfaction je DC über 3 Jahre**
- a) **Scatter chart**: x = Ø Service-Rating, y = Ø Product-Rating, **jeder Punkt = ein Distribution Center**, **eine Serie/Farbe pro Jahr** oder **Trellis display** (3 Scatter mit gleichen Skalen, einer pro Jahr). Grund: Beziehung zwischen zwei quantitativen Variablen; Trellis erlaubt den Jahresvergleich. Plus PivotTable mit beiden Durchschnitten nach DC × Jahr.
- b) PivotChart + Slicer für Year (mit bestehendem Year-Slicer **verbunden**) einfügen, neben dem DC-Chart (Chart 4) platzieren, Tabelle neben/unter die bestehende Tabelle. Alles weiterhin auf **einem Bildschirm**, ggf. andere Elemente verkleinern.

**Activity 3 – Weitere Manufacturing-KPIs**
- **OEE (Overall Equipment Effectiveness)**, Ausschuss-/Fehlerquote (scrap/defect rate), First-pass yield, Kapazitätsauslastung, Zykluszeit/Durchlaufzeit, Termintreue (on-time delivery), Lagerbestand/Lagerumschlag, Kosten pro Einheit, Arbeitsunfälle (safety incidents), Energieverbrauch, Mean time between failures (MTBF), Rüstzeit (changeover time), Arbeitsproduktivität, Kundenreklamationen.

**Activity 4 – EJB-Dashboard bauen**: Schritte siehe Anhang A (PivotChart & PivotTable, Slicers, Move Chart, Report Connections, Protect Sheet).

### 8.9 Mögliche Prüfungsfragen Modul 9
- Definiere Data Dashboard und KPI; Prinzipien effektiver Dashboards.
- Taxonomien erklären: static/dynamic, interactive/non-interactive (Drill-down, Hierarchical filtering …), operational/tactical/strategic/analytical; einem Szenario zuordnen.
- KPIs für einen Bereich vorschlagen (Manufacturing, HR, Marketing …).
- Design-Überlegungen (Purpose, User needs, Display, Context, Engineering, Testing).
- Häufige Fehler; ein Dashboard kritisieren und verbessern.
- **Datei:** PivotChart + Slicers erstellen, Slicer verbinden, Dashboard-Layout.

<div style="page-break-after: always;"></div>

## 9. Modul 10 – Telling the Truth with Data Visualisation

### 9.1 Missing Data & Data Errors
- Schlechte Datenqualität → irreführende Visualisierungen → schlechte Entscheidungen. **Zuerst fehlende Daten, dann Fehler** behandeln.
- **Fehlende Daten in Excel finden:**
  - **Sort** (Leerzellen landen am Ende)
  - **Conditional Formatting** (*Home → Conditional Formatting → Highlight Cells Rules → More Rules → Format only cells that contain → **Blanks***)
  - **`=COUNTBLANK(C2:C457)`** pro Variable
  - Filter (Blanks)
- **Datenfehler** (Ursachen: manuelle Eingabefehler, falsch kalibrierte Sensoren) finden über:
  - **Summary statistics** (`MIN`, `MAX`, `AVERAGE`) → unrealistische Werte (Blakely Tires: Reifenlebensdauer 601 Monate statt 60,1; Profiltiefe 16,7/12 > Neureifen; 0,0 = nicht fahrbar)
  - Sortieren, Frequency distributions, **Histogramme**
  - **Scatter charts** → auch **nicht-extreme** Fehler (Punkte, die nicht zur Beziehung passen)
- Erst sicher sein, dass ein Wert falsch ist → **mehrere Methoden kombinieren**. Dann logisch korrigieren (601 → 60,1) oder als fehlend behandeln.

### 9.2 Biased Data
- **Bias**: Die Stichprobe repräsentiert die Zielpopulation nicht (**nicht zufällig** gezogen).
- **Selection bias**: Stichprobe nicht zufällig, repräsentiert die Population nicht (z. B. Umfrage nur per Festnetz → eher ältere Befragte; Umfrage zum Trinken & Fahren vor einer Bar spät abends).
- **Simpson's paradox** (Form der Selection bias): Ein **Trend in Teilgruppen kehrt sich um oder verschwindet**, wenn die Gruppen **aggregiert** werden (Ursache: Lurking variable bzw. ungleiche Gruppengrößen). **Erkennen:** Scatter chart aggregiert vs. **nach Gruppe eingefärbt/disaggregiert** vergleichen.
- **Survivor bias**: Die Stichprobe enthält überproportional viele Beobachtungen mit **positivem Ausgang** eines vorherigen Ereignisses (nur die „Überlebenden" werden betrachtet). Klassiker: **WWII-Flugzeuge**, nur zurückgekehrte Flugzeuge analysiert; die Einschusslöcher zeigen, wo Treffer **überlebbar** sind, also sollte man die Stellen **ohne** Löcher panzern. Beispiel: erfolgreiche Unternehmer haben hohe Risikotoleranz (die gescheiterten fehlen in der Stichprobe).
- **Deine Notiz:** *selection, survivor (brilliance bias) and Simpson's paradox (confirmation bias)*
- **Artefacts**: künstliche Muster durch Mängel in der Datenerhebung, nicht mit echten **Fakten** verwechseln.

### 9.3 Adjusting for Inflation
- **Inflation** = allgemeiner Anstieg nominaler Preise über die Zeit, gemessen über einen **Price index** (Preis eines Warenkorbs, z. B. CPI). Den **passendsten Index** für die Produktart wählen.
- **Formel (Base year B):**

  **Inflationsbereinigter Wert(t) = Nominaler Wert(t) × Index(B) / Index(t)**

- Beispiel Folie: Benzin 1978 = $0,65; Index 1978 = 51,9; Index 2017 = 211,8 → 0,65 × 211,8 / 51,9 ≈ **$2,65–2,66** in 2017-Dollar. Excel: **`=B2*($C$41/C2)`** (absoluter Bezug auf den Basisjahr-Index!)
- Basisjahr frei wählbar, abhängig von den gewünschten Vergleichen (oft das aktuellste Jahr).
- Makeover-Beispiel: Box-Office-Top-10 sieht inflationsbereinigt völlig anders aus (ältere Filme rücken nach oben).

### 9.4 Deceptive Design

**a) Chart axes**
- **Column/Bar charts: y-Achse immer bei 0 beginnen** (Länge = Wert). Ein abgeschnittener Achsenstart **übertreibt Unterschiede** (z. B. Wählerumfrage 52 % vs. 48 % sieht wie Faktor 3 aus). Ausnahme: negative und positive Werte im gleichen Chart.
- **Line/Scatter charts** (Orientation/Position): Hier darf/soll die Achse **enger** sein, um Variabilität/Trend/Korrelation sichtbar zu machen. Eine zu weite Skala **versteckt Insights** (Erdtemperatur auf 0–100 °F-Skala wirkt flach).
- **Aspect ratio** (Breite : Höhe): **Hoch & schmal** (kleine Aspect ratio) **übertreibt** Trends, **flach & breit** (große Aspect ratio) **versteckt** Trends.

**b) Dual-axis charts**
- Zwei Variablen mit unterschiedlichen Einheiten/Größenordnungen auf **Primär- und Sekundärachse**. Schwer zu lesen, verleitet zu **falschen Vergleichen**: Schnittpunkte und relative Höhen sind bedeutungslos und hängen nur von der Skalenwahl ab, sodass sich jede gewünschte Beziehung „konstruieren" lässt.
- **Lösung:** **zwei separate Charts** (untereinander, gleiche x-Achse) mit je einer Variable.

**c) Data selection & temporal frequency**
- Die **Auswahl des Zeitraums** (Start-/Enddatum) bestimmt die Botschaft (Cherry picking).
- **Niedrige Temporal frequency glättet** → versteckt saisonale/zyklische Schwankungen (z. B. Aktienkurs täglich vs. monatlich). Daten möglichst häufig erheben und **mehrere Frequenzen** betrachten.

**d) Geographic maps**
- **Absolute Zahlen** auf Choropleth maps spiegeln oft nur die Bevölkerungsgröße (Anzahl Menschen in Armut → große Staaten dunkel). **Besser relative Werte/Raten** (Poverty **rate** = Armut / Bevölkerung).

### 9.5 Workshop-Activities Modul 10 – Lösungen

**Activity 1 – Java Cup Taste Data (217 Befragte, Skala 0–100)**
- a) **Missing values**: `=COUNTBLANK()` pro Spalte, **Conditional Formatting → Blanks** hervorheben, nach Spalte sortieren/filtern (Blanks) → Respondent-ID und fehlende Variable notieren. (Deine Notiz: *Price, Conditional Formatting, Count Blank*)
- b) **Erroneous values**: Skala 0–100, also mit `MIN`/`MAX` je Spalte prüfen, **sortieren/filtern**, Conditional Formatting für Werte **< 0 oder > 100** (oder Nicht-Zahlen), ggf. Histogram/Scatter. Werte wie 150 oder −5 oder Kommafehler (z. B. 7,5 statt 75) markieren. (Deine Notiz: *Sort, Filter, min/max*)
- **Antwort-Skizze (EN):** *"Using COUNTBLANK on each column and conditional formatting for blank cells, respondents X and Y have missing values for …. Sorting each variable and checking MIN/MAX against the valid 0–100 scale shows respondent Z has a value of … for …, which is impossible and therefore likely an entry error."*

**Activity 2 – Bias zuordnen** (deine Lösungen aus dem Workshop)
1. **Dr. Rhine / Telepathie → Survivor bias**: Nur wer in jeder Runde richtig lag, kam weiter. Bei 500 Teilnehmern gewinnt rein zufällig jemand jede Runde. Die vielen „Ausgeschiedenen" werden ignoriert, die Schlussfolgerung beruht nur auf dem „Überlebenden".
2. **Exit poll vor Restaurant spät abends → Selection bias**: Die Stichprobe (Gäste, die nachts trinken, Lobbygruppe der Alkoholindustrie) ist **nicht zufällig** und nicht repräsentativ für die Bevölkerung. Diese Gruppe hält Trinken & Fahren eher für unproblematisch.
3. **Rotwein-Kohorte (40 Jahre) → Simpson's paradox**: Die aggregierten Daten zeigen „Weintrinker = gesünder". Weintrinker sind aber **reicher und gebildeter** (Lurking variable). Disaggregiert man nach Einkommen/Bildung, kann der Zusammenhang verschwinden oder sich umkehren. Aggregation über ungleiche Gruppen erzeugt den Scheineffekt.

**Activity 3 – Guaraldi Consultants (Scatter + Trendline, Simpson's paradox)** – nachgerechnet mit `Module 10.xlsx`:

| Gruppe | n | Trendline | R² | Ø Dienstjahre | Ø Urlaubsstunden |
|---|---|---|---|---|---|
| **Alle** | 111 | **y = −4,26x + 66,48** (negativ) | 0,20 | – | 41,5 |
| Junior | 56 | y = 0,56x + 23,48 (**positiv**) | 0,04 | 7,0 | 27,4 |
| Senior | 55 | y = 1,33x + 49,49 (**positiv**) | 0,01 | 4,7 | 55,7 |

- a) **Alle zusammen:** negative Beziehung, d. h. mehr Dienstjahre gehen mit **weniger** Urlaub einher.
- b) **Nach Junior/Senior getrennt:** **innerhalb jeder Gruppe positiver** (leicht steigender) Zusammenhang, also das **Gegenteil**.
- c) **Ja, Simpson's paradox**: Der Trend kehrt sich bei Aggregation um. **Lurking variable = Consultant title**: Seniors nehmen viel mehr Urlaub (Ø 55,7 h vs. 27,4 h), haben aber im Schnitt **weniger** Dienstjahre (4,7 vs. 7,0). Beim Zusammenwerfen entsteht so ein scheinbar negativer Trend. (Die Zusammenhänge sind insgesamt schwach, R² klein.)
- **Excel:** Scatter → Rechtsklick Punkt → *Add Trendline* → Linear, *Display Equation* + *R-squared*. Für b) nach Title sortieren und zwei Serien anlegen (*Select Data → Add*), je eine Trendline.

**Activity 4 – COVID-19 Positivity Rate Ohio**
- Problem (deine Notiz: „y-Achsen-Ratio passt nicht zur x-Achse"): **y-Achse 0–100 %**, obwohl die Werte nur zwischen **≈ 4,6 % und 14,5 %** liegen, dazu ein **flaches, breites** Chart (große Aspect ratio) → Trend ist unsichtbar.
- a) Verbesserungen: **y-Achse auf z. B. 0–16 %** beschränken, **Chart höher machen** (kleinere Aspect ratio), tägliche Schwankungen per **7-Tage-Moving-Average** glätten, aussagekräftiger Titel mit der Botschaft (z. B. „Positivity rate fell from ~12 % in April to under 5 % in October"), Gridlines reduzieren.
- b) Daten: Monatsdurchschnitt April 11,6 % → Mai 11,1 % → Juni 7,5 % → Juli 6,5 % → Aug 5,9 % → Sep 5,2 % → Okt 4,7 %; Maximum 14,5 % am 21.04.2020. **Klarer Abwärtstrend.**
- Hinweis: Line chart muss nicht bei 0 beginnen (Orientation-Attribut), 0 als Untergrenze ist hier aber auch ok.

**Activity 5 – Maximus Fashion Headcount vs. Revenue (Dual-axis)**
- Daten: Headcount (FTE) 14, 16, 18, 16, 12, 8, 10, 12 · Revenue $815k, 828k, 820k, 741k, 721k, 735k, 731k, 728k (Q1–Q8)
- a) **Verwirrung:** Das Publikum (wenig Erfahrung mit Data Vis) vergleicht die **Höhen beider Linien** direkt bzw. interpretiert **Schnittpunkte**, obwohl die Achsen unterschiedliche Einheiten/Skalen haben. Welche Achse zu welcher Linie gehört, ist unklar. Durch die Skalenwahl lässt sich eine beliebige (Schein-)Beziehung erzeugen.
- b) **Redesign:** **Zwei separate Line charts** untereinander mit **gleicher x-Achse (Quartale)**: oben Headcount (FTE), unten Revenue ($ Tausend), klare Titel mit Botschaft, direkte Labels, keine Sekundärachse. Alternative: beide auf **Index Q1 = 100** normieren und in einem Chart zeigen.
- Insight: Headcount fiel von 18 (Q3) auf 8 (Q6) und erholte sich auf 12. Der Umsatz fiel nach Q3 von ~$820k auf ~$730k und blieb trotz wieder steigender Mitarbeiterzahl **flach**.

### 9.6 Mögliche Prüfungsfragen Modul 10
- **Activity 1 (Java Cup):** fehlende und fehlerhafte Werte in einer Datei finden und benennen (Datei-Upload + Text) – **sehr wahrscheinlich!**
- **Activity 2:** Drei Studien den Bias-Typen zuordnen und begründen – **sehr wahrscheinlich!**
- **Activity 3:** Scatter chart + Trendline, dann nach Gruppe aufteilen, Simpson's paradox erklären.
- Selection bias, Survivor bias, Simpson's paradox definieren + eigenes Beispiel.
- Inflationsbereinigung berechnen (Formel!) und erklären, warum nötig.
- Irreführendes Chart erkennen (Achse nicht bei 0, Aspect ratio, Dual-axis, Temporal frequency, absolute Werte auf Karten) und Redesign vorschlagen.
- **Datei:** Ohio-Chart redesignen; Dual-axis-Chart in zwei Charts aufteilen.

<div style="page-break-after: always;"></div>

## 10. Anhang A – Excel-Anleitungen (Windows-Begriffe, Mac-Hinweise)

> **Mac-Excel:** Den „+"-Button (*Chart Elements*) gibt es auf dem Mac nicht. Stattdessen: Chart anklicken → Tab **Chart Design → Add Chart Element** (Titel, Achsentitel, Data Labels, Error Bars, Gridlines, Legend, Trendline). Formatieren: Rechtsklick → *Format …* öffnet die Seitenleiste. *PivotChart Analyze* heißt teils *PivotTable Analyze*.

**Grundsätzliches Chart-Cleanup (immer machen!)**
1. Aussagekräftigen Titel setzen (linksbündig, ggf. mit der Botschaft)
2. Achsentitel hinzufügen (mit Einheit); y-Titel horizontal oben an der Achse
3. Gridlines entfernen oder aufhellen, Chart-Rahmen entfernen (*Format Chart Area → Border → No line*)
4. Legende entfernen, wenn nur eine Serie; sonst direkte Labels
5. Einheitliche Sans-serif-Schrift; Achsenlinien dezent
6. Sinnvolle Achsengrenzen (Column/Bar ab 0)
7. Farben: eine Farbe, Hervorhebung gezielt

**Scatter chart + Trendline** (sehr prüfungsrelevant!)
1. x- und y-Spalte markieren (x **links**)
2. *Insert → Insert Scatter (X,Y) or Bubble Chart → Scatter*
3. Rechtsklick auf einen Datenpunkt → *Add Trendline* → **Linear** (oder Polynomial / Moving Average)
4. Im Format-Trendline-Pane: **Display Equation on chart** + **Display R-squared value on chart**
5. Achsenskalen: *Format Axis → Bounds Minimum/Maximum* knapp unter Min / über Max
6. Achsentitel, Titel, Gridlines entfernen; möglichst **quadratisch**
- **Mehrere Gruppen** (z. B. Junior/Senior): Daten nach Gruppe **sortieren** → Chart für Gruppe 1 → Rechtsklick *Select Data* → Series umbenennen → **Add** → Series name, X values, Y values für Gruppe 2 → je Serie eigene Trendline
- **Eine Gruppe hervorheben**: andere Serien *Format Data Series → Marker → Fill: No fill, Border grau*

**Column / Bar / Clustered / Stacked**: Daten markieren → *Insert → Insert Column or Bar Chart* → Typ wählen. Jahr-Problem: *Change Chart Type* bzw. *Select Data → Horizontal (Category) Axis Labels = Jahre*. Sortieren: Daten vorher sortieren (Data → Sort) oder bei PivotChart *Sort Largest to Smallest*.

**Line chart**: *Insert → Line or Area → Line (with Markers)*; bei numerischen x-Werten: *Scatter with Straight Lines and Markers*.

**Histogram**: Spalte markieren → *Insert → Insert Statistic Chart → Histogram* → *Format Axis → Bin width / Number of bins / Overflow/Underflow bin*. Alternativ `FREQUENCY` + Column chart (Gap width 0 %).

**Box & Whisker**: Spalten (unstacked) markieren → *Insert → Statistic Chart → Box and Whisker*; *Format Data Series*: Show mean markers, Show outlier points.

**Frequency distribution (kategorial)**: PivotTable (Feld in Rows **und** Values = Count) oder `=COUNTIF(Bereich;"Kategorie")`; Prozent: *Value Field Settings → Show Values As → % of Grand Total*.

**Strip chart / Jitter**: Gruppen sortieren, y-Hilfsspalte (10/20), Scatter, zweite Serie per *Select Data → Add*, Marker No fill, Jitter `=C2+RAND()` als neue Y-Werte.

**Error bars (Confidence interval)**: Column chart → *Chart Elements → Error Bars → More Options → Custom → Specify Value* → positive = negative = Zelle mit Margin of error (`=CONFIDENCE.T(0,05;s;n)`) → Textfeld „95 % confidence interval".

**Prediction-interval-Linien**: *Select Data → Add* für Prediction/Lower/Upper → *Change Series Chart Type → Scatter with Smooth Lines*; Beobachtungen: Line = No line, Marker automatic.

**Choropleth (Filled Map)**: Region + Wert markieren → *Insert → Maps → Filled Map* (Internet nötig). Farbe: *Format Data Series → Series Colour → Sequential (2-colour)* bzw. *Diverging (3-colour)*.

**Heat map**: Zahlenbereich markieren → *Home → Conditional Formatting → Color Scales → Blue-White-Red* (diverging) oder einfarbig (sequential).

**Treemap**: zuerst nach Kategorie **sortieren** → *Insert → Insert Hierarchy Chart → Treemap* → *Format Data Labels → Value*.

**Funnel**: *Insert → Insert Waterfall, Funnel, Stock, Surface or Radar Chart → Funnel*.

**Waterfall**: Zeilen (mit Strg/Cmd) markieren → *… → Waterfall* → Total-Säule doppelt anklicken (nur diesen Punkt) → *Format Data Point → **Set as total***.

**Stock (High-Low-Close)**: Datum + High, Low, Close (in dieser Reihenfolge) markieren → *… → Stock → High-Low-Close* → Data Labels → High/Low-Labels löschen → Close-Marker schwarz, 3 pt.

**Slope chart**: Bereich (Labels + 2 Spalten) markieren → *Insert → Line with Markers* → *Select Data → **Switch Row/Column*** → Gridlines, Legende und y-Achse entfernen → Data Labels rechts; links: Label → *Series Name* + Position Left.

**Dot matrix**: *Insert → Symbol → Geometric Shapes → ●* in Zelle → auf Matrix kopieren → Spaltenbreite verkleinern → *View → Gridlines* aus → Zellen mit Fill colour hinterlegen (Enclosure) → Titel/Legende („● = 1 million").

**BAN**: Textfeld (*Insert → Text Box*) mit großer, fetter Zahl neben das Chart.

**PivotChart + Slicers**: Zelle im Datenbereich → *Insert → PivotChart* (& PivotTable) → Felder in Values/Axis/Legend ziehen → *Change Chart Type* → *PivotChart Analyze → Insert Slicer* → Slicer formatieren (Columns-Anzahl) → *Hide All Field Buttons* → Achse *Display Units: Thousands*. **Connected slicer:** *Slicer → Report Connections*.

**Moving average trendline**: Rechtsklick Serie → *Add Trendline → Moving Average → Period = 3/4/6/12*.

**Sparklines**: Zielzelle → *Insert → Sparklines → Line* → Data range.

**Table lens**: nach Hauptvariable absteigend sortieren → jede Spalte *Conditional Formatting → Data Bars* (ggf. „Show Bar Only").

**Fehlende Werte / Fehler**: `=COUNTBLANK(Bereich)`, *Conditional Formatting → New Rule → Format only cells that contain → Blanks* (bzw. *Cell Value > 100 / < 0*), *Data → Sort/Filter*, `=MIN()`, `=MAX()`.

**Inflation**: `=B2*($C$41/C2)` → runterziehen → Line chart nominal vs. adjusted.

**Farbe exakt (HSL)**: *Format → Fill → Solid fill → Colour → More Colours → Custom → HSL*.

**Datei abgeben**: *File → Save As* → Dateityp **Excel Workbook (.xlsx)** → **umbenennen** wie gefordert → hochladen → Upload-Bestätigung prüfen.

<div style="page-break-after: always;"></div>

## 11. Anhang B – Formeln & Excel-Funktionen

| Zweck | Formel / Funktion |
|---|---|
| Relative frequency | Häufigkeit / n · Excel `=COUNTIF(...)/COUNTA(...)` |
| Percent frequency | Relative frequency × 100 |
| Approximate bin width | (Max − Min) / Anzahl Bins |
| Häufigkeiten in Bins | `=FREQUENCY(Daten; Bin-Obergrenzen)` |
| Mean / Median / Mode | `AVERAGE` / `MEDIAN` / `MODE.SNGL`, `MODE.MULT` |
| Range | `=MAX()−MIN()` |
| Standard deviation (sample) | `STDEV.S` |
| Percentile / Quartile | `PERCENTILE.EXC(Daten; 0,9)` / `QUARTILE.EXC(Daten; 1)` |
| IQR | Q3 − Q1 |
| Outlier-Grenzen | Q1 − 1,5 × IQR · Q3 + 1,5 × IQR |
| Empirical rule | 68 % (±1 SD) · 95 % (±2 SD) · 99,7 % (±3 SD) |
| Margin of error (Mean) | t × s/√n · `=CONFIDENCE.T(0,05; s; n)` |
| Margin of error (Proportion, 95 %) | 1,96 × √(p(1−p)/n) |
| Confidence interval | Schätzwert ± Margin of error |
| Correlation | `=CORREL(x; y)` (−1 … +1) |
| Inflationsbereinigung | Nominal(t) × Index(Basis) / Index(t) · `=B2*($C$41/C2)` |
| Prozentuale Veränderung | (Neu − Alt) / Alt |
| Fehlende Werte zählen | `=COUNTBLANK(Bereich)` |
| Jitter | `=Wert+RAND()` |
| Bin-Label | `=CONCAT("(";D6;",";E6;"]")` |

---

## 12. Anhang C – Antwort-Frameworks für Essay-Fragen

### „Critique this visualisation / How would you improve it?"
Gehe diese Checkliste durch und nenne pro Punkt **Problem → Auswirkung → Verbesserung**:
1. **Chart type** passend zu Ziel und Daten? (Pie → Bar, Area → Line, Dual-axis → 2 Charts, 3D → 2D)
2. **Axes** (Column/Bar ab 0? Skala zu weit/eng? Aspect ratio? Einheiten/Titel?)
3. **Colour** (unnötig, zu viel, zu wenig Kontrast, inkonsistent, farbenblind-tauglich, passendes Scheme?)
4. **Clutter / Data-ink ratio** (Gridlines, Rahmen, Legende, Hintergrund, Dezimalstellen)
5. **Eye travel** (Legende statt direkter Labels, Titel-Ausrichtung)
6. **Text** (Titel mit Botschaft, Sans-serif, Lesbarkeit)
7. **Audience** (needs + analytical comfort, passt die Komplexität?)
8. **Truthfulness** (Bias, fehlende Inflationsbereinigung, absolute statt relative Werte, Zeitraum-Auswahl)

### Definitions-Frage (z. B. 4 Punkte)
Definition (1) → Merkmal/Erklärung (1) → Beispiel (1) → Bedeutung für Data Vis/Entscheidungen (1)

### Vergleichs-Frage (A vs. B)
Tabelle im Kopf: Definition A / B → Wann A / Wann B → je ein Beispiel → Empfehlung für das konkrete Szenario

### Datei-Frage mit Interpretation
„The chart shows … (Trend/Richtung). The trendline equation y = …x + … indicates that for each additional unit of x, y changes by about … . R² = … means the relationship is weak/moderate/strong. However, correlation does not imply causation; a lurking variable such as … may explain …"

### Nützliche englische Formulierungen
- *"This reduces the cognitive load for the audience because …"*
- *"Humans are better at comparing lengths than angles or areas, so a bar chart is more effective than a pie chart."*
- *"This increases the data-ink ratio by removing non-data ink such as …"*
- *"Using the Gestalt principle of proximity/enclosure/similarity/connection, …"*
- *"The preattentive attribute of colour/size draws the audience's attention to …"*
- *"The distribution is left/right skewed, so the median is a better measure of central location than the mean."*
- *"Because the missingness is related to the value itself, the data are MNAR …"*
- *"When the data are disaggregated by …, the trend reverses, which is an example of Simpson's paradox."*
- *"A dual-axis chart invites misleading comparisons; two separate charts sharing the same horizontal axis are clearer."*

---

## 13. Anhang D – Glossar EN → DE

| EN | DE / Erklärung |
|---|---|
| Aspect ratio | Seitenverhältnis Breite : Höhe |
| BAN (Big Associated Number) | große hervorgehobene Kennzahl |
| Bin / class | Klasse/Intervall im Histogramm |
| Cartogram | Kartogramm (verzerrte Karte) |
| Choropleth map | Flächenkartogramm (eingefärbte Regionen) |
| Cognitive load | kognitive Belastung |
| Confidence interval | Konfidenzintervall |
| Correlation / causation | Korrelation / Kausalität |
| Cross-sectional data | Querschnittsdaten |
| Crosstabulation | Kreuztabelle |
| Data-ink ratio | Anteil datentragender „Tinte" |
| Declutter | entrümpeln |
| Drill-down | in Details hineinzoomen |
| Dual-axis chart | Diagramm mit zwei y-Achsen |
| Enclosure / proximity / similarity / connection | Umschließung / Nähe / Ähnlichkeit / Verbindung |
| Eye travel | Blickwege |
| Frequency polygon | Häufigkeitspolygon |
| Hue / saturation / luminance | Farbton / Sättigung / Helligkeit |
| Interquartile range (IQR) | Interquartilsabstand |
| Jittering | zufälliges Versetzen von Punkten |
| KPI | Leistungskennzahl |
| Lurking variable | versteckte Drittvariable (Confounder) |
| Margin of error | Fehlerspanne |
| Moving average | gleitender Durchschnitt |
| Occlusion | Überdeckung von Punkten |
| Preattentive attributes | vorbewusst wahrgenommene Merkmale |
| Prediction interval | Prognoseintervall |
| Price index | Preisindex (z. B. CPI) |
| Seasonality | Saisonalität |
| Skewness (left/right) | Schiefe (links-/rechtsschief) |
| Slicer | Datenschnitt (Filter-Buttons) |
| Sparkline | Mini-Diagramm in einer Zelle |
| Stacked / unstacked data | gestapelte / aufgeteilte Datenanordnung |
| Strip chart | Streifendiagramm (Einzelwerte) |
| Survivor bias | Survivorship-Bias |
| Table lens | Tabelle mit Balken |
| Temporal frequency | zeitliche Auflösung |
| Trellis display | Small Multiples |
| Waterfall chart | Wasserfalldiagramm |
