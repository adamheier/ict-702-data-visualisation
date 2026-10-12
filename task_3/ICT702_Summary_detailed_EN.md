# ICT702 Data Visualisation – Detailed Summary (Modules 2–10)

Exam preparation for Task 3 · Based on the textbook Camm, Cochran, Fry & Ohlmann (2021) *Data Visualization – Exploring and Explaining with Data*, lecture slides, Canvas pages and workshop activities

> **Note on numbering:** The Canvas modules are called **Modules 2–10**, but the slide decks are numbered **Modules 1–9** (always offset by one). This summary uses the **Canvas numbering** (= folder names, = numbers of the workshop activity sheets).
>
> **Model answers:** The sample answers are a guide only. Copy & paste is not allowed in the exam, so always type the answer **in your own words**.

---

## Contents

0. Exam information & strategy
1. Module 2 – Introducing Data Visualisation
2. Module 3 – Selecting a Chart Type
3. Module 4 – Data Visualisation and Design
4. Module 5 – Purposeful Use of Colour
5. Module 6 – Visualising Variability
6. Module 7 – Exploring Data Visually
7. Module 8 – Explaining Visually to Influence with Data
8. Module 9 – Data Dashboards
9. Module 10 – Telling the Truth with Data Visualisation
10. Appendix A – Excel how-to guides (incl. Mac notes)
11. Appendix B – Formulas & Excel functions
12. Appendix C – Answer frameworks for essay questions
13. Appendix D – Glossary

---

## 0. Exam Information & Strategy

### Conditions
- **Weighting:** 40 % of the final grade · Canvas exam during the Week 12 workshop (starts 15 min after the workshop begins)
- **Duration:** 90 minutes, auto-submits at the end
- **5 questions** (short essay or file upload), randomly drawn from question pools
- **Marks according to my notes:** Q1 = 4 · Q2 = 8 · Q3 = 10 · Q4 = 12 · Q5 = 6 → **40 marks**
- **No going back** → answer each question completely (including file upload!) before moving on
- **Allowed:** paper notes (typed/printed or handwritten). **Not allowed:** digital resources, phone, generative AI
- **No copy & paste** from any source → 0 marks for that answer
- Bring student ID; the login password is given in the workshop
- Content: **Modules 2–10** (Power Platform/PL-900 is **not** examined)
- Lecturer's tip: **Redo all workshop activities**; exam questions are similar (e.g. Activity 1 or 2 from Module 10, "create a scatter chart and trendline")

### Time plan (≈ 2.2 min per mark)

| Question | Marks | Time budget | Clock time (start 12:15) |
|---|---|---|---|
| Q1 | 4 | ~8 min | until ~12:23 |
| Q2 | 8 | ~17 min | until ~12:40 |
| Q3 | 10 | ~22 min | until ~13:02 |
| Q4 | 12 | ~26 min | until ~13:28 |
| Q5 | 6 | ~13 min | until ~13:41 |
| Buffer | – | ~4 min | end 13:45 |

### Strategy
- **Marks = number of expected arguments.** 4 marks → at least 4 clear points; 12 marks → definition + several justified points + example/reference to the data.
- **Structure of every answer:** (1) direct answer, (2) justification using the technical term, (3) concrete reference to the example/data, (4) improvement suggestion if relevant.
- **File questions:** download the file → edit → **save as .xlsx** → **rename** (e.g. `Surname_StudentID_Q3.xlsx`) → upload → check the upload arrived → only then move on. If asked, also write a short **interpretation** in the text box.
- In case of technical problems, take a **screenshot with the time visible**.

<div style="page-break-after: always;"></div>

## 1. Module 2 – Introducing Data Visualisation

### 1.1 Analytics
- **Analytics** = the scientific process of transforming data into **insights for better decisions** (discovering, interpreting and communicating patterns).
- **Reasons for the explosive growth of analytics:** technological developments, methodological developments, huge increase in computing power and storage capability.

| Type | Question | Examples |
|---|---|---|
| **Descriptive** | What happened? | Data queries, standard reports, descriptive statistics, **data visualisation**, dashboards, cluster analysis, what-if spreadsheet models |
| **Diagnostic** | Why did it happen? | Root-cause analysis, drill-down (Canvas page only, not on the slides) |
| **Predictive** | What will happen? | Linear regression, time series analysis, predictive data mining, forecasts |
| **Prescriptive** | What should we do? | Optimisation, simulation, decision analysis |

- **Data visualisation is part of descriptive analytics**, but it is also used to explain results of predictive/prescriptive models.
- Weather app example: the forecast is **predictive**. If it recommends an action ("take an umbrella"), that would be **prescriptive**.

### 1.2 Why visualise data?
1. **Exploring data**: identify patterns (e.g. seasonality in zoo attendance) and relationships between variables
2. **Explaining / communicating**: convey insights and model results to an audience
- **Anscombe's quartet:** data sets with an identical regression equation (y = 0.5x + 3) and R² = 0.67 look completely different when plotted. Lesson: **always visualise; never rely on summary statistics alone.**

### 1.3 Types of data

| Term | Meaning | Example |
|---|---|---|
| **Quantitative data** | Numbers indicate **magnitude**; arithmetic operations possible | Price, volume, revenue |
| **Categorical data** | **Labels/names** for groups; no arithmetic | Company, industry, symbol |
| **Cross-sectional data** | Several entities at the **same point in time** | Prices of 75 houses on 3 Jan 2021 |
| **Time series data** | Observations over **several time periods** (usually regular) | Dow Jones 2010–2020, Netflix subscribers per year |

- Caution: **numbers can be categorical** (e.g. postcode, year used as a label, rating 1–4 = ordinal).
- **Big data**: data too large/complex for a desktop computer or standard processing techniques. **The 4 Vs:**
  - **Volume** – amount of data generated
  - **Velocity** – speed of data generation
  - **Variety** – diversity of types and structures
  - **Veracity** – reliability/quality of the data
- **Word cloud**: commonly used chart to summarise words in large sets of text data.

### 1.4 Visualisations by business function (examples from the slides)

| Function | Chart | Purpose |
|---|---|---|
| Accounting | Clustered column: **Benford's Law** vs. actual data | Fraud detection (first-digit law) |
| Finance | **High-low-close stock chart** | Closing price trend + daily volatility |
| HR | **Stacked column** (leavers/new hires per month) | Part-to-whole over time |
| Marketing | **Funnel chart** | Conversion from large to small values (website visitors → buyers) |
| Operations | **Line chart** | Trend, repeating patterns, forecast |
| Engineering | **Control chart** (upper/lower control limits) | Is the process "in control"? |
| Science | **Spaghetti chart** on a map | Many possible paths (e.g. hurricane model tracks) |
| Sports | **Shot chart** | Shot locations; symbol/colour = made/missed |

### 1.5 Benford's Law (First-Digit Law)
- Expected proportion of the first digit in many real-life data sets:

| Digit | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 |
|---|---|---|---|---|---|---|---|---|---|
| Benford | 30.1 % | 17.6 % | 12.5 % | 9.7 % | 7.9 % | 6.7 % | 5.8 % | 5.1 % | 4.6 % |

- If data deviate strongly, **fraud investigation may be warranted** (not proof of fraud).

### 1.6 Cognitive load & refining a chart (zoo example)
- **Cognitive load** = mental effort needed to understand a visualisation. Goal: as low as possible.
- Typical improvements to Excel's default chart (Activity 5): remove gridlines, meaningful title left-aligned above the vertical axis, add axis titles (vertical axis title **horizontal** above the axis), black axis lines, tick marks "Inside", consistent font (Calibri 10.5 / title 16), remove chart border.

### 1.7 Workshop Activities Module 2 – Solutions

**Activity 1 – Types of Analytics**
1. Data dashboard → **descriptive**
2. Model that finds the production schedule minimising overtime → **prescriptive** (optimisation)
3. Model that forecasts next quarter's sales → **predictive**
4. Bar chart → **descriptive**
5. Model that allocates investments to achieve a financial goal → **prescriptive**

**Activity 2 – House Price & Square Footage (75 houses, 3 Jan 2021)**
1. **Quantitative** (price and size are measurements)
2. **Cross-sectional** (one point in time, many houses)
3. **Scatter chart**, because it shows the relationship between two quantitative variables; each point = one house. Bar/column charts compare categories and are not suitable here.

**Activity 3 – Netflix Subscribers 2010–2019**
1. **Quantitative** (number of subscribers in millions)
2. **Time series** (annual values)
3. **Column chart** with data labels (alternative for the trend: line chart)

**Activity 6 – Benford vs. Tucker Software (read from the chart)**

| Digit | Benford | Tucker (approx.) | Deviation |
|---|---|---|---|
| 1 | 0.301 | 0.255 | −0.046 (≈ −15 %) → **under-represented, largest absolute deviation** |
| 3 | 0.125 | 0.100 | −0.025 (≈ −20 %) |
| 4 | 0.097 | 0.080 | −0.017 (≈ −18 %) |
| 5 | 0.079 | 0.150 | **+0.071 (almost double)** → over-represented |
| 7 | 0.058 | 0.040 | −0.018 (≈ **−31 %, largest relative deviation**) |
| 9 | 0.046 | 0.100 | **+0.054 (≈ double)** → over-represented |

- **Model answer:** *"The data do not fully conform to Benford's Law. Digits 5 and 9 are clearly over-represented (roughly double the expected probability), while digit 1 is under-represented by the largest absolute amount (about 4.6 percentage points) and digit 7 by the largest relative amount (about 30 % below expectation). These deviations do not prove fraud but warrant further investigation of the accounts payable entries."*

### 1.8 Possible Exam Questions Module 2
- Assign examples to analytics types (descriptive/predictive/prescriptive) and justify.
- For a data set, decide quantitative/categorical **and** cross-sectional/time series; recommend a chart type with justification.
- Explain the 4 Vs of big data.
- Explain the two reasons for visualising data (explore vs. explain), with Anscombe as an example.
- Interpret a Benford chart (over-/under-represented digits, absolute vs. relative deviation).
- **File:** create a column chart from the zoo data and refine it (decluttering steps).

<div style="page-break-after: always;"></div>

## 2. Module 3 – Selecting a Chart Type

### 2.1 Defining the goal of your visualisation
- Before choosing a chart: **know your data, know your audience, know the chart types.**
- Communicating → choice depends on the **message**. Exploring → choice depends on the **question** you want answered. The **data type** also matters.
- **Four common goals:**
  - **Composition** – what makes up the whole? (components)
  - **Ranking / Comparison** – what is the relative order? (order)
  - **Relationship** – how are two variables related? (patterns)
  - **Distribution** – how are the values dispersed? (dispersion)

### 2.2 Guidelines for Selecting a Chart (slide, important!)

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

(Canvas quiz version: Scatter = relationship + distribution · Bubble = relationship · Histogram = distribution · Stacked column/area = composition + comparison · Pie/Waterfall = composition · Table/Line/Spider/Column = comparison)

