# ICT702 – Cheat Sheet Task 3 (Modules 2–10)

**Exam:** 90 min · 5 questions · 40 marks (4 · 8 · 10 · 12 · 6) · no going back · no copy & paste

| Q | Marks | Time | done by (start 12:15) |
|---|---|---|---|
| 1 | 4 | 8′ | 12:23 |
| 2 | 8 | 17′ | 12:40 |
| 3 | 10 | 22′ | 13:02 |
| 4 | 12 | 26′ | 13:28 |
| 5 | 6 | 13′ | 13:41 (+4′ buffer) |

- **1 mark ≈ 1 justified point.** Structure: answer → technical term/reason → reference to the data → improvement
- **File question:** edit → *Save As .xlsx* → **rename** → upload → check upload → interpretation in text box → only then move on
- Technical problem → screenshot with the time visible

---

## Module 2 – Introducing Data Vis

- **Analytics** = data → insights → better decisions. Growth driven by: technology, methods, computing power/storage
- **Descriptive** (what happened: reports, **data vis**, dashboards) · **Diagnostic** (why) · **Predictive** (what will happen: regression, forecast) · **Prescriptive** (what to do: optimisation, simulation)
- **Why visualise:** (1) explore (patterns, relationships), (2) explain/communicate. **Anscombe:** same statistics, different patterns → always plot
- **Quantitative** (magnitude, arithmetic possible) vs. **categorical** (labels) · **Cross-sectional** (one point in time) vs. **time series** (several points in time)
- **Big data 4 Vs:** volume, velocity, variety, veracity
- **Benford:** 1 = 30.1 % · 2 = 17.6 · 3 = 12.5 · 4 = 9.7 · 5 = 7.9 · 6 = 6.7 · 7 = 5.8 · 8 = 5.1 · 9 = 4.6 % → deviation ⇒ investigate fraud
- By function: accounting = Benford clustered column · finance = high-low-close · HR = stacked column · marketing = funnel · ops = line · engineering = control chart · science = spaghetti chart · sports = shot chart

**Exam questions M2 (short answers)**
- Dashboard = descriptive · production schedule min. overtime = prescriptive · sales forecast = predictive · bar chart = descriptive · investment allocation = prescriptive
- House price vs. size (75 houses, 1 day) = quantitative, cross-sectional, **scatter**
- Netflix 2010–19 = quantitative, time series, column chart
- Tucker vs. Benford: **5 & 9 over-represented** (≈ double); **1 largest absolute** under-representation (−4.6 pp); **7 largest relative** (≈ −31 %); 3/4 also under → investigate, not proof

---

## Module 3 – Selecting a Chart Type

**Goals:** composition · ranking · relationship · distribution

| Chart | Rel. | Distr. | Comp. | Rank. |
|---|:-:|:-:|:-:|:-:|
| Scatter / Bubble | ✓ | ✓ | | |
| Line / Stock / Heat map | ✓ | | | |
| Column | ✓ | ✓ | | ✓ |
| Bar | ✓ | ✓ | ✓ | ✓ |
| Choropleth | | ✓ | | |
| Stacked bar/column, Treemap, Waterfall | | | ✓ | |
| Funnel | | | | ✓ |

- **Bar instead of column:** long category names, rankings · **Column:** time (left → right)
- **Stacked:** part-to-whole + total · **Clustered:** compare series (gets crowded) · **Line:** time, continuity, trend
- **Bubble** = scatter + 3rd variable as size · **Treemap** = hierarchical · **Waterfall** = cumulative +/− · **Funnel** = stages large → small
- **Table instead of chart:** exact values, precise comparisons, different units/magnitudes
- **Avoid:** pie (→ bar: length > angle), radar (→ clustered column), area (→ line), combo/dual-axis (→ 2 charts), 3D (→ 2D)
- Excel: year plotted as a number → *Change Chart Type* / set year as axis labels

**Exam questions M3**
- Stacked > clustered (Cheetah): shows regional shares **and** total sales, less clutter. Line chart for comparing trends (regional managers), stacked for total + shares (senior management)
- NYC budget bar > pie: (1) length more accurate than angle/area, (2) many categories = many colours + legend → cognitive load; sortable. Bar > column: long labels readable horizontally
- Anscombe: DS1 linear fits; DS2 curved → linear trendline wrong, despite same equation/R² = 0.67

---

## Module 4 – Design

