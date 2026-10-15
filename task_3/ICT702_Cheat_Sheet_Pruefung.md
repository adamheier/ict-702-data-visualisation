# ICT702 – Cheat Sheet Task 3 (Module 2–10)

**Prüfung:** 90 Min · 5 Fragen · 40 Punkte (4 · 8 · 10 · 12 · 6) · kein Zurück · kein Copy & Paste · Antworten auf **Englisch**

| Q | Pkt | Zeit | fertig bis (Start 12:15) |
|---|---|---|---|
| 1 | 4 | 8′ | 12:23 |
| 2 | 8 | 17′ | 12:40 |
| 3 | 10 | 22′ | 13:02 |
| 4 | 12 | 26′ | 13:28 |
| 5 | 6 | 13′ | 13:41 (+4′ Puffer) |

- **1 Punkt ≈ 1 begründetes Argument.** Struktur: Antwort → Fachbegriff/Begründung → Bezug auf die Daten → Verbesserung
- **Datei-Frage:** bearbeiten → *Save As .xlsx* → **umbenennen** → hochladen → Upload prüfen → Interpretation ins Textfeld → erst dann weiter
- Technisches Problem → Screenshot mit Uhrzeit

---

## Modul 2 – Introducing Data Vis

- **Analytics** = Daten → Insights → bessere Entscheidungen. Wachstum durch: Technologie, Methoden, Rechen-/Speicherleistung
- **Descriptive** (was passierte: Reports, **Data Vis**, Dashboards) · **Diagnostic** (warum) · **Predictive** (was wird: Regression, Forecast) · **Prescriptive** (was tun: Optimierung, Simulation)
- **Warum visualisieren:** (1) explore (Muster, Beziehungen), (2) explain/communicate. **Anscombe:** gleiche Statistik, andere Muster → immer plotten
- **Quantitative** (Magnitude, rechnen möglich) vs. **categorical** (Labels) · **Cross-sectional** (ein Zeitpunkt) vs. **time series** (mehrere Zeitpunkte)
- **Big Data 4 V:** Volume, Velocity, Variety, Veracity
- **Benford:** 1 = 30,1 % · 2 = 17,6 · 3 = 12,5 · 4 = 9,7 · 5 = 7,9 · 6 = 6,7 · 7 = 5,8 · 8 = 5,1 · 9 = 4,6 % → Abweichung ⇒ Betrug prüfen
- Funktionsbereiche: Accounting = Benford-Clustered column · Finance = High-low-close · HR = stacked column · Marketing = funnel · Ops = line · Engineering = control chart · Science = spaghetti chart · Sports = shot chart

**Prüfungsfragen M2 (Kurzlösung)**
- Dashboard = descriptive · Produktionsplan min. Überstunden = prescriptive · Sales-Forecast = predictive · Bar chart = descriptive · Investment-Allokation = prescriptive
- Hauspreis vs. Fläche (75 Häuser, 1 Tag) = quantitative, cross-sectional, **scatter**
- Netflix 2010–19 = quantitative, time series, column chart
- Tucker vs. Benford: **5 & 9 überrepräsentiert** (≈ doppelt); **1 größte absolute** Unterrepräsentation (−4,6 pp); **7 größte relative** (≈ −31 %); 3/4 auch unter → untersuchen, kein Beweis

---

## Modul 3 – Selecting a Chart Type

**Ziele:** Composition · Ranking · Relationship · Distribution

| Chart | Rel. | Distr. | Comp. | Rank. |
|---|:-:|:-:|:-:|:-:|
| Scatter / Bubble | ✓ | ✓ | | |
| Line / Stock / Heat map | ✓ | | | |
| Column | ✓ | ✓ | | ✓ |
| Bar | ✓ | ✓ | ✓ | ✓ |
| Choropleth | | ✓ | | |
| Stacked bar/column, Treemap, Waterfall | | | ✓ | |
| Funnel | | | | ✓ |

- **Bar statt Column:** lange Kategorienamen, Rankings · **Column:** Zeit (links → rechts)
- **Stacked:** Part-to-whole + Total · **Clustered:** Serien vergleichen (wird schnell voll) · **Line:** Zeit, Kontinuität, Trend
- **Bubble** = Scatter + 3. Variable als Größe · **Treemap** = hierarchisch · **Waterfall** = kumulative +/− · **Funnel** = Stufen groß → klein
- **Table statt Chart:** exakte Werte, präzise Vergleiche, versch. Einheiten/Größenordnungen
- **Vermeiden:** Pie (→ Bar: Länge > Winkel), Radar (→ Clustered column), Area (→ Line), Combo/Dual-axis (→ 2 Charts), 3D (→ 2D)
- Excel: Jahr als Zahl → *Change Chart Type* / Jahr als Achsenbeschriftung