### 2.3 Chart types in detail
- **Column chart**: compares categories; distribution over discrete categories or time periods. Better than bar for time (time naturally runs left to right).
- **Bar chart**: like column but horizontal. Better for **long category names**. **Sorted** bar charts are good for rankings.
- **Clustered column/bar**: several series side by side. Gets cluttered quickly with many series.
- **Stacked column/bar**: **part-to-whole**; total height shows the sum (e.g. East + West = total sales).
- **Line chart**: time series. Connected points suggest **continuity** and make trends/changes easy to see. Multiple-line chart to compare series (often less cluttered than clustered column).
- **Scatter chart**: relationship between **two quantitative variables**; each point = a pair of measurements (e.g. average low temperature vs. snowfall in 51 US cities). "Among the most useful charts for exploring pairs of quantitative data."
- **Bubble chart**: scatter + **third quantitative variable as bubble size** (airports: x = TSA wait time, y = cheapest parking rate, size = enplanements). Weakness: sizes are hard to judge.
- **Choropleth map**: values (quantitative or categorical) shaded over geographic areas (e.g. population by state, Amazon fulfilment centre yes/no).
- **Heat map**: 2D table where **shades of colour show magnitude**; good for patterns between categories.
- **Treemap**: **hierarchical** data. Rectangle size = value, colour = parent category (e.g. industry → brand → brand value).
- **Waterfall chart**: cumulative effect of positive and negative changes (composition over time/categories, e.g. monthly gross profit → total).
- **Stock chart (high-low-close)**: daily high, low and closing price.
- **Funnel chart**: progression from large to small values across stages (applicants → hires). Can also show composition (drill-down).
- **Tables** instead of charts when:
  - specific numerical values are required
  - precise comparisons between values are needed
  - values have different units or very different magnitudes
- **Table + chart combined** (e.g. line chart with data table underneath) is also possible.

### 2.4 Chart types to avoid (+ alternative)

| Avoid | Why | Better |
|---|---|---|
| **Pie chart** (more than a few categories) | People judge **length** better than **angle/area**; many colours increase cognitive load; labels/legend → eye travel | (sorted) **bar chart** |
| **Radar/spider chart** | difficult to interpret | **Clustered column chart** |
| **Area chart** (esp. simple/stacked) | cluttered, hidden areas, hard to read | **(Multiple) line chart** |
| **Combo / dual-axis chart** | cluttered, invites wrong comparisons | **two separate charts** |
| **3D charts** | third dimension = clutter, distorts proportions | **2D version** |

### 2.5 Excel specifics
- Excel usually uses the **leftmost column as the horizontal axis**; the assignment can be switched ("Switch Row/Column").
- **"Year as a number" problem:** if you select Year + Sales, Excel plots Year as its own data series. **Fix:** right-click → *Change Chart Type* → choose the version with one series (or set Year as text/axis labels via *Select Data → Horizontal (Category) Axis Labels*).
- Line chart from numeric x values: *Insert → Scatter → Scatter with Straight Lines and Markers*.
- **Recommended Charts** tool: gives suggestions but does not replace your own judgement.

### 2.6 Workshop Activities Module 3 – Solutions

**Activity 1 – Cheetah Sports (column, clustered, stacked)**
- *Why is the stacked column chart preferred over clustered?* It shows **each region's contribution and the total sales at the same time** (total column height), i.e. composition and total over time, with only one column per year and less clutter.
- *Two examples of when the audience would prefer each chart:*
  - **Line chart**: regional managers want to **compare the trends of both regions directly** (e.g. West growing over the last three years, East dropping since year 7). A line chart shows trend direction and turning points clearly.
  - **Stacked column chart**: senior management is interested in **total sales per year and how much each region contributes** (part-to-whole).

**Activity 2 – Line chart (Cheetah)** → Scatter with Straight Lines and Markers; lines suggest continuity.

**Activity 3 – New York City Budget**
1. Two reasons for bar instead of pie:
   - People compare **lengths** more accurately than **angles/areas** (preattentive attribute length).
   - Many categories need many colours + a legend in a pie → higher **cognitive load** and eye travel. A bar chart can be **sorted** and labelled directly.
2. Bar instead of column: the **long category names** (budget items) are easy to read horizontally; a sorted horizontal ranking reads naturally from top to bottom.

**Activity 4 – Anscombe & trendlines**
- Same regression equation (y = 0.5x + 3) and R² = 0.67, but: **data set 1** scatters randomly around a straight line → linear trendline is appropriate. **Data set 2** follows a clearly **curved (nonlinear)** pattern → a linear trendline is inappropriate; a polynomial (order 2) fits.
- **Model answer:** *"Identical summary statistics can hide very different patterns. A linear fit is appropriate for data set 1, but data set 2 follows a curved pattern, so a straight line misrepresents the relationship. This is why data should always be visualised before fitting a model."*

### 2.7 Possible Exam Questions Module 3
- Which chart for goal X (composition/ranking/relationship/distribution) and data type Y? Justify.
- Why bar instead of pie (2–3 reasons)? Why bar instead of column?
- Which charts should be avoided, why, and what is the alternative?
- Clustered vs. stacked column vs. multiple line: when to use which?
- When to use a table instead of a chart?
- **File:** column/clustered/stacked column chart from CheetahRegion; fix the year-as-number problem; add data labels.
- **File:** create a scatter chart + trendline and judge whether a linear fit is appropriate.

<div style="page-break-after: always;"></div>

## 3. Module 4 – Data Visualisation and Design

### 3.1 Visual perception & preattentive attributes
- **Visual perception**: the brain process that interprets reflections of light entering the eyes. Three forms of memory affect it: **iconic memory**, **short-term memory**, **long-term memory**.
- **Preattentive attributes** = features processed by **iconic memory**, i.e. recognised **without conscious effort** in a fraction of a second.
- **Cognitive load** = effort needed to process information accurately and efficiently. Proper use of preattentive attributes **reduces** it.

| Category | Attributes | Notes |
|---|---|---|
| **Colour** | Hue, saturation, luminance | Highlighting, grouping |
| **Form** | Orientation, size, shape, length, width | Orientation: slope in line charts. **Size is estimated poorly.** Length: bar/column. Width: Sankey chart (line width = flow) |
| **Spatial positioning** | Position in 2D space | e.g. points in a scatter chart |
| **Movement** | Flicker (flashing), motion (directed movement) | Usually not possible in static charts |

- Combining attributes (e.g. colour × shape) creates more groups (3 colours × 3 shapes = 9 groups) but also more cognitive load.
- **Overuse** of preattentive attributes → clutter: "If everything is highlighted, nothing is highlighted."

### 3.2 Gestalt principles
How people bring order and meaning to what they see. The **four main principles for data vis:**

| Principle | Meaning | Application |
|---|---|---|
| **Similarity** | Similar characteristics (colour, shape) → same group | Same colour for the same category in every chart |
| **Proximity** | Close together → belong together | Labels directly next to the data series; space between groups |
| **Enclosure** | Enclosed/shaded together → belong together | Shaded area for the forecast period; box around a group in a scatter |
| **Connection** | Connected objects → belong together | Lines in time series; dashed line for forecast vs. solid for actual |

(Others from the Canvas quiz: **closure, continuation, symmetry, good figure/prägnanz**.)

