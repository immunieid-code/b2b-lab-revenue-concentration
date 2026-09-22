# B2B Lab Equipment — 11-Year Revenue Concentration & Risk Diagnosis

A historical revenue and customer-concentration study for **PT Andaru Persada Mandiri**, reconstructing eleven years of purchase-order history (2013–2023) plus a 2025 outlook to diagnose why revenue swings so hard year to year, and how exposed the business is to losing a handful of accounts.

**Tools:** Python (Pandas, NumPy), Excel/Power Pivot for the delivered workbook

---

## Project Overview

PT Andaru Persada Mandiri's 2026 study reconciled separate 2013–2017 and 2018–2023 purchase-order ledgers to show how revenue and customer concentration changed over eleven years. It is a different client from the PT Gagas Envirotek studies. The 58.5% concentration finding applies only to the 2013–2017 portion; the 2025 outlook is a simulation.

## The problem

The business had two spreadsheets of purchase orders going back to 2013 and a gut feeling that revenue was "lumpy," but no consolidated view of *how* lumpy, *who* was driving it, or whether the pattern was cyclical, structural, or just noise. Leadership needed to know how much of their revenue sat on a small number of relationships before deciding where to invest in retention versus new business.

## What I built

- **Consolidated an 11-year PO ledger** (2013–2017 and 2018–2023, plus a 2025 simulation layer) from raw transaction exports into clean annual, quarterly, and monthly revenue series.
- **Year-over-year growth decomposition** to separate a genuine demand cycle from noise — isolating a 2020–2021 boom and the 2022–2023 correction that followed it.
- **Customer segmentation by revenue concentration** (Champions, Loyal High-Value, Potential Growth, At-Risk Big Spender) run independently for the 2013–2017 and 2018–2023 windows, so the client could see whether their revenue base was getting more or less concentrated over time.
- **Risk exposure modeling** quantifying, in revenue terms, what happens if the top segment churns versus the next tier down.
- **A target customer-mix structure** (e.g., Loyal High-Value at 30–35% of revenue, At-Risk under 5%) proposed as the stability goal, not just a diagnosis.

## Key results

- **2013–2017:** 24 of roughly 96 active customers — the Loyal High-Value (17) and At-Risk Big Spender (7) segments — accounted for **58.5% of all revenue**, confirming the concentration risk was not a recent development.
- **2018–2023 year-over-year growth:** +250% (2020), +13% (2021), **-67% (2022), -43% (2023)** — a pattern that read as a boom-and-correction cycle driven by a handful of large project closings, not organic, repeatable growth.
- **Champions held the largest revenue share of any segment in 2018–2023 despite being the smallest by customer count**, while Loyal High-Value was the next-largest contributor — the inverse of a healthy, broad-based revenue mix.
- Diagnosed the business as **over-reliant on single large instrument sales with no recurring-revenue floor**, and delivered a three-layer response: protect the core (lock in contracts with top accounts), convert the middle (grow Potential Growth accounts toward Loyal), and diversify (cap any one segment below 40% of revenue).

## Notes

The cleaned project notebooks are in [`notebooks/2013-2017.ipynb`](notebooks/2013-2017.ipynb) and [`notebooks/2018-2023.ipynb`](notebooks/2018-2023.ipynb). They have no executed outputs. The client's purchase-order ledger and customer-level results are not published, so the notebooks require private inputs before they can run. The 58.5% figure applies to the 2013–2017 portion only; the 2025 outlook is a simulation.