**Prüfungsfragen M3**
- Stacked > clustered (Cheetah): zeigt Regionsanteile **und** Gesamtumsatz, weniger Clutter. Line chart für Trendvergleich (Regionalmanager), stacked für Gesamtumsatz + Anteile (Geschäftsführung)
- NYC-Budget Bar > Pie: (1) Länge genauer als Winkel/Fläche, (2) viele Kategorien = viele Farben + Legende → Cognitive load; sortierbar. Bar > Column: lange Labels horizontal lesbar
- Anscombe: DS1 linear passt; DS2 gekrümmt → lineare Trendline falsch, trotz gleicher Gleichung/R² = 0,67

---

## Modul 4 – Design

- **Preattentive attributes** (iconic memory, ohne Anstrengung): **Colour** (hue, saturation, luminance) · **Form** (orientation, size, shape, length, width) · **Spatial positioning** · **Movement** (flicker, motion). Size wird schlecht geschätzt. Überbenutzung → Clutter
- Gedächtnis: iconic → short-term → long-term
- **Gestalt:** **Similarity** (gleiche Farbe/Form = Gruppe) · **Proximity** (nah = Gruppe) · **Enclosure** (Rahmen/Schattierung) · **Connection** (Linien; Forecast gestrichelt). Weitere: closure, continuation, symmetry
- **Data-ink ratio** = Daten-Tinte / Gesamt-Tinte → erhöhen = **declutter** (Gridlines, Rahmen, Legende, 3D, Hintergrund, Dezimalstellen weg; White space)
- **Eye travel minimieren:** Titel + y-Titel linksbündig an der y-Achse, Labels direkt ans Linienende, x-Titel am Achsenende
- **Tabellen:** Zahlen rechtsbündig, Text linksbündig, gleiche Dezimalstellen, große Zahlen runden
- **Schrift:** Sans-serif (Arial, Calibri, Verdana) für Data Vis; Serif (Times) für Druck; eine Schrift, Achsentitel gleich
- **Fehler:** falscher Chart-Typ, zu viel Info (→ separate Charts), Excel-Defaults, zu viele Attribute, 3D

**Prüfungsfragen M4**
- 7er zählen (neben hue/size): shape, orientation, width (bold), enclosure (Kasten), luminance (Rest grau), spatial offset, flicker
- Scarf Sales entfernen: Gridlines, Legende, Rahmen, „Chart Title" → hinzufügen: Titel, Achsentitel, Labels
- Snow: wärmer → weniger Schnee, negativ & nichtlinear, flacht bei 0 ab
- NYC: Attribut = **spatial positioning**; positive Beziehung % Graduates ↔ Rent (≠ Kausalität)

---

## Modul 5 – Colour

- **Hue** = Farbton (Primärfarben RGB) · **Saturation** = Grauanteil (0 % grau, 100 % rein) · **Luminance** = Schwarz/Weiß-Anteil (0 % schwarz, 100 % weiß) → Kontrast, Hierarchie
- **Psychology** (angeboren; cool = beruhigend/weiter weg, warm = Energie/Gefahr) vs. **Symbolism** (kulturell, ändert sich)
- **Complementary** (gegenüber, Kontrast/Dissonanz) vs. **analogous** (benachbart, harmonisch)
- **Schemes:** **Categorical** (ungeordnet, ≤ 6 Hues) · **Sequential** (1 Hue, Luminance-Gradient, geordnet) · **Diverging** (2 Hues, gemeinsamer Mittelpunkt = Referenzwert, z. B. 0) · **Highlight** (Rest grau)
- **HSL Excel** (0–255): Sat 0 = grau · Lum 0 = schwarz, 255 = weiß, 128 = reiner Farbton
- **6 Fehler:** unnecessary colour (→ 1 Farbe), excessive colour (→ Fokus farbig, Rest grau), insufficient contrast (→ Luminance-Differenz), inconsistency across charts, **colour-blindness** (Rot-Grün häufigste, Männer; → Blau/Orange + Labels), **mode of delivery** (Beamer: dick, scharf, hoher Kontrast/Sat/Lum; Druck: weicher, weniger Sat/Kontrast; testen!)