### 3.3 Data-ink ratio & decluttering
- **Data-ink ratio** = proportion of ink used to display data relative to the total ink in a chart/table (Edward Tufte's concept).
  - **Data-ink**: necessary to convey the meaning of the data
  - **Non-data-ink**: serves no purpose (e.g. heavy gridlines, borders, 3D effects, background colours, redundant legends, logos)
- **Decluttering** = increasing the data-ink ratio. **White space** has the same effect.
- **Typical declutter steps:** remove/lighten gridlines, remove border, remove legend (single series) or replace with direct labels, remove background colour, remove unnecessary decimals, remove 3D, subtle axes, data labels instead of an axis (if few values).
- **Table rules:**
  - Numbers **right-aligned**, text **left-aligned**
  - **Same number of decimal places** within a column, but only as many as needed
  - Round large numbers (thousands, millions)
  - Few lines, plenty of white space

### 3.4 Minimising eye travel
Cognitive load is reduced by using preattentive attributes, Gestalt principles, a higher data-ink ratio and **minimal eye travel**:
- Align the chart title and vertical-axis title **left with the vertical axis**
- Place **line labels directly to the right of the lines** (instead of a legend)
- Place the horizontal-axis label at the end of the axis, level with the line labels

### 3.5 Fonts
- **Sans-serif** (Arial, Calibri, Verdana, Myriad Pro) → **preferred for data vis**, legible at small sizes
- **Serif** (Times New Roman, Courier) → for printed body text; end-of-stroke features, less legible at small sizes
- **Consistent and restrained:** ideally **one** font; horizontal- and vertical-axis titles same font and size. Use size, **bold**, *italic* and colour deliberately for emphasis.

### 3.6 Common design mistakes
1. **Wrong type of visualisation** (e.g. clustered column instead of line chart for a time comparison)
2. **Displaying excessive information** in one chart (e.g. OEM + aftermarket sales for many regions). **Fix:** stacked clustered column or **separate charts**
3. Using **Excel default settings** unchanged
4. **Too many attributes** (colour + shape + size at once)
5. **Unnecessary 3D**
6. Logos/pictures instead of columns (fast-food makeover): distorts perception

### 3.7 Workshop Activities Module 4 – Solutions

**Activity 1 – Discuss the statements**
- *Preattentive attributes draw the audience's attention:* true. A contrasting colour for the most important bar draws the eye there immediately.
- *Overuse leads to clutter:* true. Many colours/shapes/sizes compete for attention, nothing stands out any more, and cognitive load increases.

**Activity 2 – Counting the 7s in a 16×10 digit matrix** (besides hue and size)
- **Shape/form:** 7s in a different font or as a different symbol
- **Orientation:** 7s tilted/rotated
- **Width:** 7s in **bold** (thicker stroke)
- **Enclosure:** box/circle around each 7 (Gestalt) or **background shading** of the cell
- **Luminance/saturation:** all other digits light grey, 7s black
- **Spatial positioning:** 7s slightly offset (higher/lower)
- **Movement (digital):** make the 7s flash (flicker)

**Activity 3 – Scarf Sales: increasing the data-ink ratio**
1. *Remove:* gridlines, legend (only one series), chart border, unnecessary decimals/axis line if any, default "Chart Title".
2. *Add for readability:* meaningful title (left-aligned), axis titles (vertical title horizontal at the top of the axis), sensible axis scale/units, data labels for key points if useful, consistent font.

**Activity 4 – Scatter chart Snow (51 cities)**
- The **higher the average low temperature**, the **less snowfall** (negative, **nonlinear** relationship). For warm cities, snowfall approaches **zero and levels off**; cold cities show large variability.

**Activity 5 – Bubble chart Airports**
- Formulate conclusions: is there a relationship between wait time (x) and parking rate (y)? Do large airports (big bubbles) have higher parking rates/wait times? Which outliers stand out?
- Swap axes via *Select Data → Edit*: reassign Series X values / Y values / bubble size. Then judge whether the new assignment shows the most important relationship better (the two variables with the most important relationship belong on the axes, because bubble sizes are hard to compare).

**Activity 6 – NYC: % college graduates vs. median monthly rent**
1. Preattentive attribute: **spatial positioning** (2D position of the points)
2. **Positive relationship:** sub-boroughs with a higher share of college graduates tend to have higher median rents. Correlation ≠ causation (e.g. income as a lurking variable).

### 3.8 Possible Exam Questions Module 4
- Define preattentive attributes and name the 4 categories with examples.
- Name/explain the 4 Gestalt principles with an application example in a chart for each.
- What is the data-ink ratio? How do you increase it (list of steps)?
- How do you minimise eye travel?
- Serif vs. sans-serif: which for data vis and why?
- Critique a given chart: what is poor, how to improve it?
- **File:** declutter a default chart (Scarf Sales), create and interpret a scatter (Snow) or bubble chart (Airport).

<div style="page-break-after: always;"></div>

## 4. Module 5 – Purposeful Use of Colour

### 4.1 The three attributes of colour
- **Colour** = the property of an object resulting from how it reflects or emits light.

| Attribute | Meaning | Extremes |
|---|---|---|
| **Hue** | The "base" of a colour, its position on the light spectrum. Primary hues (slides: **RGB = red, green, blue**; Canvas text: red, yellow, blue) cannot be mixed from other hues; combinations give secondary/tertiary colours (colour wheel) | – |
| **Saturation** | Amount of **grey**, i.e. intensity/purity | 100 % = pure hue · 0 % = grey |
| **Luminance** | Amount of **black vs. white** | 100 % = white · 0 % = black; creates contrast and **hierarchy** |

### 4.2 Colour psychology vs. colour symbolism
- **Colour psychology**: **innate** relationships between colour and human behaviour (fairly universal)
  - **Cool hues** (purple, blue, green) → calming, reassuring; appear **more distant**
  - **Warm hues** (yellow, orange, red) → energy, passion, danger
- **Colour symbolism**: **cultural** meaning (e.g. white = mourning in parts of Asia). Varies much more across cultures and **changes over time**.
- **Perceived colour**: colour is perceived **relative to its surroundings/background** (the same colour looks different on different backgrounds).
- **Complementary colours** (opposite on the colour wheel) → **dissonance**, strong contrast, good for making things stand out; overuse distracts.
- **Analogous colours** (adjacent on the colour wheel) → soft, harmonious, less contrast.
- Multicoloured backgrounds are distracting.

### 4.3 Colour schemes (by data type)

| Scheme | Data type | Construction | Example |
|---|---|---|---|
| **Categorical** | Categorical, **no inherent order** | Distinct, easily distinguishable hues; **max. ~6 colours** | Industries in a treemap |
| **Sequential** | Ordered / quantitative (ascending) | **One hue**, gradient of **luminance** (more common) or saturation; light = low, dark = high | Choropleth of population, average temperature (brown = warmth) |
| **Diverging** | Quantitative **with a meaningful reference value** (e.g. 0, average) | **Two** sequential schemes sharing a **common midpoint**; two different hues; luminance shows the size of the deviation | Same-store sales heat map (red = decline, white = 0, blue = growth) |
| **Highlight** | Emphasise one element | Everything grey, one element in an accent colour | One line among many |

### 4.4 HSL in Excel
- *Format → Fill → More Colors → Custom → Colour model HSL*
- Values 0–255: **Hue** (slider left → right), **Sat** (0 = grey, 255 = pure), **Lum** (0 = black, 255 = white; **128 = pure hue**)
- **Eyedropper** to copy a colour (e.g. company logo); **Transparency** 0–100 %. RGB model as an alternative.

### 4.5 Common mistakes with colour
1. **Unnecessary colour**: colour that carries no information (e.g. every column a different colour + legend). **Fix:** one colour, label categories directly on the axis.
2. **Excessive colour**: too many colours (51 states = 51 colours). **Fix:** focus group in colour, rest **grey**, replace legend with direct labels.
3. **Insufficient contrast**: colours too similar. **Fix:** increase the luminance difference.
4. **Inconsistency across related charts**: same category coloured differently in different charts. **Fix:** consistent colour coding (e.g. adults always orange, children always blue).
5. **Neglecting colour-blindness**: most common is **red-green colour-blindness** (more common in men); also blue-yellow; total colour-blindness is rare. **Fix:** avoid red-green, use blue-orange/blue-red, add luminance differences, labels and shapes.
6. **Not considering the mode of delivery**:
   - **Projected:** thick lines, sharp outlines, strong contrast, **high** saturation and luminance
   - **Printed:** softer outlines, **less** saturation, lower luminance, less contrast
   - Colours vary between monitors/projectors/printers → **check the output beforehand**

### 4.6 Workshop Activities Module 5 – Solutions

**Activity 1 – Hue, saturation or luminance?** (my answers)
a) **Saturation** · b) **Luminance** · c) **Luminance** · d) **Hue** · e) **Saturation** · f) **Luminance**
- Reasoning: same hue but one looks greyish/dull → saturation. Same hue but lighter/darker → luminance. Completely different hue (pink vs. blue) → hue.

**Activity 2 – Choropleth map StatePopulation**
- Dark = high population: **California, Texas, Florida, New York** are the most populous. Sparsely populated states (e.g. Wyoming, Alaska, Vermont) are light.
- Critical addition: **absolute numbers** favour large states; for fair comparisons use **relative values** (e.g. population density) (see Module 10).

**Activity 3 – Choosing colour schemes**
- *Median family income by state* → **sequential colour scheme**: **one hue** (e.g. green or blue), **luminance gradient**: light = low, dark = high income. Reason: ordered quantitative variable without a natural midpoint.
- *Change in income 2010 vs. 2020* → **diverging colour scheme**: **reference value 0 % change** = white/light grey. **Two hues**, e.g. **red/orange** for decrease and **blue** for increase; the darker (lower luminance), the bigger the change. Avoid red-green (colour-blindness).

**Activity 4 – Heat map SameStoreSales** (Conditional Formatting → Colour Scales → Blue-White-Red)
- Red = decline, blue = increase vs. the same month last year. Easy to spot: e.g. **Austin** consistently strongly positive. **Phoenix/Seattle** start positive and turn negative during the year. **Cincinnati/St. Louis** the reverse (negative → positive). **Albany** negative almost all year.
- Difficulty: exact values are hard to read (fix: keep the numbers in the cells). Fine gradations are hard to distinguish; red/white/blue is more colour-blind friendly than red/green.

**Activity 5 – Treemap BrandValues** → first sort by Industry, then *Insert → Hierarchy Chart → Treemap*; show values via *Format Data Labels → Value*. Colour = industry, rectangle size = brand value.

**Activity 6 – ManagementTop25 treemap** (Sector → Company → Score; sort by sector first)
- Sector with the most companies: **Technology (12 of 25)**; highest score in Technology: **Amazon (120.2)** (recalculated from the file).

### 4.7 Possible Exam Questions Module 5
- Define hue, saturation and luminance and classify colour pairs accordingly.
- Colour psychology vs. colour symbolism with examples.
- Which colour scheme (categorical/sequential/diverging) for scenario X? Define hues and luminance!
- Name and explain common colour mistakes and how to avoid them (colour-blindness, projection vs. print …).
- Complementary vs. analogous colours.
- **File:** create and interpret a choropleth (Filled Map), heat map (Conditional Formatting) or treemap.

<div style="page-break-after: always;"></div>

## 5. Module 6 – Visualising Variability

### 5.1 Basic terms
- **Random variable**: quantity whose value is not known with certainty
- **Variation**: difference in the values of a variable across observations (time, customer, product …) → creates **uncertainty**
- **Sample**: subset of the **population**; if representative, conclusions about the population can be drawn
- **Frequency distribution**: which values occur and how often?

### 5.2 Frequency distribution – categorical data
- Divide data into non-overlapping **bins/classes** → count frequency (PivotTable or `COUNTIF`)
- **Relative frequency** = frequency of the bin / n
- **Percent frequency** = relative frequency × 100 → **estimates the probability distribution**
- Display: column/bar chart, **sorted** (largest first). **Exception: ordinal data** (e.g. satisfaction 1–5) → **keep the natural order**!

### 5.3 Frequency distribution – quantitative data (histogram)
Three things to define:
1. **Number of non-overlapping bins**: **5–20** (depends on n). Too few → variation is blurred (too aggregated). Too many → no generalisable patterns.
2. **Bin width**: **the same** for all bins; approximation: **(largest value − smallest value) / number of bins**
3. **Range spanned by the bins**: first bin must include the smallest value, last bin the largest; **every value in exactly one bin**
- **Notation (17, 25]**: round bracket = value **not** included, square bracket = value **included**
- **Histogram** = column chart **without gaps**, height = frequency; shows the **shape** of the distribution
- **Kernel density chart**: smoothed curve of the distribution

### 5.4 Skewness
| Shape | How to recognise | Measures of location | Examples |
|---|---|---|---|
| **Left-skewed (negative)** | long tail to the **left** | **Mean < median** | Age at death, scores in an easy exam |
| **Symmetric** | bell-shaped | Mean ≈ median | Height of adult men |
| **Right-skewed (positive)** | long tail to the **right** | **Mean > median** | House prices, income, delivery time |
- In a box plot: **longer whisker / larger gap between median and quartile** on the side of the tail.

### 5.5 Comparing distributions
- **Frequency polygon**: like a histogram, but **lines** connect the bin frequencies → several distributions can be compared on top of each other (Excel: line chart). Less cluttered than clustered columns.
- **Trellis display**: several **equally sized charts with the same scales** side by side/stacked (small multiples), e.g. length of stay at 3 hospitals.
- **Strip chart**: each **individual value** as a point along an axis (e.g. half-marathon times by sex). Problem **occlusion**: points overlap.
  - **Fixes:** hollow markers (No fill) and **jittering** (random vertical offset, `=C2+RAND()`)
- **Box and whisker chart** (see 5.7), **violin chart** = box plot + mirrored kernel density curve.

### 5.6 Measures of location and variability

| Measure | Definition | Excel | Note |
|---|---|---|---|
| **Mean** | sum / n | `AVERAGE` | influenced by outliers |
| **Median** | middle value of sorted data (even n: average of the two middle values) | `MEDIAN` | robust, **preferred for skewed data** |
| **Mode** | most frequent value (can be several/none) | `MODE.SNGL` / `MODE.MULT` | useful with few distinct values; in a histogram = tallest column |
| **Range** | max − min | `MAX` − `MIN` | uses only 2 values, sensitive to extremes |
| **Standard deviation** | average deviation from the mean | `STDEV.S` | reliable for symmetric/bell-shaped data; **not** for skewed data |
| **Percentile (p-th)** | value exceeding p % of observations | `PERCENTILE.EXC` | robust |
| **Quartiles** | Q1 = 25th · Q2 = 50th (= median) · Q3 = 75th percentile | `QUARTILE.EXC` | split data into 4 parts |
| **IQR** | **Q3 − Q1** (middle 50 %) | – | robust, no bell shape needed |

- **Empirical rule** (bell-shaped, symmetric distribution): ≈ **68 %** within ±1 SD, ≈ **95 %** within ±2 SD, ≈ **99.7 %** within ±3 SD.