- **Preattentive attributes** (iconic memory, no conscious effort): **colour** (hue, saturation, luminance) · **form** (orientation, size, shape, length, width) · **spatial positioning** · **movement** (flicker, motion). Size is estimated poorly. Overuse → clutter
- Memory: iconic → short-term → long-term
- **Gestalt:** **similarity** (same colour/shape = group) · **proximity** (close = group) · **enclosure** (box/shading) · **connection** (lines; forecast dashed). Others: closure, continuation, symmetry
- **Data-ink ratio** = data ink / total ink → increase = **declutter** (remove gridlines, border, legend, 3D, background, decimals; white space)
- **Minimise eye travel:** title + vertical-axis title left-aligned with the axis, labels at the end of lines, horizontal-axis title at the end of the axis
- **Tables:** numbers right-aligned, text left-aligned, same decimals, round large numbers
- **Fonts:** sans-serif (Arial, Calibri, Verdana) for data vis; serif (Times) for print; one font, axis titles identical
- **Mistakes:** wrong chart type, excessive information (→ separate charts), Excel defaults, too many attributes, 3D

**Exam questions M4**
- Counting 7s (besides hue/size): shape, orientation, width (bold), enclosure (box), luminance (rest grey), spatial offset, flicker
- Scarf Sales remove: gridlines, legend, border, "Chart Title" → add: title, axis titles, labels
- Snow: warmer → less snow, negative & nonlinear, levels off at 0
- NYC: attribute = **spatial positioning**; positive relationship % graduates ↔ rent (≠ causation)

---

## Module 5 – Colour

- **Hue** = base colour (primary RGB) · **Saturation** = amount of grey (0 % grey, 100 % pure) · **Luminance** = amount of black/white (0 % black, 100 % white) → contrast, hierarchy
- **Psychology** (innate; cool = calming/distant, warm = energy/danger) vs. **symbolism** (cultural, changes over time)
- **Complementary** (opposite, contrast/dissonance) vs. **analogous** (adjacent, harmonious)
- **Schemes:** **categorical** (unordered, ≤ 6 hues) · **sequential** (1 hue, luminance gradient, ordered) · **diverging** (2 hues, shared midpoint = reference value, e.g. 0) · **highlight** (rest grey)
- **HSL in Excel** (0–255): Sat 0 = grey · Lum 0 = black, 255 = white, 128 = pure hue
- **6 mistakes:** unnecessary colour (→ 1 colour), excessive colour (→ focus in colour, rest grey), insufficient contrast (→ luminance difference), inconsistency across charts, **colour-blindness** (red-green most common, men; → blue/orange + labels), **mode of delivery** (projector: thick, sharp, high contrast/sat/lum; print: softer, less sat/contrast; test!)

**Exam questions M5**
- Colour pairs: a sat · b lum · c lum · d hue · e sat · f lum
- Median income map = **sequential**, 1 hue, light = low → dark = high
- Income **change** 2010 vs. 2020 = **diverging**, midpoint 0 % = white, red = decrease, blue = increase, darker = larger (no red-green)
- Same-store sales heat map: blue-white-red; Austin always +, Phoenix/Seattle + → −, Cincinnati/St. Louis − → +
- ManagementTop25: most companies = **Technology (12)**, highest score = **Amazon**

---

## Module 6 – Variability

- **Random variable**, **variation**, **sample** vs. population, **frequency distribution**
- Relative freq. = f/n · percent = ×100 (≈ probability distribution) · sort categorical, **not ordinal**
- **Histogram:** 5–20 bins, equal width ≈ (max − min)/bins, every value in exactly 1 bin; **(17, 25]** = 17 excluded, 25 included
- **Skew:** left = tail left, **mean < median** (age at death, easy exam) · right = **mean > median** (house prices, income) · symmetric (height)
- **Mean** (`AVERAGE`, outlier-sensitive) · **median** (`MEDIAN`, better for skew) · **mode** (`MODE.SNGL/MULT`) · **range** (max − min) · **SD = standard deviation** (`STDEV.S`, symmetric only) · **percentile** (`PERCENTILE.EXC`) · **Q1/Q2/Q3** · **IQR = Q3 − Q1**
- **Empirical rule:** 68 / 95 / 99.7 % within ±1/2/3 SD
- **Box plot:** box Q1–Q3, line = median, X = mean, **outlier < Q1 − 1.5·IQR or > Q3 + 1.5·IQR**
- **Frequency polygon** (lines instead of columns, comparison) · **trellis** (same scales) · **strip chart** (individual values) → **occlusion** → hollow markers + **jitter** `=C2+RAND()` · **violin** = box + density
- **CI** = estimate ± **margin of error**; MoE ↓ as n↑, ↑ as s↑, ↑ as confidence↑ · `=CONFIDENCE.T(0.05, s, n)` · proportion: 1.96·√(p(1−p)/n)
- CI contains 0 → no conclusion about the sign; entirely > 0 → positive with 95 %
- **Prediction interval** (future individual value) > CI; gets **wider the further into the future** or the further x is from its mean
- **Independent (x, cause)** vs. **dependent (y, effect)**

