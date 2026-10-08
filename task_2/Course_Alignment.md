# Course Alignment — ICT702 concepts applied to the golf dashboard

Companion to `ICT702_Task2_Golf_Dashboard_v3.xlsx`.
Everything below maps to material in `module_2` to `module_8`, so the report can cite the course directly.

---

## 1. The four analytical goals (Module 3.2)

The course frames chart choice around a question, not a preference. Decide the goal first, then pick the chart.

| Goal | Question it answers | Charts the course endorses |
|---|---|---|
| **Composition** | What makes up the whole? | Stacked bar/column, treemap, **waterfall**, **funnel** |
| **Ranking** | What is the relative order? | **Sorted** bar or column chart |
| **Relationship** | How do two variables relate? | Scatter, bubble, line, heat map |
| **Distribution** | How are the items dispersed? | Histogram, frequency polygon, choropleth, scatter, box plot |

Comparison over time sits with relationship: Module 3 is explicit that line charts suit time series because connecting points implies continuity.

---

## 2. Chart selection matrix (Modules 3.4 and 8)

| Chart | Relationship | Distribution | Composition | Ranking | Use it when |
|---|:-:|:-:|:-:|:-:|---|
| Scatter | ● | ● | | | Two quantitative variables |
| Bubble | ● | ● | | | Three quantitative variables |
| Line | ● | | | | Time series, trends |
| Column | ● | ● | ● | ● | Categories; distribution **over time** |
| Bar | ● | ● | ● | ● | Long category labels; ranking when sorted |
| Heat map | ● | | | | Two categorical dimensions, magnitude by colour |
| Choropleth | | ● | | | Values across geography |
| Stacked bar/column | | | ● | ● | Parts plus the total |
| Treemap | | | ● | | Hierarchical composition |
| **Waterfall** | | | ● | | How a total is built up or eroded |
| **Funnel** | | | ● | | Drill-down through sequential stages |
| Histogram / frequency polygon | | ● | | | Distribution of one quantitative variable |
| Slope | ● | | | ● | Change between exactly two time points |
| Table | | | | | Exact values, mixed units or magnitudes |

**Avoid (Module 3.4):** pie charts (length beats angle and area), radar charts (use clustered column), area charts (use multiple line), combo charts (use two separate charts), any 3D chart.

---

## 3. What changed in the dashboard, and why

| # | Was | Now | Course basis |
|---|---|---|---|
| 3 | Uniform blue bars | **Diverging colour** at zero — losses orange, gains blue | Module 5: diverging scheme around a meaningful reference value |
| 5 | Alphabetical order, uniform blue | **Sorted descending**, orange below the national average | Module 3.4: ranking needs a sorted bar. Module 5: diverging at a reference value |
| 6 | All bars blue | **Highlight scheme** — Germany blue, all context grey | Module 5: "apply a different colour for the focus and grey for all others" |
| all | Excel gridlines | **Gridlines removed** | Module 4: data-ink ratio, decluttering |
| all | Generic titles | Headings that state the finding | Module 4: minimising eye travel |

Charts 1 and 4 were already correct — line charts for time series, applying the Gestalt principle of connection.

---

## 4. Two charts worth upgrading by hand

openpyxl cannot generate Excel's funnel and waterfall chart types, so the workbook ships bar-chart versions. Both are legitimate composition charts, but the course teaches the specialised types for exactly these cases, and building them yourself is two clicks and strengthens Criterion 2.

**Funnel chart** — sheet `07_Funnel`, the block headed *Ready for Excel's native Funnel chart*
Select the two-column range, then Insert → Insert Waterfall, Funnel, Stock, Surface or Radar Chart → Funnel.
This is Module 8, Activity 2, using the same menu path as the `DataScienceSearch` exercise.

**Waterfall chart** — sheet `11_Metrics`, section C
Select the two-column range, same menu → Waterfall. Right-click the Total bar → Set as Total.
Module 3.4: a waterfall visualises the composition of a quantitative variable over categories — which is exactly what the age-band change is.

---

## 5. Principles applied across the whole dashboard

**Pre-attentive attributes (Module 4)**
Colour carries meaning only — blue for male and volume, orange for female and shortfall. Every comparison is encoded as length, the attribute people judge most accurately; no angles or areas anywhere. Spatial position sets the reading order: state of play → opportunity → structural problem → where to act.

**Gestalt principles (Module 4)**
*Similarity* — identical colour encoding across all six charts. *Proximity* — KPI tiles form one band under the title; each chart sits under its own heading. *Enclosure* — filled title bar and KPI blocks separate the summary layer from the charts. *Connection* — lines join time-series markers so trends read as continuous.

**Data-ink ratio (Module 4)**
Gridlines, chart borders and decorative fills removed. Legends dropped wherever a single series or a direct label already identifies the data.

**Font (Module 4)**
Calibri throughout — sans-serif, which the module recommends for on-screen work because it stays legible at small sizes.

**Colour (Module 5)**
Two hues, well inside the six-colour ceiling for categorical schemes. Diverging schemes used twice, each around a meaningful reference value. Highlight scheme on the European benchmark. Blue #0072B2 and orange #E69F00 from Okabe-Ito stay separable under deuteranopia, protanopia and tritanopia — Module 5 names neglecting colourblindness as a common mistake. Colour encoding held constant across charts, mirroring the module's own adults/children worked example.

---

## 6. Preparation pipeline (Criterion 3 asks for all stages)

1. **Source selection** — ten DGV yearbooks as the primary series, Allensbach for latent demand, R&A for benchmarking, Destatis for denominators.
2. **Extraction** — tables read out of the published PDFs rather than retyped, removing transcription error as a failure mode.
3. **Validation** — for every year 2016–2025, four independently published figures reconcile exactly.
4. **Structuring** — wide tables kept in published shape for auditability; parallel long-format tables added so PivotTables need no restructuring.
5. **Derivation** — rates and shares as live formulas, not pasted values.
6. **Chart selection** — each visualisation matched to one of the four goals before a chart type was chosen.
7. **Design refinement** — decluttering, colour encoding, sorting and labelling as a deliberate pass; Module 4 names leaving Excel defaults as a common mistake.

---

## 7. Course reference for the report

Camm, J. D., Cochran, J. J., Fry, M. J., & Ohlmann, J. W. (2021). *Data visualization: Exploring and explaining with data* (1st ed.). Cengage.

This is the text the ICT702 lecture slides are drawn from, so citing it alongside Okabe & Ito covers the theory sections properly.