### 5.7 Box and whisker chart
- **Box** from **Q1 to Q3**, **line = median**, **X = mean**
- **Whiskers** extend to the smallest/largest value **within the limits**
- **Outliers** (dots): values outside **[Q1 − 1.5 × IQR ; Q3 + 1.5 × IQR]**
- Ideal for **comparing several distributions** (e.g. house prices in 5 suburbs: Shadyside highest, Hamilton lowest; Irving and Groton same median, Irving higher variability)

### 5.8 Uncertainty – statistical inference
- **Statistical inference**: drawing conclusions about a population from a sample. There is always **sampling error**, so show estimates as **intervals** (otherwise the audience overestimates their precision).
- **Confidence interval (CI)** = point estimate **± margin of error**. Indicates how close the sample mean/proportion is likely to be to the population value (usually 95 % or 99 %).
- **Margin of error (mean)** depends on:
  - **Sample size n** ↑ → MoE **smaller**
  - **Variability (s)** ↑ → MoE **larger**
  - **Confidence level** ↑ → MoE **larger** (wider interval)
- **Margin of error (proportion)** depends on n, the sample proportion and the confidence level.
- Formulas (extra knowledge): mean: `t × s/√n`, in Excel **`=CONFIDENCE.T(0.05, s, n)`**. Proportion: `z × √(p(1−p)/n)` with z = 1.96 for 95 %.
- **Visualisation:** column chart with **error bars** (Custom: positive and negative value = MoE) + text box "95 % confidence interval".
- **Interpretation:** if the **entire** 95 % CI is above 0, we can conclude with 95 % confidence that the mean is positive. **If the CI contains 0**, we cannot.

### 5.9 Uncertainty in predictive models
- **Prediction interval (PI)**: range in which a **future individual observation** will fall with a given probability (wider than a CI, because individual values vary more).
- **Simple linear regression**: approximates the relationship between the **independent variable (x)** (cause, explanatory, horizontal axis) and the **dependent variable (y)** (effect, predicted, vertical axis) with a straight line.
- **Time series**: the **further into the future**, the **wider** the prediction interval (more uncertainty). In regression, the PI widens the further x is from its mean.
- Display: observations as points, point prediction as a line, lower/upper PI limits as (dashed) lines.

### 5.10 Workshop Activities Module 6 – Solutions

**Activity 1 – Pop (500 soft drinks): count vs. % of grand total**
- **% (percent frequency)** is usually more useful: shares can be compared directly, independent of sample size, and it estimates the probability distribution (market shares). Counts are useful when absolute numbers matter. The shape of the chart is identical; only the axis changes.

**Activity 2 – Histogram Death (700 people)**
- **Left-skewed**: most people die at an older age (approx. 70–90), few young. Mode in the high age range, long tail towards young ages. Mean < median.

**Activity 3 – Skewness**
1. **Age of death → left-skewed**: most die old, few die young
2. **Scores in an easy exam → left-skewed**: most score high, few score low
3. **Housing prices → right-skewed**: most moderate, a few very expensive houses
4. **Adult male height → symmetric**: bell-shaped around the average

**Activity 4 – Frequency polygon DeathTwo**
- `=COUNTIF(B2:B701,"Female")`, bins 0, 7, 14, … 105 / 7, 14, … 112
- `=FREQUENCY(A2:A328,E6:E21)/$F$3` (dynamic array → relative frequency)
- Labels: `=CONCAT("(",D6,",",E6,"]")`
- Clustered column chart → then line chart = frequency polygon

**Activity 5 – Frequency polygon considerations**
1. Detecting left skew: **mean < median**; **median − Q1 > Q3 − median**; in a box plot the **lower whisker is longer**.
2. Alternative display: **box and whisker charts** (male/female side by side), trellis of histograms, violin chart, kernel density.
3. Outliers: count values below **Q1 − 1.5 × IQR** or above Q3 + 1.5 × IQR (shown as dots in the box plot).

**Activity 6 – Strip chart & jittered strip chart (HalfMarathon)**
- Sort (Sex Z→A, then Time), Male = 10 and Female = 20 as y-value, scatter chart with 2 series, markers **No fill**, jitter `=C2+RAND()`, replace legend with text boxes.

**Activity 7 – CEO time in meetings**: strip chart with jitter, `MEDIAN`, `AVERAGE`, `MODE.SNGL` (most common value).

**Activity 8 – Box & whisker SalesComparison**: *Insert → Statistic Chart → Box and Whisker*. Insights: compare median (location), box width/IQR (spread), whisker length (skewness), outliers.

**Activity 9 – XFL viewership (Friday vs. Saturday)**: both box plots in one chart. Compare median, IQR, range, skewness and outliers ("Saturday games have a higher/lower median viewership …").

**Activity 10 – Confidence-interval error bars**: *Chart Elements → Error Bars → More Options → Custom → Specify Value*, positive & negative = cells containing the margin of error.

**Activity 11 – FedTaxErrors (n = 10,001)**
1. Mean: `=AVERAGE(...)` · 2. SD: `=STDEV.S(...)` · 3. MoE: `=CONFIDENCE.T(0.05, s, n)`
4. Column chart with error bars ±MoE
5. If the **lower CI limit is > 0**, we can conclude with 95 % confidence that taxpayers **underpay** on average. If the CI contains 0, we cannot.

**Activity 12 – Prediction intervals for regression (Yourier)**
- As the number of requests increases, travel time increases (positive linear relationship). Most observations fall within the 95 % PI band. The band is wider for values further from the mean of x, so predictions there are less certain.

**Activity 13 – Prediction intervals for a time series (Bundaberg root beer)**
- Point forecasts continue the trend and **seasonality**. The 95 % PI **widens the further the forecast extends into the future** → planning should account for this uncertainty.

### 5.11 Possible Exam Questions Module 6
- Define mean, median, mode, range, SD, percentile, quartile, IQR; when to use median instead of mean?
- Determine and justify skewness for examples (Activity 3!).
- Read a box plot: median, IQR, outliers, skewness; compare two distributions.
- Calculate outlier limits (Q1 − 1.5 IQR, Q3 + 1.5 IQR).
- Define bins (number, width, range); notation (a, b].
- What is occlusion and how do you fix it (jitter, hollow markers)?
- Confidence interval vs. prediction interval; what affects the margin of error?
- **File:** create a histogram, box & whisker, strip chart, column chart with error bars, frequency polygon.

<div style="page-break-after: always;"></div>

## 6. Module 7 – Exploring Data Visually

### 6.1 Exploratory data analysis (EDA)
- Understanding data through **descriptive statistics and visualisation** **before** analysing/presenting.
- **Objectives:**
  1. Detect **errors, missing values and unusual observations**
  2. Characterise the **distribution of individual variables** (univariate)
  3. Identify **patterns and relationships** between variables (multivariate)
- **Structural dimensions:** **tall data** = many rows (records). **Wide data** = many columns (variables). The bigger the table, the more likely errors/gaps are. Wide data is harder to explore (many variable combinations).
- Excel tools: **Excel Table** (Format as Table), **filter & sort** (alphabetically, chronologically, by magnitude), **calculated fields** (e.g. Time to Deliver = Delivered − Ordered), derive Year/Month/Day variables, **Total Row**, **conditional formatting** for missing values.

### 6.2 Univariate analysis
- One variable at a time. **Categorical** → PivotTable/PivotChart (frequency distribution), **do not re-sort ordinal data**. **Quantitative** → histogram, box plot.
- **PivotTable**: calculates, summarises and analyses data (comparisons, patterns, trends). **PivotChart**: interactive visualisation of it.
- **Investigate outliers in box plots**: if erroneous → possibly remove. **But do not remove without good cause**, otherwise variability is artificially reduced and the analysis is distorted.

### 6.3 Multivariate analysis – relationships
- **Crosstabulation**: table showing the relationship between **two or more (usually categorical) variables** (for quantitative variables, create bins). In Excel as a PivotTable, filtered interactively with **slicers**.
- **Scatter chart** for two quantitative variables:
  - **Aspect ratio**: ideally **square** (height = width), so neither variable is favoured
  - **Axis scales**: start slightly **below the minimum** and end slightly **above the maximum**
  - **Trendline**: positive slope = positive correlation, negative slope = negative correlation
- **Correlation (r)**: strength of the **linear** relationship, **−1 to +1**. Near 0 = no linear relationship (but possibly **nonlinear**!). Visually: the closer the points cluster around the trendline, the stronger the correlation.
- **Spurious relationship**, possible when:
  - a **third variable (lurking variable)** affects both
  - the data are **biased/not representative**
  - there are too few data to rule out random coincidence
- **Correlation ≠ causation!**
- A **nonlinear trendline** (e.g. polynomial) can reveal a relationship that a linear trendline misses.
- **Categorical variable in a scatter:** a colour per category (separate data series) or **highlight one category** (others grey, no fill) + its own trendline.
- **Scatter-chart matrix**: all pairwise scatter charts of all quantitative variables in one grid.
- **Table lens**: table with horizontal **bars proportional to the values**. Good for **wide and tall data**. **Sort descending** by one variable, then:
  - large → small pattern in another column = **positive** relationship
  - small → large pattern = **negative** relationship
  - no pattern = **no** relationship

### 6.4 Missing data
- **Legitimately missing**: naturally missing (question not relevant, e.g. after "N/A")
- **Illegitimately missing**: respondents don't answer, drop out, a sensor fails
- **3 options** for illegitimately missing data:
  1. **Discard** observations/rows with missing values
  2. **Fill in** missing values with estimates (imputation)
  3. Treat missing data as a **separate category** (categorical variables only)
- **First** try to find the actual value (check the source, determine it logically).

| Type | Meaning | Example | Handling (rule of thumb) |
|---|---|---|---|
| **MCAR** – Missing Completely At Random | Missingness is unrelated to the value **and** to other variables | Corrupted file, random sensor failure | Discarding causes no bias (only less data); simple imputation ok |
| **MAR** – Missing At Random | Missingness is related to **another variable** | Men less likely to give their job title | Estimate using the other variables (e.g. group means); simply discarding can bias |
| **MNAR** – Missing Not At Random | Missingness is related to **the missing value itself** | Low education → education question left blank | Most problematic: discarding/imputation biases; separate category, investigate cause, communicate openly |

- **Explore patterns of missing data**: e.g. compare frequencies by distribution centre **with vs. without** a rating.

### 6.5 Time series data
- A **line chart** shows:
  - **Trend**: long-run pattern over several periods
  - **Variability**: difference from period to period
  - **Seasonality**: regularly recurring pattern (hourly, daily, monthly, quarterly …)
- **Temporal frequency**: the rate at which data are displayed on the horizontal axis (annual/quarterly/monthly). **Lower frequency smooths** (hides seasonality); higher frequency shows more variability.
- **Detecting seasonality**: overlay **one line per year** (x = month/quarter).
- A (linear) **trendline** uses **all** data. For time series, a **moving average** is often better: average of the last x periods; uses only data **up to the current point in time** and **none from the distant past**.
- **Trellis display**: same size/scales/formatting, only the data differ (e.g. 3-, 6-, 12-month moving average).
- **Stacked data** (all values in **one** column, another column identifies the group) vs. **unstacked data** (each group in **its own column**). Rearrange depending on the chart.
- **Sparklines**: mini line charts **in a cell**; show the **trend, not the magnitude**; no axes/labels; place next to the data. *Insert → Sparklines → Line*.
- Box plots also work for time series (from unstacked data, e.g. per year).