**Exam questions M6**
- Skewness: age at death left · easy exam left · house prices right · male height symmetric
- % of grand total vs. count: % compares shares independent of n
- Left skew from statistics: mean < median, median − Q1 > Q3 − median, lower whisker longer
- Comparing box plots: median (location), IQR (spread), whiskers (skew), outliers
- **File:** histogram, box & whisker, strip/jitter, error bars

---

## Module 7 – Exploring Data (EDA)

- **EDA objectives:** find errors/gaps/outliers · distribution of individual variables · patterns/relationships. **Tall** = many rows, **wide** = many columns
- Univariate (PivotTable/-Chart, histogram, box plot) → multivariate (**crosstab**, slicers, scatter)
- Investigate outliers, **don't delete without good cause** (reduces variability)
- **Scatter:** square, axes slightly below min / above max, trendline; **r ∈ [−1, +1]**, close to line = strong, ~0 = no linear relationship (maybe nonlinear!)
- **Spurious:** lurking variable, biased sample, too few data · **correlation ≠ causation**
- **Scatter-chart matrix** (all pairs) · **table lens** (bars; sort by one variable: large → small = positive, small → large = negative, no pattern = none)
- **Missing:** legitimate (natural) vs. illegitimate (refusal, dropout, sensor). Options: discard rows · estimate/impute · separate category
  - **MCAR** = related to nothing · **MAR** = related to **another** variable · **MNAR** = related to **its own value**
- **Time series:** trend · variability · seasonality (1 line per year). **Temporal frequency** low = smooths. **Moving average** (past only, not distant past). Stacked (1 column + group column) vs. unstacked (column per group). **Sparkline** = trend without magnitude in a cell
- **Choropleth:** good for relative comparisons/high-level, but large areas dominate, granularity issues, better **rates/density** · **Cartogram:** area ∝ value (can become unrecognisable) · **Equal-area cartogram:** equal areas, colour = value

**Exam questions M7**
- Education missing for low education = **MNAR** · job title missing more for men = **MAR**
- Red wine → no causation (observational study, lurking: income/education) → **randomised controlled experiment**/control for confounders
- Body fat vs. exertion 1–4 (ordinal) → **box plots per level** / jittered strip (scatter = occlusion)
- Wide data (dozens of variables) → table lens / scatter-chart matrix / correlation heat map
- Highlight Queens: rest grey, own trendline → relationship in Queens **weaker**
- Annual (trend) vs. quarterly (seasonality) vs. monthly (detail/noise)

---

## Module 8 – Explaining & Storytelling

- **Audience:** needs (high-level vs. detailed) × analytical comfort (low vs. high)
  - Low/high-level: simple bar/column, line, summary tables, dot matrix, BAN · Low/detailed: clustered/stacked, crosstabs
  - High/detailed: **scatter**, box & whisker, histogram, strip, violin, Sankey, scatter matrix
  - Chan Life: sales agents = line (high-level) · underwriters = clustered column (detailed) · hospital: low comfort = column, high = box plot
- **Decision maker:** many factors, stakeholders, incomplete info, time pressure → clear, high data-ink ratio
- **Empathy challenges:** (1) large numbers → convert to something familiar, no 10⁹ notation, dot matrix with context; (2) aggregation → persona, individual case, picture
- **Slope chart** = change between 2 points in time per entity (line with markers → **Switch Row/Column**) · **BAN** = size · colour highlights one line
- **Rhetorical triangle:** **ethos** (credibility: source, assumptions, nothing distorted) · **pathos** (emotion/empathy) · **logos** (logic of the argument)
- **Freytag:** introduction → rising action → climax → falling action (recommendations) → conclusion (costs/benefits, limitations). **Not chronological by analysis steps!**
- **Story:** set-up → conflict → resolution · **SCQA:** situation, complication, question, answer
- **Storyboard:** sticky notes (flexible, methodical) vs. PowerPoint **slide sorter**, separate from the final presentation