**Prüfungsfragen M5**
- Farbpaare: a Sat · b Lum · c Lum · d Hue · e Sat · f Lum
- Median income map = **sequential**, 1 Hue, hell = niedrig → dunkel = hoch
- Einkommens**veränderung** 2010 vs. 2020 = **diverging**, Mitte 0 % = weiß, Rot = Rückgang, Blau = Anstieg, dunkler = stärker (kein Rot-Grün)
- Heat map Same-store sales: Blue-White-Red; Austin durchgehend +, Phoenix/Seattle + → −, Cincinnati/St. Louis − → +
- ManagementTop25: meiste Firmen = **Technology (12)**, höchster Score = **Amazon**

---

## Modul 6 – Variability

- **Random variable**, **variation**, **sample** vs. population, **frequency distribution**
- Relative freq. = f/n · Percent = ×100 (≈ Wahrscheinlichkeitsverteilung) · kategorial sortieren, **ordinal nicht**
- **Histogram:** 5–20 Bins, gleiche Breite ≈ (Max − Min)/Bins, alle Werte genau 1 Bin; **(17, 25]** = 17 nicht drin, 25 drin
- **Skew:** left = Schwanz links, **Mean < Median** (Sterbealter, leichte Prüfung) · right = **Mean > Median** (Hauspreise, Einkommen) · symmetric (Körpergröße)
- **Mean** (`AVERAGE`, ausreißeranfällig) · **Median** (`MEDIAN`, bei Schiefe besser) · **Mode** (`MODE.SNGL/MULT`) · **Range** (Max − Min) · **SD = Standard Deviation (Standardabweichung)** (`STDEV.S`, nur bei symmetrisch) · **Percentile** (`PERCENTILE.EXC`) · **Q1/Q2/Q3** · **IQR = Q3 − Q1**
- **Empirical rule:** 68 / 95 / 99,7 % in ±1/2/3 SD
- **Box plot:** Box Q1–Q3, Linie = Median, X = Mean, **Outlier < Q1 − 1,5·IQR oder > Q3 + 1,5·IQR**
- **Frequency polygon** (Linien statt Säulen, Vergleich) · **Trellis** (gleiche Skalen) · **Strip chart** (Einzelwerte) → **Occlusion** → hohle Marker + **Jitter** `=C2+RAND()` · **Violin** = Box + Density
- **CI** = Schätzung ± **Margin of error**; MoE ↓ mit n↑, ↑ mit s↑, ↑ mit Konfidenz↑ · `=CONFIDENCE.T(0,05;s;n)` · Proportion: 1,96·√(p(1−p)/n)
- CI enthält 0 → keine Aussage über Vorzeichen; ganz > 0 → positiv mit 95 %
- **Prediction interval** (zukünftiger Einzelwert) > CI; wird **breiter, je weiter in die Zukunft** bzw. je weiter x vom Mittel
- **Independent (x, Ursache)** vs. **dependent (y, Wirkung)**

**Prüfungsfragen M6**
- Skewness: Sterbealter left · easy exam left · Hauspreise right · Männergröße symmetric
- % of grand total vs. count: % vergleicht Anteile unabhängig von n
- Linksschiefe aus Statistik: Mean < Median, Median − Q1 > Q3 − Median, unterer Whisker länger
- Box plot Vergleich: Median (Lage), IQR (Streuung), Whisker (Schiefe), Ausreißer
- **Datei:** Histogram, Box & whisker, strip/jitter, error bars

---

## Modul 7 – Exploring Data (EDA)

- **EDA-Ziele:** Fehler/Lücken/Ausreißer finden · Verteilung einzelner Variablen · Muster/Beziehungen. **Tall** = viele Zeilen, **wide** = viele Spalten
- Univariate (PivotTable/-Chart, Histogram, Box plot) → multivariate (**crosstab**, Slicers, Scatter)
- Ausreißer untersuchen, **nicht grundlos löschen** (reduziert Variabilität)
- **Scatter:** quadratisch, Achsen knapp unter Min / über Max, Trendline; **r ∈ [−1, +1]**, nahe Linie = stark, ~0 = kein linearer (evtl. nichtlinear!)
- **Spurious:** lurking variable, biased sample, zu wenige Daten · **Correlation ≠ causation**
- **Scatter-chart matrix** (alle Paare) · **Table lens** (Balken; nach Variable sortieren: groß → klein = positiv, klein → groß = negativ, kein Muster = keine)
- **Missing:** legitimate (natürlich) vs. illegitimate (Verweigerung, Abbruch, Sensor). Optionen: Zeilen löschen · schätzen/imputieren · eigene Kategorie
  - **MCAR** = hängt mit nichts zusammen · **MAR** = hängt mit **anderer** Variable zusammen · **MNAR** = hängt mit **eigenem Wert** zusammen