### 6.6 Geospatial data

| | Choropleth map | Cartogram | Equal-area cartogram |
|---|---|---|---|
| **What** | Areas shaded by value (colour/shade/symbols) | Areas **distorted in proportion to the variable** | All areas **the same size**, colour = value |
| **Strengths** | High-level patterns by region; **relative** comparisons; familiar (weather map) | Uses the audience's geographic knowledge; prevents large, sparsely populated areas from dominating | Balanced, every region equally visible, position still recognisable |
| **Weaknesses** | Large areas dominate visually; coarse **granularity** hides variation within areas and suggests abrupt changes between them; **absolute values** mislead | Strong distortion can make the map unrecognisable | Area has no meaning |
| **Good when** | Variable fairly constant within regions; **density/rate-based** values; regions roughly equal in size | – | Many small and large regions |

### 6.7 Workshop Activities Module 7 – Solutions

**Activity 1 – PivotChart with slicers (EJB)**: $ Sales → Values, Distribution Centre + Year Ordered → Rows, New Customer? → Columns, stacked column, insert slicers, hide field buttons, axis in thousands. Answer the questions with the slicers; percentage change = **(new − old) / old**.

**Activity 2 – Red wine study (Copenhagen)**
- **No**, causation cannot be inferred: it is an **observational study** that only shows a **correlation**. **Lurking variables** such as **income and education** (wine drinkers were richer and better educated) probably affect both wine consumption and health (diet, exercise, healthcare).
- **Improvement:** a **randomised controlled experiment** (random assignment to wine/no wine), or control for confounders (stratify by income/education and compare), a larger and representative sample.

**Activity 3 – Body fat % vs. exertion level (1–4, ordinal)**
- Exertion is **ordinal with only 4 values**, so a scatter chart is poor (occlusion, points in 4 rows). Better: **box and whisker chart of body fat for each exertion level** (distribution per group comparable) or a **jittered strip chart**; simpler: column chart of average body fat per level (in natural order 1–4).

**Activity 4 – Correlation analysis of wide data (dozens of variables)**
- **Scatter-chart matrix**: shows all pairwise relationships, but becomes very large/unreadable with dozens of variables.
- **Table lens**: good for **wide and tall** data; sort by a variable and read the patterns; remains readable when zoomed out.
- Recommendation: table lens (or a correlation heat map) for screening, then scatter charts for the most interesting pairs.

**Activity 5 – Types of missing data**
- a) Education missing more often for low education → **MNAR** (missingness depends on the missing value itself)
- b) Job title missing more often for men → **MAR** (missingness relates to **another** variable, gender)

**Activity 6 – Univariate EJB**: PivotChart with "% of Grand Total" for Category and New Customer (relabel "Existing"/"New") and describe the findings.

**Activity 7/8 – NYC scatter with borough series & highlighting Queens**
- Sort by borough, each borough as its own series (*Select Data → Add*). Then all except Queens **grey, no fill**, trendline **for Queens only**.
- Interpretation: in **Queens the positive relationship** between % college graduates and median rent is **weaker** (flatter trendline, points more scattered) than across all boroughs.

**Activity 9 – Table lens Bravman**: sort descending by Purchase Amount, data bars (*Conditional Formatting → Data Bars*) on each column, then read positive/negative/no relationship for wait time, age and credit score.

**Activity 10 – Smartphone sales (annual/quarterly/monthly)**
- **Annual**: long-term trend clear, seasonality invisible (smoothed)
- **Quarterly**: seasonality (e.g. Q4 peaks) visible, trend still visible
- **Monthly**: maximum variability/detail, but more "noise"; monthly patterns visible
- Conclusion: different temporal frequencies reveal different patterns, so check several views.

**Activity 11 – Moving average trendline (pear juice)**: right-click the series → *Add Trendline → Moving Average, Period 3* (then 6, 12) → trellis display. Longer period = smoother but reacts more slowly.

**Activity 12 – Umbrella sales**: line chart + **4-period moving average** (quarterly data → smooths out one year's seasonality). Seasonality: 5 lines (one per year, x = Q1–Q4). If highs/lows recur in the same quarters every year, there is seasonality.

### 6.8 Possible Exam Questions Module 7
- Objectives of EDA; tall vs. wide data.
- Classify MCAR/MAR/MNAR from examples and justify (very likely!).
- List options for handling missing data.
- Correlation vs. causation; lurking variable; critique a study (red wine).
- Which visualisation for relationship X (ordinal vs. quantitative, wide data)?
- Interpret a table lens.
- Trend/variability/seasonality; temporal frequency; moving average vs. linear trendline.
- Choropleth vs. cartogram: strengths/weaknesses.
- **File:** PivotChart + slicers; scatter with categories + trendline; moving average; sparklines.

<div style="page-break-after: always;"></div>

## 7. Module 8 – Explaining Visually to Influence with Data

### 7.1 Know your audience
- **Storytelling** = building a meaningful, memorable narrative from data that is likely to influence the audience.
- Two dimensions:
  1. **Insight needs**: **high-level understanding** (simple charts, main message) vs. **detailed understanding** (more sophisticated visualisations, prompts discussion)
  2. **Analytical comfort**: **low** (simple charts, one key insight, low cognitive load) vs. **high** (detailed, statistical charts)
- Examples:
  - **Chan Life Insurance:** **sales agents** need high-level understanding (line chart of total quote response time, projections dashed). **Underwriters** need detail (clustered column by individual task).
  - **General Hospital:** **low** comfort → column chart of average satisfaction. **High** comfort → box and whisker chart.
- **Chart matrix** (my own assignment following the course logic, textbook p. 292; hint given: scatter = detailed + high comfort):

| | Low analytical comfort | High analytical comfort |
|---|---|---|
| **Only high-level insights** | Simple bar/column charts, line charts, pie charts (few categories), summary tables, dot matrix charts, BANs | Slope charts, bubble charts, geographic information systems (maps, choropleths), tree maps |
| **Detailed insights** | Clustered & stacked bar/column charts, cross-tabulation tables | Scatter charts, scatter-chart matrix, box & whisker, histograms, strip charts, violin charts, Sankey charts |

### 7.2 Know your message – what helps the decision maker?
- Know the data well: what they mean to the audience, what **limitations** they have and how these affect the insights.
- Decision makers often have to: weigh many quantitative + qualitative factors, consider the **impact on stakeholders**, decide with **incomplete information** and under **time pressure**.
- Therefore: **clear, quick to interpret, high data-ink ratio, no chart junk.**

### 7.3 Empathising with data
- **Empathy** = the ability to understand and share the feelings of others; data often represent **real people**.
- **Two challenges + strategies:**
  1. **Large numbers** lose meaning (people can only picture groups of up to about 100):
     - **convert into something familiar** ($357 million lottery = $171,000 per week for 40 years)
     - **no scientific notation** (millions/billions instead of 10⁶/10⁹)
     - give **context**, e.g. a **dot matrix chart** (40 million lost jobs ≈ 7 × Ohio's labour force)
  2. **Aggregate statistics** hide individual cases:
     - **individual case/persona** with a name and characteristics, **pictures** (shelter dog in a stacked column chart), present cluster results as personas
- **BAN – Big Associated Number**: a number in very large font (preattentive attribute **size**) for emphasis.

### 7.4 Storytelling with charts
- **Choose the correct chart**: e.g. a **slope chart** instead of a clustered column chart when the **change between two points in time** for each entity is the message (Opening Horizons: Durango ↑, Salida ↓ becomes obvious immediately).
  - **Slope chart** = line chart of connected pairs of points for multiple entities. Excel: line with markers → **Switch Row/Column** → remove gridlines/legend/vertical axis, labels on the left (name + value) and right (value).
- **Preattentive attributes** for the story: **colour** highlights one line (Florida in the subprime crisis, the rest grey), **size** via a BAN.
- **Three elements of a story** (HBR video): **set-up → conflict → resolution**.

### 7.5 Aristotle's rhetorical triangle

| Element | Meaning | In data vis |
|---|---|---|
| **Ethos** | **Credibility** | Accurate data, nothing distorted/hidden, disclose data source, assumptions and data manipulation, present alternative interpretations |
| **Pathos** | **Emotion** | Create empathy: individual cases, personas, pictures |
| **Logos** | **Logic** | A clear, logical argument: how data and analysis lead to the insights and why these enable better decisions |

### 7.6 Freytag's pyramid (5 parts)
1. **Introduction (exposition)**: problem, context, why it matters; introduce the protagonist/persona
2. **Rising action**: tension/problems build up (data show the problem)
3. **Climax**: peak of the conflict, the key insight
4. **Falling action**: recommendations/path to a solution
5. **Conclusion (resolution)**: costs/benefits of the recommendations, assumptions, limitations
- **Mistake** (Hawaiian Bell): presenting **chronologically by analysis steps** (data cleaning → EDA → results). This is boring and the message comes too late.
- **SCQA framework** (video): **Situation, Complication, Question, Answer** + pyramid principle (key message first).

### 7.7 Storyboarding
- A visual outline of the main points of a story; **modular**, sections can be reordered.
1. **Low-tech: sticky notes (Post-its)**: easy to add/reorder/remove, encourages a methodical approach, stops you jumping to finished slides too early
2. **High-tech: PowerPoint**: create slides along the story stages (Freytag), use the **slide sorter view** to reorder and get an overview. Develop the storyboard **separately** from the final presentation.

### 7.8 Special charts in Module 8
- **Funnel chart** (*Insert → Waterfall, Funnel, Stock, Surface or Radar → Funnel*)
- **Stock chart high-low-close** (select date + high, low, close; keep close labels, delete high/low labels, close markers black 3 pt)
- **Waterfall chart** (total column: *Format Data Point → **Set as total***)
- **Dot matrix chart** (copy the ● symbol into cells, narrow the columns, gridlines off, context via cell fill = **enclosure**)
- **Slope chart**, **BAN**

### 7.9 Workshop Activities Module 8 – Solutions

**Activity 1 – Chan Life underwriters**
- Problem: a clustered column chart with many tasks × 6 time points is cluttered; the eyes jump between legend and columns.
- Alternative: **multiple line chart** (one line per task, x = month) with **labels directly at the end of each line** (no legend), **projections dashed or lighter** (Gestalt connection/similarity), possibly highlight one line. Or a **stacked column** for total time + composition, or small multiples.

**Activity 2 – Funnel chart (data science hiring: 51 → 37 → 12 → 7 → 4)**
- Other uses: **sales pipeline** (leads → opportunities → deals), **website/e-commerce conversion** (visit → cart → purchase), marketing campaigns, university applications, onboarding processes, support ticket escalation.

**Activity 3 – Slope chart Opening Horizons** (previous → current year)

| Location | Previous | Current | Change |
|---|---|---|---|
| Durango | 341 | 432 | **+91 (+26.7 %)**, now the largest location |
| Salida | 395 | 360 | **−35 (−8.9 %)**, loses first place |
| Pagosa Springs | 302 | 298 | −4 (−1.3 %) |
| Montrose | 198 | 202 | +4 (+2.0 %) |
| Gunnison | 164 | 150 | −14 (−8.5 %) |

- Insight: Durango and Salida moved in **opposite directions**. Durango overtakes Salida; the others remain largely stable.

**Activity 4 – ESU engineering salaries (slope chart)**

| Major | Starting | 5 years | Increase |
|---|---|---|---|
| Chemical | $72,500 | $91,400 | +$18,900 (+26 %), **stays highest** |
| Electrical | $64,800 | $87,400 | **+$22,600 (+35 %), largest increase**, overtakes Computer |
| Computer | $68,400 | $83,600 | +$15,200 (+22 %) |
| Mechanical | $62,900 | $77,100 | +$14,200 (+23 %) |
| Industrial | $57,400 | $74,000 | +$16,600 (+29 %), overtakes Civil |
| Civil | $61,000 | $70,300 | **+$9,300 (+15 %), smallest increase**, becomes the lowest |

- Insight: all salaries rise. The ranking changes (lines cross): Electrical and Industrial catch up, Civil falls behind.

**Activity 5 – Dot matrix (40 million jobs)**: 20 × 20 = 400 dots, **1 dot = 100,000 jobs**. Ohio's labour force ≈ 58 dots (≈ 5.8 million) shaded blue. Text: "almost 7 times larger than the total labour force in Ohio".

**Activity 6 – Drinking water (663 million people)**
- a) **BAN** "663 million" in large font next to/above the bar chart
- b) Dot matrix: **25 × 26 = 650 + 13 = 663 dots**, ● = 1 million
- c) Colours by region + legend (categorical colour scheme)
- d) Shade **330 dots** (≈ US population) with fill colour = **Gestalt principle of enclosure**, label it ("≈ population of the USA")