**Exam questions M8**
- Opening Horizons: Durango 341 → 432 (+27 %, new no. 1), Salida 395 → 360 (−9 %), rest ~stable
- ESU: all ↑; Electrical +35 % (overtakes Computer), Civil +15 % (becomes last), Chemical stays top
- Dot matrix 40 m jobs: 20×20, ● = 100,000, Ohio ≈ 58 dots (≈ 7×) · water 663 m: 25×26 + 13, ● = 1 m, USA 330 ● shaded = **enclosure**, BAN "663 million"
- Funnel also for: sales pipeline, website conversion, recruiting, onboarding
- Air Transat Freytag: intro (July 2017, diversion to Ottawa, persona) → rising (> 4 h on tarmac, no food/water/AC) → **climax (911 call, media)** → falling (CTA hearing, blame-shifting, fine) → conclusion (recommendations, costs/benefits)
- Chan Life alternative: multiple line chart, labels at line ends, projections dashed

---

## Module 9 – Dashboards

- **Dashboard** = vis tool with multiple outputs, possibly real-time, shows **KPIs** at the "moment of value"
- **Principles:** all KPIs of one area on **1 screen**, several dashboards rather than scrolling, KPIs clear and decision-relevant, design principles, colour used judiciously
- **Taxonomies:** **static** (cheap, manual, slow KPIs) vs. **dynamic** (automatic, fast KPIs) · **non-interactive** vs. **interactive** (drill-down, hierarchical filtering, time-interval widget, customisation) · **operational** (lower managers, real-time) · **tactical** (mid-level, strengths/weaknesses, strategy) · **strategic** (executives, overarching goals) · **analytical** (analysts, trends, predictions)
- **Design:** purpose · user needs (involve users!) · display (chart type, layout, device/lighting/resolution) · **context** (over time, vs. goal, internal/external) · engineering (eye travel, maintenance, future) · data on a separate sheet, users can't change it · **testing**
- **Mistakes:** ignoring org goals/users · ignoring environment · poor positioning · wrong chart type · ignoring design principles · too cluttered/too sparse · unattractive · ignoring future needs
- **Excel:** PivotTable, PivotChart, **slicers**, **Report Connections** (1 slicer → several charts), hide field buttons, protect sheet
- **EJB:** tactical, dynamic & interactive · KPIs = total $ sales + avg. delivery time

**Exam questions M9**
- Improve the yellow EJB dashboard: neutral background, sans-serif title, larger charts, compact/connected slicers next to charts, consistent colours, related charts adjacent
- Service vs. product satisfaction per DC × year → **scatter** (point = DC) as a **trellis per year** or colour per year + PivotTable; connect to the Year slicer
- Manufacturing KPIs: OEE, defect rate, first-pass yield, utilisation, cycle time, on-time delivery, inventory turnover, cost/unit, safety incidents, energy, MTBF, changeover time

---

## Module 10 – Telling the Truth

- **Missing first, then errors.** Missing: **sort**, **conditional formatting (blanks)**, **`=COUNTBLANK()`**, filter. Errors: **MIN/MAX**/summary stats, sort, frequency, histogram, **scatter** (also non-extreme). Combine methods (Blakely: 601 → 60.1 months)
- **Selection bias:** non-random sample (landline poll) · **Simpson's paradox:** trend in subgroups **reverses when aggregated** (colour scatter by group!) · **Survivor bias:** only "survivors"/positive outcomes (WWII planes: armour the areas **without** holes)
- My note: selection, survivor (*brilliance bias*), Simpson's (*confirmation bias*)
- **Inflation:** **real(t) = nominal(t) × index(base) / index(t)** · `=B2*($C$41/C2)` · 0.65 × 211.8/51.9 ≈ $2.65 (slide: $2.66)
- **Axes:** column/bar **from 0** (otherwise exaggerated); line/scatter narrower ok (too wide hides the trend). **Aspect ratio:** tall & narrow exaggerates, short & wide hides
- **Dual-axis** → false comparisons/intersections → **2 separate charts** (same x-axis)
- **Temporal frequency/time period:** low frequency smooths, cherry picking
- **Maps:** **rates instead of absolute numbers** (poverty rate instead of number of poor people)