- **Time series:** Trend · Variability · Seasonality (1 Linie pro Jahr). **Temporal frequency** niedrig = glättet. **Moving average** (nur Vergangenheit, nicht ferne). Stacked (1 Spalte + Gruppenspalte) vs. unstacked (Spalte pro Gruppe). **Sparkline** = Trend ohne Magnitude in Zelle
- **Choropleth:** gut für relative Vergleiche/High-level, aber große Flächen dominieren, Granularität, besser **Raten/Dichte** · **Cartogram:** Fläche ∝ Wert (kann unkenntlich werden) · **Equal-area cartogram:** gleiche Flächen, Farbe = Wert

**Prüfungsfragen M7**
- Bildung fehlt bei niedriger Bildung = **MNAR** · Job-Titel fehlt eher bei Männern = **MAR**
- Rotwein → keine Kausalität (Beobachtungsstudie, lurking: Einkommen/Bildung) → **randomised controlled experiment**/für Confounder kontrollieren
- Körperfett vs. Exertion 1–4 (ordinal) → **Box plots je Level** / jittered strip (Scatter = Occlusion)
- Wide data (Dutzende Variablen) → table lens / scatter-chart matrix / Korrelations-Heatmap
- Queens hervorheben: Rest grau, eigene Trendline → Beziehung in Queens **schwächer**
- Annual (Trend) vs. quarterly (Saison) vs. monthly (Detail/Rauschen)

---

## Modul 8 – Explaining & Storytelling

- **Audience:** Needs (high-level vs. detailed) × analytical comfort (low vs. high)
  - Low/high-level: simple bar/column, line, summary tables, dot matrix, BAN · Low/detailed: clustered/stacked, crosstabs
  - High/detailed: **scatter**, box & whisker, histogram, strip, violin, Sankey, scatter matrix
  - Chan Life: Sales agents = Line (high-level) · Underwriters = clustered column (detailed) · Hospital: low comfort = column, high = box plot
- **Decision maker:** viele Faktoren, Stakeholder, unvollständige Infos, Zeitdruck → klar, hohe Data-ink ratio
- **Empathie-Probleme:** (1) große Zahlen → vertraut umrechnen, keine 10⁹-Notation, Dot matrix mit Kontext; (2) Aggregation → Persona, Einzelfall, Bild
- **Slope chart** = Veränderung zwischen 2 Zeitpunkten je Entität (Line with markers → **Switch Row/Column**) · **BAN** = Size · Farbe hebt eine Linie hervor
- **Rhetorical triangle:** **Ethos** (Glaubwürdigkeit: Quelle, Annahmen, nichts verzerren) · **Pathos** (Emotion/Empathie) · **Logos** (Logik der Argumentation)
- **Freytag:** Introduction → Rising action → Climax → Falling action (Empfehlungen) → Conclusion (Kosten/Nutzen, Limitationen). **Nicht chronologisch nach Analyseschritten!**
- **Story:** Set-up → Conflict → Resolution · **SCQA:** Situation, Complication, Question, Answer
- **Storyboard:** Sticky notes (flexibel, methodisch) vs. PowerPoint **Slide sorter**, getrennt von finaler Präsentation

**Prüfungsfragen M8**
- Opening Horizons: Durango 341 → 432 (+27 %, neue Nr. 1), Salida 395 → 360 (−9 %), Rest ~stabil
- ESU: alle ↑; Electrical +35 % (überholt Computer), Civil +15 % (wird Letzter), Chemical bleibt Top
- Dot matrix 40 Mio. Jobs: 20×20, ● = 100.000, Ohio ≈ 58 Punkte (≈ 7×) · Wasser 663 Mio.: 25×26 + 13, ● = 1 Mio., USA 330 ● schattiert = **Enclosure**, BAN „663 million"
- Funnel auch für: Sales pipeline, Website-Conversion, Recruiting, Onboarding
- Air Transat Freytag: Intro (Juli 2017, Umleitung Ottawa, Persona) → Rising (> 4 h Rollfeld, kein Essen/Wasser/Klima) → **Climax (911-Anruf, Medien)** → Falling (CTA-Verfahren, Schuld hin und her, Strafe) → Conclusion (Empfehlungen, Kosten/Nutzen)
- Chan Life Alternative: multiple line chart, Labels am Linienende, Prognose gestrichelt