**Activity 7 – Stock chart Verizon**: shows the closing price trend and daily **volatility** (length of the high-low line).

**Activity 8 – Waterfall Gossamer**: mark the total column as **Set as total**. Shows how monthly gross profits add up to the total (positive vs. negative months).

**Activity 9 – Air Transat storyboard (Freytag)**
1. **Introduction**: July 2017, two Air Transat flights diverted to Ottawa due to weather. Introduce a persona (e.g. a family with a toddler on board).
2. **Rising action**: passengers stuck **on the tarmac for over 4 hours**, on one flight without food, water or air conditioning. Frustration and health risk grow (data: waiting time, temperature, number affected).
3. **Climax**: a passenger calls **911** to force the airline to act. Media coverage.
4. **Falling action**: CTA investigation; airline and airport **blame each other**; the airline is **fined/held responsible**.
5. **Conclusion**: recommendations (clear tarmac-delay protocols, provision of food/water after X hours, clear responsibilities, communication) with costs/benefits, assumptions and limitations.
- In PowerPoint slide sorter view, 1–2 slides per stage. Build in ethos/pathos/logos.

### 7.10 Possible Exam Questions Module 8
- How do audience needs and analytical comfort affect chart choice? Assign examples.
- Two challenges in creating empathy + strategies.
- What is a BAN / dot matrix chart / slope chart, and when do you use them?
- Explain the rhetorical triangle (ethos, pathos, logos) and apply it to a case.
- Freytag's pyramid: 5 stages, design a storyboard for a case (Air Transat!).
- Storyboarding: sticky notes vs. PowerPoint.
- **File:** slope chart (Opening Horizons / ESU), funnel, waterfall (set as total), stock chart, dot matrix + BAN.

<div style="page-break-after: always;"></div>

## 8. Module 9 – Data Dashboards

### 8.1 What is a data dashboard?
- A visualisation tool that gives **multiple outputs** and may update **in real time**. It gives decision makers timely information on **KPIs (key performance indicators)** at the **"moment of value"** when decisions are made.
- KPIs are aligned with **organisational goals** and differ by organisation (e.g. financial position, inventory on hand, pending orders, project progress, customer service metrics).

### 8.2 Principles of effective dashboards
1. **All KPIs** for one aspect on **a single screen** ("at a glance")
2. Better **several dashboards** of related KPIs than scrolling
3. KPIs must **convey meaning quickly and clearly** and relate to the **user's decisions**
4. All components follow the **principles of good data vis** (data-ink, Gestalt, preattentive …)
5. **Use colour judiciously**: to highlight values and differentiate categories

### 8.3 Areas of application (with typical KPIs)
- **Investment**: current price, rate of return, relative risk vs. the market, share per industry
- **Manufacturing**: quantity produced, quality, production speed, frequency of problems (machine downtime, returns, missed targets)
- **Marketing**: quantities sold/delivered, success rate of sales calls, revenue/prices, advertising spend, exposure/response, customer satisfaction
- **Human resources**: number of employees, churn (turnover), length of employment, performance/satisfaction, absenteeism, training, reasons for leaving
- **Technical support**: type of problem, response/resolution time, outstanding/persistent issues, downtime, maintenance
- **Personal fitness/health**: pulse, blood pressure, weight/BMI, steps, calories, blood sugar
- **Donor**: number/value of donations, contacts, expenditure, conversion rate, cash flow, campaign status
- Others: crime, school performance

### 8.4 Dashboard taxonomies

| Criterion | Type | Characteristics |
|---|---|---|
| **Data updates** | **Static** | cheap and easy to build, updated **manually** and infrequently (laborious), good for **slowly** changing KPIs |
| | **Dynamic** | more effort to build, updates **automatically** and frequently, good for **rapidly** changing KPIs |
| **User interaction** | **Non-interactive** | user cannot customise, good for infrequently changing data |
| | **Interactive** | user filters/customises: **drill-down** (more detail on one element), **hierarchical filtering** (nested filters, e.g. country → region → store), **time-interval widget** (choose the time period), **customisation tools** (show/hide variables/categories) |
| **Organisational function** | **Operational** | **lower-level managers**, rapidly changing critical conditions, **real-time** updates |
| | **Tactical** | **mid-level managers**, assess strengths/weaknesses, develop strategies, less frequent updates |
| | **Strategic** | **executives**, status of KPIs for overarching objectives, recurring but less frequent |
| | **Analytical** | **analysts**, investigate trends, predict outcomes, insights in large data volumes |

### 8.5 Dashboard design & development
- **Purpose**: support operations, decision-making and strategic planning. Possible objectives: track KPIs/monitor processes, assess goal attainment, develop insight, share information, measure performance, forecasting/exploration.
- **Users' needs**: design for **specific users and tasks**. The team must understand what users need and how this supports the organisation's objectives → determines **what information** and **how** it is presented. **Involve users from the start.**
- **Display**: appropriate chart types, preattentive attributes/Gestalt/colour, **practical layout** (related charts adjacent), avoid overcrowding (subsets, interactive tools), consider **device, ambient lighting, screen size and resolution**.
- **Context** for KPIs: variation over time, comparison with a **goal**, comparison **internally** (divisions, regions) or **externally** (customers, competitors, industry).
- **Engineering**: arrange charts to minimise **eye travel**; maintenance and effectiveness assessment; plan for future objectives/KPIs/data sources.
- **Organisation (Excel)**:
  - Data source in **its own worksheet**
  - Dashboard should **not draw directly** from the source data; extract required data into a **separate** worksheet (PivotTables)
  - Users must not make **permanent changes** (protect the sheet, hide helper sheets)
- **Testing**: test at every step. Otherwise: faulty product leading to poor decisions, costly revisions, loss of credibility. **Final review**: test all slicer combinations, let users test (user friendly, functions and outputs as expected), set up an ongoing monitoring/revision process.

### 8.6 Common mistakes in dashboard design
1. Ignoring the organisation's needs/objectives (important info missing, unimportant info dominating, **users not involved**)
2. Ignoring the **environment of use** (device, lighting, touch/projector)
3. Charts/tables **poorly positioned** (related ones not adjacent)
4. **Inappropriate chart types**
5. Ignoring design principles for individual components
6. **Too cluttered or too sparse**
7. **Unattractive** design (e.g. garish background colour, script font)
8. Not considering **future needs**

### 8.7 Excel tools for dashboards
- **PivotTables** (filters), **PivotCharts** (interactive charts), **slicers** (filter buttons)
- **Connected slicers**: one slicer controls several PivotCharts. *Select slicer → Slicer tab → **Report Connections** → tick the PivotTables*
- Hide field buttons (*Hide All Field Buttons*), axis in thousands, **Don't move or size with cells**, disable autofit column widths, gridlines off, **consistent colour coding** (*File → Options → Advanced → Properties follow chart data point*)
- **Protection**: slicer "Disable resizing and moving" + not locked; *Review → Allow Edit Ranges*; *Protect Sheet* with "Use PivotTable & PivotChart" + password; hide helper sheets
- **EJB dashboard** (mid-level operations, i.e. **tactical**, **dynamic & interactive**): KPIs = **total $ sales** and **average delivery time**. Charts: (1) stacked column sales by DC × year × new/existing, (2) line chart sales by year/month × category, (3) clustered column sales by year × flavour × category, (4) clustered bar avg. delivery time by DC × year, (5) PivotTable sales by category/flavour/DC/date. Layout: charts 1 + 3 (sales by year), 1 + 4 (DC level), 2 + 3 (category level) adjacent; table at the top.

### 8.8 Workshop Activities Module 9 – Solutions

**Activity 1 – Improve the alternative EJB dashboard** (image: garish yellow background, script title, small charts at the bottom, large slicer area)
- Neutral/dark **background** instead of garish yellow (contrast, less distraction)
- Sans-serif **title** instead of script font (legibility)
- **Larger charts**; smaller, more compact slicers placed **next to their charts** (proximity, less eye travel); possibly **connected slicers** so fewer are needed
- Related charts adjacent, table at the top
- **Consistent colour coding** (new/existing, juice/smoothie, years) across all charts
- Simplify crowded horizontal axes (e.g. quarters instead of days), increase data-ink ratio

**Activity 2 – Service vs. product satisfaction per DC over 3 years**
- a) **Scatter chart**: x = avg. service rating, y = avg. product rating, **each point = one distribution centre**, **one series/colour per year** or a **trellis display** (3 scatters with the same scales, one per year). Reason: relationship between two quantitative variables; trellis allows comparing years. Plus a PivotTable with both averages by DC × year.
- b) Add a PivotChart + Year slicer (**connected** to the existing Year slicer), place it next to the DC chart (chart 4), table next to/below the existing table. Keep everything on **one screen**, shrink other elements if necessary.

**Activity 3 – Additional manufacturing KPIs**
- **OEE (overall equipment effectiveness)**, scrap/defect rate, first-pass yield, capacity utilisation, cycle time/throughput time, on-time delivery, inventory level/turnover, cost per unit, safety incidents, energy consumption, mean time between failures (MTBF), changeover time, labour productivity, customer complaints.

**Activity 4 – Build the EJB dashboard**: steps see Appendix A (PivotChart & PivotTable, slicers, Move Chart, Report Connections, Protect Sheet).

### 8.9 Possible Exam Questions Module 9
- Define data dashboard and KPI; principles of effective dashboards.
- Explain taxonomies: static/dynamic, interactive/non-interactive (drill-down, hierarchical filtering …), operational/tactical/strategic/analytical; assign them to a scenario.
- Suggest KPIs for an area (manufacturing, HR, marketing …).
- Design considerations (purpose, user needs, display, context, engineering, testing).
- Common mistakes; critique and improve a dashboard.
- **File:** create a PivotChart + slicers, connect slicers, dashboard layout.

