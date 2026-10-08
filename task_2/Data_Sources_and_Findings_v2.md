# Task 2 — Data Sources and Key Findings (v2)

**Topic:** Growing Golf in Germany — Participation Dashboard 2016–2025
**Audience:** German Golf Federation (DGV), state golf associations, golf facility operators
**Artefact:** `ICT702_Task2_Golf_Dashboard_v2.xlsx`

---

## 1. How v2 differs from v1

| | v1 | v2 |
|---|---|---|
| DGV data | 2 years (2022, 2025) | **10 years (2016–2025)**, all parsed from the yearbooks |
| Gender series | 2020–2025 | 2012–2025 |
| Demand-side data | none | **Allensbach AWA funnel 2019–2025** |
| International context | none | **R&A benchmark, 17 European markets** |
| Cross-checks | row/column totals | **four independent sources reconcile exactly** |
| Charts | 6 | 6 (two replaced with stronger ones) |

The decisive gain is the ten-year window. Over three years the 41–60 decline looked like a wobble; over ten it is unmistakable, and it changes the recommendation.

---

## 2. Sources (APA 7th)

Deutscher Golf Verband. (2017–2026). *DGV-Statistiken 2016–2025* [Annual statistics, ten editions]. Wiesbaden: Deutscher Golf Verband.

Deutscher Golf Verband. (2026). *Golf in Deutschland erreicht neue Höchstwerte* [Press release, 21 January 2026].

Institut für Demoskopie Allensbach. (2025). *Allensbacher Markt- und Werbeträgeranalyse (AWA 2025)* [Data set, via Statista, IDs 171038, 171039, 171147].

Statista. (2026). *Golfmarkt* [Data set collection: IDs 5148, 6888, 6892, 6894, 6899, 6900, 6904, 214654; data attributed to Deutscher Golf Verband].

The R&A. (2025). *Global Golf Participation 2024* [Report, June 2025, excluding the USA and Mexico].

The R&A. (2021). *Women in Golf Charter — Impact studies* [March 2021].

Statistisches Bundesamt. (2025). *Bundesländer mit Hauptstädten nach Fläche, Bevölkerung und Bevölkerungsdichte am 31.12.2024*.

Statistisches Bundesamt. (2025). *By 2035, one quarter of Germany's population will be aged 67 or over* [Press release No. 446, 11 December 2025].

Huth, C., & Billion, F. (2022). Impacts of the COVID-19 pandemic on German golf – a comparison between club-owned and commercial golf clubs. *Quality in Sport, 8*(1), 21–27. https://doi.org/10.12775/QS.2022.08.01.002

Deutscher Olympischer Sportbund. (2025). *Bestandserhebung* (as at 1 January 2025), cited in DGV-Statistiken 2025.

Okabe, M., & Ito, K. (2008). *Color Universal Design (CUD)*. https://jfly.uni-koeln.de/color/

---

## 3. Reconciliation — worth a paragraph in the report

All ten DGV yearbooks were parsed programmatically. For **every** year 2016–2025, four independently published figures agree exactly:

1. the sum of the age-by-gender table,
2. the sum of the 13 state association rows,
3. the national player series published separately via Statista,
4. the sum of state facility counts against the national facility series.

The R&A reconciles too: for Germany it reports 417,194 adult men + 227,267 adult women + 42,247 juniors = 686,708, matching the DGV 2024 total exactly. The R&A simply separates juniors, which the DGV does not.

This is worth stating explicitly in the methodology section — it evidences data preparation, which Criterion 3 asks for ("all stages from preparation to end product").

---

## 4. Key findings

### Finding 1 — All net growth over the decade came from members aged 61 and over
Total membership rose 52,459 (+8.2%) between 2016 and 2025. The 61+ band alone grew by 53,506 — **102% of the net gain**.

| Age band | 2016 | 2025 | Change | Contribution to net growth |
|---|---|---|---|---|
| 21 to 26 | 20,036 | 32,899 | +64.2% | +24.5% |
| 27 to 35 | 34,861 | 51,385 | +47.4% | +31.5% |
| 41 to 50 | 109,959 | 70,850 | **−35.6%** | **−74.6%** |
| 51 to 55 | 78,623 | 60,319 | **−23.3%** | **−34.9%** |
| 56 to 60 | 67,694 | 93,686 | +38.4% | +49.5% |
| 61 and over | 252,647 | 306,153 | +21.2% | +102.0% |

The 41–55 cohort lost 57,413 members. Young adults grew strongly in percentage terms but from a small base — they replace less than half of what the middle cohorts lost. Growth is a cohort ageing through the system, not new demand.

### Finding 2 — The real constraint is conversion, not interest
Allensbach (2025, population aged 14+):