---

## Modul 9 – Dashboards

- **Dashboard** = Vis-Tool mit mehreren Outputs, ggf. Echtzeit, zeigt **KPIs** zum „moment of value"
- **Prinzipien:** alle KPIs eines Bereichs auf **1 Screen**, lieber mehrere Dashboards als scrollen, KPIs klar und entscheidungsrelevant, Design-Prinzipien, Farbe sparsam
- **Taxonomien:** **Static** (billig, manuell, langsame KPIs) vs. **Dynamic** (automatisch, schnelle KPIs) · **Non-interactive** vs. **Interactive** (drill-down, hierarchical filtering, time-interval widget, customisation) · **Operational** (untere Manager, Echtzeit) · **Tactical** (mittlere, Stärken/Schwächen, Strategie) · **Strategic** (Executives, übergeordnete Ziele) · **Analytical** (Analysten, Trends, Prognosen)
- **Design:** Purpose · User needs (User einbeziehen!) · Display (Chart-Typ, Layout, Gerät/Licht/Auflösung) · **Context** (über Zeit, vs. Ziel, intern/extern) · Engineering (Eye travel, Wartung, Zukunft) · Daten in separatem Blatt, User keine Änderungen · **Testing**
- **Fehler:** Org-Ziele/User ignoriert · Umgebung ignoriert · falsche Positionierung · falscher Chart-Typ · Design-Prinzipien ignoriert · zu voll/zu leer · unattraktiv · Zukunft ignoriert
- **Excel:** PivotTable, PivotChart, **Slicers**, **Report Connections** (1 Slicer → mehrere Charts), Hide Field Buttons, Protect Sheet
- **EJB:** tactical, dynamic & interactive · KPIs = total $ sales + avg. delivery time

**Prüfungsfragen M9**
- Gelbes EJB-Dashboard verbessern: neutraler Hintergrund, Sans-serif-Titel, größere Charts, kompakte/verbundene Slicer neben Charts, konsistente Farben, Zusammengehöriges nebeneinander
- Service vs. Product satisfaction je DC × Jahr → **Scatter** (Punkt = DC) als **Trellis pro Jahr** oder Farbe pro Jahr + PivotTable; mit Year-Slicer verbinden
- Manufacturing-KPIs: OEE, Ausschussquote, First-pass yield, Auslastung, Zykluszeit, Termintreue, Lagerumschlag, Kosten/Einheit, Unfälle, Energie, MTBF, Rüstzeit

---

## Modul 10 – Telling the Truth

- **Erst Missing, dann Errors.** Missing: **Sort**, **Conditional Formatting (Blanks)**, **`=COUNTBLANK()`**, Filter. Errors: **MIN/MAX**/Summary stats, Sort, Frequency, Histogram, **Scatter** (auch nicht-extreme). Mehrere Methoden kombinieren (Blakely: 601 → 60,1 Monate)
- **Selection bias:** nicht-zufällige Stichprobe (Festnetz-Umfrage) · **Simpson's paradox:** Trend in Teilgruppen **kehrt sich bei Aggregation um** (Scatter nach Gruppe färben!) · **Survivor bias:** nur „Überlebende"/positive Ausgänge (WWII-Flugzeuge: Stellen **ohne** Löcher panzern)
- Meine Notiz: selection, survivor (*brilliance bias*), Simpson's (*confirmation bias*)
- **Inflation:** **Real(t) = Nominal(t) × Index(Basis) / Index(t)** · `=B2*($C$41/C2)` · 0,65 × 211,8/51,9 ≈ $2,65 (Folie: $2,66)
- **Achsen:** Column/Bar **ab 0** (sonst übertrieben); Line/Scatter enger ok (zu weit versteckt Trend). **Aspect ratio:** hoch & schmal übertreibt, flach & breit versteckt
- **Dual-axis** → falsche Vergleiche/Schnittpunkte → **2 separate Charts** (gleiche x-Achse)
- **Temporal frequency/Zeitraum:** niedrige Frequenz glättet, Cherry picking
- **Karten:** **Raten statt absolute Zahlen** (Poverty rate statt Anzahl Armer)