<div style="page-break-after: always;"></div>

## 9. Module 10 – Telling the Truth with Data Visualisation

### 9.1 Missing data & data errors
- Poor data quality → misleading visualisations → poor decisions. Deal with **missing data first, then errors**.
- **Finding missing data in Excel:**
  - **Sort** (blank cells end up at the bottom)
  - **Conditional formatting** (*Home → Conditional Formatting → Highlight Cells Rules → More Rules → Format only cells that contain → **Blanks***)
  - **`=COUNTBLANK(C2:C457)`** per variable
  - Filter (blanks)
- **Data errors** (causes: manual entry mistakes, miscalibrated sensors) are found via:
  - **Summary statistics** (`MIN`, `MAX`, `AVERAGE`) → unrealistic values (Blakely Tires: tyre life of 601 months instead of 60.1; tread depth of 16.7/12 exceeds a new tyre; 0.0 = undrivable)
  - Sorting, frequency distributions, **histograms**
  - **Scatter charts** → also **non-extreme** errors (points that don't fit the relationship)
- Be sure a value is wrong first → **combine several methods**. Then correct logically (601 → 60.1) or treat as missing.

### 9.2 Biased data
- **Bias**: the sample does not represent the intended population (drawn **non-randomly**).
- **Selection bias**: the sample is not random and does not represent the population (e.g. a landline-only poll → older respondents; a drink-driving poll outside a bar late at night).
- **Simpson's paradox** (a form of selection bias): a **trend in subgroups reverses or disappears** when the groups are **aggregated** (cause: a lurking variable or unequal group sizes). **Detection:** compare the aggregated scatter chart with one **coloured/disaggregated by group**.
- **Survivor bias**: the sample contains a disproportionate number of observations with a **positive outcome** of a prior event (only the "survivors" are considered). Classic: **WWII aircraft**, only returning planes were analysed; the bullet holes show where hits were **survivable**, so the areas **without** holes should be armoured. Example: successful entrepreneurs have high risk tolerance (the failed ones are missing from the sample).
- **My note:** *selection, survivor (brilliance bias) and Simpson's paradox (confirmation bias)*
- **Artefacts**: artificial patterns caused by deficiencies in data collection; don't confuse them with real **facts**.

### 9.3 Adjusting for inflation
- **Inflation** = general increase in nominal prices over time, measured with a **price index** (price of a basket of goods, e.g. CPI). Choose the index **most closely related** to the type of product.
- **Formula (base year B):**

  **Inflation-adjusted value(t) = Nominal value(t) × Index(B) / Index(t)**

- Slide example: gasoline 1978 = $0.65; index 1978 = 51.9; index 2017 = 211.8 → 0.65 × 211.8 / 51.9 ≈ **$2.65–2.66** in 2017 dollars. Excel: **`=B2*($C$41/C2)`** (absolute reference to the base-year index!)
- The base year can be any year, depending on the desired comparisons (often the most recent year).
- Makeover example: the all-time box-office top 10 looks completely different after adjusting for inflation (older films move up).

### 9.4 Deceptive design

**a) Chart axes**
- **Column/bar charts: the vertical axis should always start at 0** (length = value). A truncated axis **exaggerates differences** (e.g. a 52 % vs. 48 % poll looks like a factor of 3). Exception: negative and positive values in the same chart.
- **Line/scatter charts** (orientation/position): here a **narrower** axis is allowed/desirable to show variability/trend/correlation. Too wide a scale **hides insights** (earth's temperature on a 0–100 °F scale looks flat).
- **Aspect ratio** (width : height): **tall & narrow** (small aspect ratio) **exaggerates** trends, **short & wide** (large aspect ratio) **disguises** trends.

**b) Dual-axis charts**
- Two variables with different units/magnitudes on a **primary and secondary axis**. Hard to read and invites **incorrect comparisons**: intersections and relative heights are meaningless and depend only on the choice of scales, so any desired relationship can be "constructed".
- **Fix:** **two separate charts** (stacked vertically, same horizontal axis), one variable each.

**c) Data selection & temporal frequency**
- The **choice of time period** (start/end date) determines the message (cherry picking).
- **Low temporal frequency smooths** → hides seasonal/cyclical variation (e.g. stock price daily vs. monthly). Collect data as frequently as possible and look at **several frequencies**.

**d) Geographic maps**
- **Absolute numbers** on choropleth maps often just reflect population size (number of people in poverty → large states dark). **Use relative values/rates instead** (poverty **rate** = poverty / population).

### 9.5 Workshop Activities Module 10 – Solutions

**Activity 1 – Java Cup taste data (217 respondents, 0–100 scale)**
- a) **Missing values**: `=COUNTBLANK()` per column, highlight with **Conditional Formatting → Blanks**, sort/filter by column (blanks) → note respondent ID and missing variable. (My note: *Price, Conditional Formatting, Count Blank*)
- b) **Erroneous values**: 0–100 scale, so check `MIN`/`MAX` per column, **sort/filter**, conditional formatting for values **< 0 or > 100** (or non-numbers), optionally histogram/scatter. Flag values like 150, −5 or decimal errors (e.g. 7.5 instead of 75). (My note: *Sort, Filter, min/max*)
- **Model answer:** *"Using COUNTBLANK on each column and conditional formatting for blank cells, respondents X and Y have missing values for …. Sorting each variable and checking MIN/MAX against the valid 0–100 scale shows respondent Z has a value of … for …, which is impossible and therefore likely an entry error."*

**Activity 2 – Assign the bias** (my answers from the workshop)
1. **Dr. Rhine / telepathy → survivor bias**: only those who guessed correctly in every round moved on. With 500 participants, someone wins every round purely by chance. The many eliminated participants are ignored; the conclusion rests only on the "survivor".
2. **Exit poll outside a restaurant late at night → selection bias**: the sample (late-night diners who drink, poll by an alcohol-industry lobby group) is **not random** and not representative of the population; this group is more likely to see drink-driving as unproblematic.
3. **Red wine cohort (40 years) → Simpson's paradox**: the aggregated data show "wine drinkers = healthier", but wine drinkers are **richer and better educated** (lurking variable). Disaggregated by income/education, the relationship may disappear or reverse; aggregating across unequal groups creates the spurious effect.

**Activity 3 – Guaraldi Consultants (scatter + trendline, Simpson's paradox)** – recalculated from `Module 10.xlsx`:

| Group | n | Trendline | R² | Avg. years of service | Avg. vacation hours |
|---|---|---|---|---|---|
| **All** | 111 | **y = −4.26x + 66.48** (negative) | 0.20 | – | 41.5 |
| Junior | 56 | y = 0.56x + 23.48 (**positive**) | 0.04 | 7.0 | 27.4 |
| Senior | 55 | y = 1.33x + 49.49 (**positive**) | 0.01 | 4.7 | 55.7 |

- a) **All together:** negative relationship, i.e. more years of service are associated with **less** vacation.
- b) **Split into junior/senior:** a **positive** (slightly increasing) relationship **within each group**, i.e. the **opposite**.
- c) **Yes, Simpson's paradox**: the trend reverses when aggregated. **Lurking variable = consultant title**: seniors take much more vacation (avg. 55.7 h vs. 27.4 h) but have **fewer** years of service on average (4.7 vs. 7.0). Pooling them creates an apparently negative trend. (Relationships are weak overall, low R².)
- **Excel:** scatter → right-click a point → *Add Trendline* → Linear, *Display Equation* + *R-squared*. For b) sort by title and create two series (*Select Data → Add*), a trendline for each.

**Activity 4 – COVID-19 positivity rate Ohio**
- Problem (my note: "y-axis ratio doesn't fit the x-axis"): **vertical axis 0–100 %**, although values only range between **≈ 4.6 % and 14.5 %**, plus a **short, wide** chart (large aspect ratio) → the trend is invisible.
- a) Improvements: limit the **vertical axis to e.g. 0–16 %**, **make the chart taller** (smaller aspect ratio), smooth daily fluctuations with a **7-day moving average**, a meaningful title with the message (e.g. "Positivity rate fell from ~12 % in April to under 5 % in October"), fewer gridlines.
- b) Data: monthly average April 11.6 % → May 11.1 % → June 7.5 % → July 6.5 % → Aug 5.9 % → Sep 5.2 % → Oct 4.7 %; maximum 14.5 % on 21 Apr 2020. **Clear downward trend.**
- Note: a line chart doesn't have to start at 0 (orientation attribute), but 0 as the lower limit is also fine here.

**Activity 5 – Maximus Fashion headcount vs. revenue (dual-axis)**
- Data: headcount (FTE) 14, 16, 18, 16, 12, 8, 10, 12 · revenue $815k, 828k, 820k, 741k, 721k, 735k, 731k, 728k (Q1–Q8)
- a) **Confusion:** the audience (little data vis experience) compares the **heights of both lines** directly or interprets **intersections**, although the axes have different units/scales. It is unclear which axis belongs to which line. The choice of scales can create any (spurious) relationship.
- b) **Redesign:** **two separate line charts** stacked vertically with the **same horizontal axis (quarters)**: headcount (FTE) on top, revenue ($ thousands) below, clear titles stating the message, direct labels, no secondary axis. Alternative: index both to **Q1 = 100** and show them in one chart.
- Insight: headcount fell from 18 (Q3) to 8 (Q6) and recovered to 12. Revenue fell after Q3 from ~$820k to ~$730k and stayed **flat** despite headcount recovering.

### 9.6 Possible Exam Questions Module 10
- **Activity 1 (Java Cup):** find and name missing and erroneous values in a file (file upload + text) – **very likely!**
- **Activity 2:** assign three studies to bias types and justify – **very likely!**
- **Activity 3:** scatter chart + trendline, then split by group, explain Simpson's paradox.
- Define selection bias, survivor bias, Simpson's paradox + your own example.
- Calculate an inflation adjustment (formula!) and explain why it is needed.
- Recognise a misleading chart (axis not starting at 0, aspect ratio, dual-axis, temporal frequency, absolute values on maps) and propose a redesign.
- **File:** redesign the Ohio chart; split a dual-axis chart into two charts.

<div style="page-break-after: always;"></div>

## 10. Appendix A – Excel How-To Guides (Windows terms, Mac notes)

> **Excel on Mac:** the "+" button (*Chart Elements*) does not exist on Mac. Instead: click the chart → **Chart Design tab → Add Chart Element** (title, axis titles, data labels, error bars, gridlines, legend, trendline). Formatting: right-click → *Format …* opens the side pane. *PivotChart Analyze* is sometimes called *PivotTable Analyze*.
>
> **Formula separators:** English Excel uses commas (`=CONFIDENCE.T(0.05, s, n)`); with German regional settings, use semicolons and decimal commas (`=CONFIDENCE.T(0,05; s; n)`).

**Basic chart clean-up (always do this!)**
1. Set a meaningful title (left-aligned, ideally stating the message)
2. Add axis titles (with units); vertical title horizontal at the top of the axis
3. Remove or lighten gridlines, remove chart border (*Format Chart Area → Border → No line*)
4. Remove legend if only one series; otherwise direct labels
5. Consistent sans-serif font; subtle axis lines
6. Sensible axis bounds (column/bar from 0)
7. Colours: one colour, deliberate highlighting