| Stage | Millions |
|---|---|
| Aware of golf | 69.13 |
| Interested in golf | 6.87 |
| Play golf at all | 3.38 |
| Play golf often | 0.90 |
| DGV-registered | 0.70 |

**9.9 interested people for every registered member.** 3.49 million are interested but do not play; 2.68 million play but are not registered. Interest rose 2023–2025 (6.16m → 6.87m) while membership grew only 2.0% — the funnel leaks at conversion, not at awareness.

This reframes the whole task: the objective is not "make more people want to play golf" but "convert the people who already do".

### Finding 3 — The female share keeps falling despite a relatively good European position
36.8% (2016) → 34.7% (2025), down 2.1 percentage points. In absolute terms women's membership has been flat at roughly 241,000 while men added 47,511.

Context from the R&A: Germany's adult female share of 35.3% is actually among the highest in Europe (Austria 37.6%, Switzerland 35.7%, Netherlands 31.6%, Sweden 24.7%, England 11.5%). So Germany is not failing relative to peers — it is losing an advantage it already holds. That nuance is worth making; it is more defensible than a simple "Germany is bad at this".

### Finding 4 — Germany is far below the northern European ceiling
Registered golfers per 1,000 population, 2024: Iceland 67.0 · Sweden 53.3 · Scotland 38.3 · Ireland 31.2 · Finland 28.0 · Denmark 27.4 · Norway 27.0 · Netherlands 25.0 · England 13.7 · Switzerland 11.8 · Austria 10.4 · **Germany 8.2** · France 6.5 · Spain 6.3.

Germany has 726 courses — more than Denmark, Finland, Norway and the Netherlands combined (786 across all four, with roughly a quarter of Germany's population). Supply is not the binding constraint; conversion is.

### Finding 5 — Domestic penetration varies eighteenfold
Schleswig-Holstein 18.4 per 1,000 → Sachsen-Anhalt 1.0. Berlin/Brandenburg is the standout gap: 6.2 million residents, 4.5 per 1,000, only 19 facilities.

### Finding 6 — The junior pipeline has not recovered
Under-19 membership: 43,953 (2016) → 42,798 (2025), −2.6%. The 7–14 band fell 10.6%. Against Destatis projections — one in four Germans aged 67+ by 2035 — a shrinking junior base compounds the ageing problem rather than offsetting it.

### Finding 7 — Golf grows more slowly than German organised sport overall
The DGV is the eighth-largest federation (686,708 members) but grew +0.7%, against football +3.9%, gymnastics +3.6%, handball +3.6%. Golf is losing relative share.

---

## 5. Recommendations

1. **Target conversion, not awareness.** 2.68 million people play golf without being registered. Converting 1% adds ~27,000 members — four times the 2025 net gain. Flexible and non-club membership formats are the instrument.
2. **Investigate the 41–55 collapse.** 57,413 members lost over the decade, the single largest negative item, and the cohort with the highest willingness to pay. Exit surveys should come before any new acquisition campaign.
3. **Defend the female share.** Germany holds a European advantage that is eroding. The R&A Women in Golf Charter offers a ready framework.
4. **Prioritise capacity by penetration, not by absolute size.** Berlin/Brandenburg and Sachsen/Thüringen combine large populations with very low penetration.
5. **Set the Netherlands as the realistic benchmark.** 25.0 per 1,000 against Germany's 8.2, in a comparably dense, non-Nordic market. Sweden is the ceiling; the Netherlands is the target.
6. **Rebuild the junior pipeline** before the demographic squeeze arrives.

---

## 6. Data quality and limitations

- **VcG** (32,698 members, a nationwide non-club category) is reported separately and excluded from all penetration metrics.
- **Allensbach base mismatch:** the survey covers German speakers aged 14+ in private households; DGV counts registered memberships of all ages. Funnel ratios indicate magnitude, not exact rates. State this.
- **Senior bands overlap:** the five-year bands (325,743) overlap "61 and over" (306,153). Do not add.
- **Facility counts** partly reflect reclassification, not only closures.
- **"Registered membership" ≠ "golfer":** multiple memberships and casual play are not captured — which is precisely what the Allensbach funnel makes visible.
- **R&A figures** are rounded after calculation and use national federation definitions that vary between countries.
- Two 2025 state rows carried a stale editorial note in the source PDF; both reconcile exactly against row and column totals and were retained.

---

## 7. Submission checklist

- Acknowledge AI use per UniSC requirements.
- Two deliverables: Excel file **and** Word report (1,500 words ±10%, APA 7).
- Report structure: purpose ~200 words · theory and principles ~400 · insights and recommendations ~400.
- Submit the report as .docx so Turnitin generates a similarity score.