**Prüfungsfragen M10 (wahrscheinlich!)**
- **A1 Java Cup:** COUNTBLANK + Conditional Formatting (Blanks) → Befragte & Variable nennen; MIN/MAX/Sort/Filter, Werte < 0 oder > 100 = Fehler
- **A2 Bias:** (1) Rhine/Telepathie = **Survivor** (nur Gewinner jeder Runde, Zufall bei 500 Teilnehmern) · (2) Exit poll vor Restaurant nachts = **Selection** (nicht repräsentativ, Lobby) · (3) Rotwein-Kohorte = **Simpson's paradox** (Einkommen/Bildung als Lurking variable; disaggregiert kann sich der Effekt umkehren)
- **A3 Guaraldi:** alle: **y = −4,26x + 66,48** (R² 0,20, negativ) · Junior: y = 0,56x + 23,48 (+) · Senior: y = 1,33x + 49,49 (+) → **Simpson's paradox**; Lurking = Titel (Seniors Ø 55,7 h Urlaub bei Ø 4,7 Jahren; Juniors 27,4 h bei 7,0 Jahren)
- **A4 Ohio:** y-Achse 0–100 % bei Werten 4,6–14,5 % + flaches Chart versteckt Trend → y auf ~0–16 %, höheres Chart, 7-Tage-MA, Titel mit Botschaft; Trend: ~12 % (Apr) → < 5 % (Okt)
- **A5 Maximus:** Dual-axis verwirrt (Höhen/Schnittpunkte bedeutungslos, Skalen willkürlich, Laien) → 2 Line charts untereinander (Headcount, Revenue) gleiche Quartalsachse; Headcount 18 → 8 → 12, Revenue ~$820k → ~$730k flach

---

## Excel Quick Steps (Mac: *Chart Design → Add Chart Element* statt „+")

- **Scatter + Trendline:** x/y markieren → *Insert → Scatter* → Rechtsklick Punkt → *Add Trendline → Linear* → ☑ *Display Equation* ☑ *R-squared* → Achsen-Bounds anpassen, Titel/Achsentitel, Gridlines weg
- **Gruppen im Scatter:** sortieren → *Select Data → Add* (Name, X values, Y values) → je Serie Trendline; Hervorheben: andere Serien grau/No fill
- **Histogram / Box plot:** *Insert → Statistic Chart* · **Treemap:** sortieren → *Hierarchy Chart* · **Filled Map:** *Insert → Maps*
- **Heat map:** *Conditional Formatting → Color Scales* · **Blanks:** *CF → New Rule → Format only cells that contain → Blanks* · `=COUNTBLANK()`
- **Waterfall:** Total → *Format Data Point → Set as total* · **Funnel/Stock:** *Insert → Waterfall, Funnel, Stock …*
- **Slope:** Line with markers → *Switch Row/Column* → Gridlines/Legende/y-Achse weg, Labels links (Series Name) + rechts
- **Error bars:** *Error Bars → More Options → Custom → Specify Value* (= MoE)
- **Moving average:** *Add Trendline → Moving Average → Period* · **Sparklines:** *Insert → Sparklines*
- **PivotChart + Slicer:** *Insert → PivotChart* → Felder ziehen → *Insert Slicer* → *Report Connections* · Achse *Display units: Thousands*
- **% Häufigkeit:** *Value Field Settings → Show Values As → % of Grand Total*
- **Inflation:** `=B2*($C$41/C2)` · **Jitter:** `=C2+RAND()` · **Prozentänderung:** (neu − alt)/alt
- **Cleanup immer:** Titel (Botschaft), Achsentitel + Einheit, Gridlines/Rahmen/Legende weg, Sans-serif, Column/Bar ab 0

---

## Antwort-Checkliste „Critique / Improve this chart"

1. **Chart type** passend? (Pie → Bar, Area → Line, Dual-axis → 2 Charts, 3D → 2D)
2. **Axes:** ab 0 (Bar/Column)? Skala/Aspect ratio? Titel/Einheiten?
3. **Colour:** unnötig/zu viel/Kontrast/konsistent/farbenblind/richtiges Scheme?
4. **Clutter:** Data-ink ratio, Gridlines, Rahmen, Legende
5. **Eye travel:** direkte Labels, Titel-Ausrichtung
6. **Audience:** needs + analytical comfort
7. **Truth:** Bias, Inflation, absolute vs. relative Werte, Zeitraum

**Phrasen:** *reduces cognitive load* · *increases the data-ink ratio* · *humans compare lengths more accurately than angles/areas* · *Gestalt principle of proximity/enclosure* · *the preattentive attribute of colour draws attention to* · *correlation does not imply causation – a lurking variable such as …* · *when disaggregated, the trend reverses (Simpson's paradox)* · *two separate charts sharing the same x-axis*