**Scatter chart + trendline** (very exam-relevant!)
1. Select the x and y columns (x **on the left**)
2. *Insert → Insert Scatter (X,Y) or Bubble Chart → Scatter*
3. Right-click a data point → *Add Trendline* → **Linear** (or polynomial / moving average)
4. In the Format Trendline pane: **Display Equation on chart** + **Display R-squared value on chart**
5. Axis scales: *Format Axis → Bounds Minimum/Maximum* slightly below min / above max
6. Axis titles, title, remove gridlines; ideally **square**
- **Several groups** (e.g. junior/senior): **sort** the data by group → chart for group 1 → right-click *Select Data* → rename the series → **Add** → series name, X values, Y values for group 2 → a trendline for each series
- **Highlight one group**: other series *Format Data Series → Marker → Fill: No fill, Border grey*

**Column / bar / clustered / stacked**: select data → *Insert → Insert Column or Bar Chart* → choose type. Year problem: *Change Chart Type* or *Select Data → Horizontal (Category) Axis Labels = years*. Sorting: sort data first (Data → Sort) or, for a PivotChart, *Sort Largest to Smallest*.

**Line chart**: *Insert → Line or Area → Line (with Markers)*; for numeric x values: *Scatter with Straight Lines and Markers*.

**Histogram**: select the column → *Insert → Insert Statistic Chart → Histogram* → *Format Axis → Bin width / Number of bins / Overflow/Underflow bin*. Alternatively `FREQUENCY` + column chart (gap width 0 %).

**Box & whisker**: select columns (unstacked) → *Insert → Statistic Chart → Box and Whisker*; *Format Data Series*: show mean markers, show outlier points.

**Frequency distribution (categorical)**: PivotTable (field in Rows **and** Values = Count) or `=COUNTIF(range,"category")`; percentages: *Value Field Settings → Show Values As → % of Grand Total*.

**Strip chart / jitter**: sort groups, helper y-column (10/20), scatter, second series via *Select Data → Add*, markers No fill, jitter `=C2+RAND()` as new Y values.

**Error bars (confidence interval)**: column chart → *Chart Elements → Error Bars → More Options → Custom → Specify Value* → positive = negative = cell with the margin of error (`=CONFIDENCE.T(0.05, s, n)`) → text box "95 % confidence interval".

**Prediction-interval lines**: *Select Data → Add* for prediction/lower/upper → *Change Series Chart Type → Scatter with Smooth Lines*; observations: line = No line, marker automatic.

**Choropleth (Filled Map)**: select region + value → *Insert → Maps → Filled Map* (internet required). Colour: *Format Data Series → Series Colour → Sequential (2-colour)* or *Diverging (3-colour)*.

**Heat map**: select the number range → *Home → Conditional Formatting → Color Scales → Blue-White-Red* (diverging) or a single-hue scale (sequential).

**Treemap**: first **sort** by category → *Insert → Insert Hierarchy Chart → Treemap* → *Format Data Labels → Value*.

**Funnel**: *Insert → Insert Waterfall, Funnel, Stock, Surface or Radar Chart → Funnel*.

**Waterfall**: select rows (with Ctrl/Cmd) → *… → Waterfall* → click the total column twice (only that point) → *Format Data Point → **Set as total***.

**Stock (high-low-close)**: select date + high, low, close (in that order) → *… → Stock → High-Low-Close* → data labels → delete high/low labels → close markers black, 3 pt.

**Slope chart**: select range (labels + 2 columns) → *Insert → Line with Markers* → *Select Data → **Switch Row/Column*** → remove gridlines, legend and vertical axis → data labels on the right; left: label → *Series Name* + position Left.

**Dot matrix**: *Insert → Symbol → Geometric Shapes → ●* into a cell → copy across the matrix → narrow column width → *View → Gridlines* off → shade cells with fill colour (enclosure) → title/legend ("● = 1 million").

**BAN**: text box (*Insert → Text Box*) with a large, bold number next to the chart.

**PivotChart + slicers**: cell in the data range → *Insert → PivotChart* (& PivotTable) → drag fields into Values/Axis/Legend → *Change Chart Type* → *PivotChart Analyze → Insert Slicer* → format slicer (number of columns) → *Hide All Field Buttons* → axis *Display Units: Thousands*. **Connected slicer:** *Slicer → Report Connections*.

**Moving average trendline**: right-click the series → *Add Trendline → Moving Average → Period = 3/4/6/12*.

**Sparklines**: target cell → *Insert → Sparklines → Line* → data range.

**Table lens**: sort descending by the main variable → each column *Conditional Formatting → Data Bars* (optionally "Show Bar Only").

**Missing values / errors**: `=COUNTBLANK(range)`, *Conditional Formatting → New Rule → Format only cells that contain → Blanks* (or *Cell Value > 100 / < 0*), *Data → Sort/Filter*, `=MIN()`, `=MAX()`.

**Inflation**: `=B2*($C$41/C2)` → fill down → line chart nominal vs. adjusted.

**Exact colour (HSL)**: *Format → Fill → Solid fill → Colour → More Colours → Custom → HSL*.

**Submitting a file**: *File → Save As* → file type **Excel Workbook (.xlsx)** → **rename** as required → upload → check the upload confirmation.

<div style="page-break-after: always;"></div>

## 11. Appendix B – Formulas & Excel Functions

| Purpose | Formula / function |
|---|---|
| Relative frequency | frequency / n · Excel `=COUNTIF(...)/COUNTA(...)` |
| Percent frequency | relative frequency × 100 |
| Approximate bin width | (max − min) / number of bins |
| Frequencies in bins | `=FREQUENCY(data, bin_upper_limits)` |
| Mean / median / mode | `AVERAGE` / `MEDIAN` / `MODE.SNGL`, `MODE.MULT` |
| Range | `=MAX()-MIN()` |
| Standard deviation (sample) | `STDEV.S` |
| Percentile / quartile | `PERCENTILE.EXC(data, 0.9)` / `QUARTILE.EXC(data, 1)` |
| IQR | Q3 − Q1 |
| Outlier limits | Q1 − 1.5 × IQR · Q3 + 1.5 × IQR |
| Empirical rule | 68 % (±1 SD) · 95 % (±2 SD) · 99.7 % (±3 SD) |
| Margin of error (mean) | t × s/√n · `=CONFIDENCE.T(0.05, s, n)` |
| Margin of error (proportion, 95 %) | 1.96 × √(p(1−p)/n) |
| Confidence interval | estimate ± margin of error |
| Correlation | `=CORREL(x, y)` (−1 … +1) |
| Inflation adjustment | nominal(t) × index(base) / index(t) · `=B2*($C$41/C2)` |
| Percentage change | (new − old) / old |
| Count missing values | `=COUNTBLANK(range)` |
| Jitter | `=value+RAND()` |
| Bin label | `=CONCAT("(",D6,",",E6,"]")` |

---

## 12. Appendix C – Answer Frameworks for Essay Questions

### "Critique this visualisation / How would you improve it?"
Go through this checklist and state **problem → effect → improvement** for each point:
1. **Chart type** suits the goal and data? (pie → bar, area → line, dual-axis → 2 charts, 3D → 2D)
2. **Axes** (column/bar from 0? scale too wide/narrow? aspect ratio? units/titles?)
3. **Colour** (unnecessary, excessive, insufficient contrast, inconsistent, colour-blind friendly, appropriate scheme?)
4. **Clutter / data-ink ratio** (gridlines, border, legend, background, decimals)
5. **Eye travel** (legend instead of direct labels, title alignment)
6. **Text** (title stating the message, sans-serif, legibility)
7. **Audience** (needs + analytical comfort; is the complexity appropriate?)
8. **Truthfulness** (bias, no inflation adjustment, absolute instead of relative values, selective time period)

### Definition question (e.g. 4 marks)
Definition (1) → characteristic/explanation (1) → example (1) → relevance for data vis/decisions (1)

### Comparison question (A vs. B)
Mental table: definition of A / B → when to use A / when to use B → one example each → recommendation for the specific scenario

### File question with interpretation
"The chart shows … (trend/direction). The trendline equation y = …x + … indicates that for each additional unit of x, y changes by about … . R² = … means the relationship is weak/moderate/strong. However, correlation does not imply causation; a lurking variable such as … may explain …"

### Useful phrases
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

## 13. Appendix D – Glossary

| Term | Short definition |
|---|---|
| Aspect ratio | Width-to-height ratio of a chart |
| BAN (Big Associated Number) | A key number displayed in very large font |
| Bin / class | Non-overlapping interval/group in a frequency distribution |
| Cartogram | Map-like diagram with areas distorted in proportion to a variable |
| Choropleth map | Map with regions shaded by the value of a variable |
| Cognitive load | Mental effort required to interpret a visualisation |
| Confidence interval | Range likely to contain the population parameter (estimate ± MoE) |
| Correlation / causation | Linear association / one variable actually causing the other |
| Cross-sectional data | Data collected from several entities at the same point in time |
| Crosstabulation | Table summarising the relationship between two or more variables |
| Data-ink ratio | Proportion of ink used to present data vs. total ink |
| Declutter | Remove non-data ink to increase the data-ink ratio |
| Drill-down | Interactive feature showing more detail on an element |
| Dual-axis chart | Chart with a primary and secondary vertical axis |
| Enclosure / proximity / similarity / connection | The four main Gestalt principles |
| Eye travel | Distance the eyes must move to interpret a visualisation |
| Frequency polygon | Line version of a histogram, used to compare distributions |
| Hue / saturation / luminance | Base colour / amount of grey / amount of black or white |
| Interquartile range (IQR) | Q3 − Q1, the middle 50 % of the data |
| Jittering | Adding small random offsets to points to reduce occlusion |
| KPI | Key performance indicator, a metric aligned with organisational goals |
| Lurking variable | Hidden third variable affecting both variables of interest (confounder) |
| Margin of error | Amount added to/subtracted from an estimate to form a CI |
| Moving average | Average of the most recent x periods, used to smooth a time series |
| Occlusion | Data points hiding each other because they overlap |
| Preattentive attributes | Features processed in iconic memory without conscious effort |
| Prediction interval | Range likely to contain a future individual observation |
| Price index | Aggregated price of a basket of goods and services (e.g. CPI) |
| Seasonality | Pattern recurring over a regular time interval |
| Skewness (left/right) | Lack of symmetry; tail to the left/right |
| Slicer | Button-based filter for PivotTables/PivotCharts |
| Sparkline | Small line chart placed in a single cell |
| Stacked / unstacked data | All values in one column with a group column / one column per group |
| Strip chart | Chart showing each individual value along an axis |
| Survivor bias | Sample over-represents positive outcomes of a prior event |
| Table lens | Table with bars proportional to the values, sorted by one variable |
| Temporal frequency | Rate at which time series data are displayed (daily, monthly …) |
| Trellis display | Set of same-sized charts with identical scales (small multiples) |
| Waterfall chart | Chart showing the cumulative effect of positive and negative changes |
