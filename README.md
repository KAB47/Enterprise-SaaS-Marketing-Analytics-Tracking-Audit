# Enterprise SaaS Marketing Analytics & Tracking Audit
Excel-Based Marketing Attribution & Channel Efficiency Analysis (Ares, Fictitious Enterprise SaaS / CDP)

Auditing tracking accuracy, calculating channel efficiency KPIs, and building pivot-table dashboards to diagnose a Paid Social decline and guide UK/US budget reallocation — all built with Excel formulas and pivot tables, no hardcoded values.

## TL;DR

A 7-task Excel project on ~25,000 rows of marketing attribution data for a fictitious SaaS/CDP client. Covers tracking-discrepancy auditing, cost lookups, channel efficiency scoring (ROAS, CPP, CAC, AOV), and pivot-table analysis of market performance, Paid Social decline, source efficiency, and UK spend vs. revenue.

## Main Insights Found / Outcomes

- US paid media returns **7.93 ROAS** vs the UK's **1.93**, despite the US spending less overall (~£1.24M vs ~£1.84M)
- **Performance Max** is the strongest-performing paid channel by ROAS (8.21), followed by Paid Search — Generic (5.82)
- **Paid Social ROAS has been declining steadily**, from 4.36 in June to 2.29 in October — a ~48% drop over 5 months
- Within Paid Social, **Snapchat is the most efficient source** (CAC of £12.58) despite receiving only ~2% of the channel's budget, while Facebook absorbs ~70% of spend at a much higher CAC (£42.80)
- UK paid spend and revenue grew together from June to October (£258K→£546K spend, £1.48M→£2.60M revenue), but **ROAS peaked in August (6.40) and fell to an average of ~4.73** in later months — a sign of diminishing returns as monthly spend passed ~£400K
- One day (5 Dec) showed a -152% GA-vs-Ares variance against a normal daily band of roughly ±4-8%, flagging it as a likely tracking outage rather than genuine traffic change

## Background

**The client:** Ares, a fictitious enterprise SaaS provider and Customer Data Platform (CDP).

**The brief:** Work through raw marketing attribution data (~25,000 rows across Date, Market, Channel, Source, Cost, Conversions, and Revenue) using only Excel formulas and pivot tables — no hardcoded values — to answer seven client questions spanning data quality, cost lookups, channel efficiency, and market/trend diagnostics.

**Constraints:** All calculations formula-driven; no reordering, renaming, or deleting sheets; answers entered directly into the provided template.

## Analysis Breakdown

**01 — Attribution & Tracking Accuracy**
Calculated the daily percentage difference between Google Analytics and Ares-reported transactions, then conditionally formatted any day outside ±10% to surface tracking issues at a glance — most days sat within a tight 3-8% band, making the 5 Dec outlier easy to spot.

**02 — Data Preparation & Lookup Analysis**
Combined Channel and Source into a single label with a text formula, then used lookup formulas against a cost table and SUMIFS-style conditions to pull total TikTok spend and total UK Facebook spend directly from the raw dataset.

**03 — Marketing Channel Performance**
Built ROAS, CPP (Cost Per Purchase), CAC, and AOV for every channel from Cost, Revenue, and Conversions, then used the scorecard to identify the best-performing paid channel on each metric (Performance Max on ROAS; Affiliates on CPP/CAC, reflecting its zero-cost organic nature).

**04 — ROAS by Market & Paid Channel (Pivot Table)**
Pivoted Cost, Revenue, and ROAS by Market for each paid channel. The US outperforms the UK on every paid channel, most sharply on Paid Social (9.24 ROAS in the US vs 1.84 in the UK) — pointing to a budget-allocation opportunity rather than a channel-quality problem.

**05 — Paid Social ROAS Trend (Pivot Table + Chart)**
Tracked Paid Social ROAS month-by-month from June to October as spend roughly doubled (£265K→£598K). ROAS fell from 4.36 to 2.29 over the same period, showing efficiency eroding as budget scaled up.

**06 — Paid Social Source Efficiency, October (Pivot Table + Chart)**
Broke October's Paid Social spend down by source (Facebook, TikTok, Snapchat, Pinterest) to compare CAC. Snapchat was cheapest to acquire on despite the smallest budget share, while Facebook — the largest budget line — was the least efficient.

**07 — UK Spend vs Revenue Over Time (Pivot Table + Chart)**
Pivoted UK Cost and Revenue by month to test whether five months of rising paid investment translated into revenue growth. It did overall, but ROAS peaked mid-way through the period and softened as spend kept climbing — consistent with diminishing marginal returns.

## Tools & Stack

- **Microsoft Excel** — formula-driven calculations throughout (no hardcoded values), conditional formatting, VLOOKUP-style cost retrieval, SUMIFS-based conditional totals
- **Pivot Tables & Pivot Charts** — Market x Channel ROAS, monthly Paid Social trend, source-level CAC breakdown, UK Cost vs Revenue over time
- **Dataset** — ~25,000-row marketing attribution export spanning Date, Market, Channel, Source, Cost, Conversions, and Revenue

## Recommendations

1. **Rebalance UK/US paid budget** — shift spend toward the US, where the same paid channels are returning 3-5x the ROAS at lower overall spend
2. **Diversify Paid Social budget away from Facebook** — reallocate toward Snapchat and TikTok, which are acquiring customers at a fraction of Facebook's CAC
3. **Investigate the Paid Social ROAS decline directly** — the month-on-month drop tracks closely with rising spend, suggesting the channel may be scaling past its efficient ceiling
4. **Watch UK paid spend for diminishing returns** — ROAS softened once monthly spend passed ~£400K, so further increases should be tested incrementally rather than scaled uniformly
5. **Flag and investigate the 5 Dec tracking anomaly** — a -152% GA/Ares variance this far outside the normal band is more consistent with a tracking or reporting fault than real traffic change

## Key Skills Demonstrated

- Formula-driven Excel analysis — conditional logic, lookups, conditional formatting, SUMIFS-style aggregation
- Pivot table and pivot chart construction for multi-dimensional comparison (Market, Channel, Source, Month)
- Marketing KPI fluency — ROAS, CPP, CAC, AOV and what each signals about channel health
- Data quality auditing — spotting and explaining anomalies in cross-source reporting
- Translating raw metrics into client-facing commentary and actionable recommendations

---