**Exam questions M10 (likely!)**
- **A1 Java Cup:** COUNTBLANK + conditional formatting (blanks) → name respondents & variable; MIN/MAX/sort/filter, values < 0 or > 100 = errors
- **A2 Bias:** (1) Rhine/telepathy = **survivor** (only winners of each round, chance with 500 participants) · (2) exit poll outside restaurant at night = **selection** (not representative, lobby group) · (3) red wine cohort = **Simpson's paradox** (income/education as lurking variable; disaggregated the effect may reverse)
- **A3 Guaraldi:** all: **y = −4.26x + 66.48** (R² 0.20, negative) · junior: y = 0.56x + 23.48 (+) · senior: y = 1.33x + 49.49 (+) → **Simpson's paradox**; lurking = title (seniors avg. 55.7 h vacation at avg. 4.7 years; juniors 27.4 h at 7.0 years)
- **A4 Ohio:** vertical axis 0–100 % with values 4.6–14.5 % + flat chart hides the trend → axis ~0–16 %, taller chart, 7-day MA, title stating the message; trend: ~12 % (Apr) → < 5 % (Oct)
- **A5 Maximus:** dual-axis confuses (heights/intersections meaningless, arbitrary scales, lay audience) → 2 line charts stacked (headcount, revenue) with the same quarter axis; headcount 18 → 8 → 12, revenue ~$820k → ~$730k flat

---

## Excel Quick Steps (Mac: *Chart Design → Add Chart Element* instead of "+")

- **Scatter + trendline:** select x/y → *Insert → Scatter* → right-click a point → *Add Trendline → Linear* → ☑ *Display Equation* ☑ *R-squared* → adjust axis bounds, title/axis titles, remove gridlines
- **Groups in a scatter:** sort → *Select Data → Add* (name, X values, Y values) → trendline per series; highlight: other series grey/no fill
- **Histogram / box plot:** *Insert → Statistic Chart* · **Treemap:** sort → *Hierarchy Chart* · **Filled map:** *Insert → Maps*
- **Heat map:** *Conditional Formatting → Color Scales* · **Blanks:** *CF → New Rule → Format only cells that contain → Blanks* · `=COUNTBLANK()`
- **Waterfall:** total → *Format Data Point → Set as total* · **Funnel/stock:** *Insert → Waterfall, Funnel, Stock …*
- **Slope:** line with markers → *Switch Row/Column* → remove gridlines/legend/vertical axis, labels left (series name) + right
- **Error bars:** *Error Bars → More Options → Custom → Specify Value* (= MoE)
- **Moving average:** *Add Trendline → Moving Average → Period* · **Sparklines:** *Insert → Sparklines*
- **PivotChart + slicer:** *Insert → PivotChart* → drag fields → *Insert Slicer* → *Report Connections* · axis *Display units: Thousands*
- **% frequency:** *Value Field Settings → Show Values As → % of Grand Total*
- **Inflation:** `=B2*($C$41/C2)` · **Jitter:** `=C2+RAND()` · **% change:** (new − old)/old
- **Always clean up:** title (message), axis titles + units, remove gridlines/border/legend, sans-serif, column/bar from 0
- German regional settings: semicolons + decimal commas in formulas (`=CONFIDENCE.T(0,05; s; n)`)

---

## Answer Checklist "Critique / Improve this chart"

1. **Chart type** appropriate? (pie → bar, area → line, dual-axis → 2 charts, 3D → 2D)
2. **Axes:** from 0 (bar/column)? scale/aspect ratio? titles/units?
3. **Colour:** unnecessary/excessive/contrast/consistent/colour-blind/right scheme?
4. **Clutter:** data-ink ratio, gridlines, border, legend
5. **Eye travel:** direct labels, title alignment
6. **Audience:** needs + analytical comfort
7. **Truth:** bias, inflation, absolute vs. relative values, time period

**Phrases:** *reduces cognitive load* · *increases the data-ink ratio* · *humans compare lengths more accurately than angles/areas* · *Gestalt principle of proximity/enclosure* · *the preattentive attribute of colour draws attention to* · *correlation does not imply causation – a lurking variable such as …* · *when disaggregated, the trend reverses (Simpson's paradox)* · *two separate charts sharing the same x-axis*
