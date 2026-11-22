# Bilingual AI Conversation — Evaluation

**Project type:** Self-directed, bilingual, fictional business-analysis simulation  
**Scope:** 13 analyst–stakeholder exchanges in Saudi Arabic and English using synthetic gift-store data  
**Evaluation approach:** Evidence-based qualitative review, not a formal benchmark or an independent assessment of language fluency

## Evaluation criteria

Each criterion is marked **Supported**, **Partially supported**, or **Not assessable** against the content of the transcript. These are descriptive judgments, not measured model performance scores.

| Criterion | Assessment | Evidence and limitation |
| --- | --- | --- |
| Question relevance | Supported | The analyst asks about products, cities, sales channels, customer types, and operational problems in exchanges 1–9. |
| Numerical consistency | Supported | Reported monthly revenue, orders, and breakdown totals align with the [SQL validation](saudi-gift-store-sql/results.md). |
| Bilingual task coverage | Supported | Exchanges 1–7 use Saudi Arabic; exchanges 8–13 use English. A single scripted sample cannot establish language proficiency. |
| Missing-data awareness | Supported | Exchange 4 identifies Taif as unavailable, and exchange 10 requests margins, customer cohorts, and other missing evidence. |
| Channel comparison | Partially supported | Exchange 5 compares website revenue against the **combined Instagram/WhatsApp channel**. Instagram-only effectiveness and conversion are not measurable. |
| Evidence versus hypothesis | Partially supported | Exchange 11 treats promotion and operational effects as hypotheses. The simulated operational statements cannot establish causality. |
| Actionability | Partially supported | Exchanges 12–13 suggest specific investigations, but the dataset does not establish which change would improve profit or retention. |
| Real-world generalizability | Not assessable | The scenario, stakeholder responses, and dataset are fictional. No real business outcomes or independent model benchmark are available. |

## Exchange-by-exchange review

| Exchange | Focus | Evidence check / interpretation |
| --- | --- | --- |
| 1 | Scenario exploration | Product, city, and channel totals reconcile to each monthly revenue total. |
| 2 | Monthly performance | Revenue: SAR 420,000 → 505,000; orders: 1,240 → 1,430. |
| 3 | Product ranking | Flowers lead in revenue both months; lowest category changes from corporate gifts to perfumes. |
| 4 | City comparison | Riyadh and Jeddah values are available; Taif is **missing**, not zero. |
| 5 | Channel comparison | Website revenue exceeds combined Instagram/WhatsApp revenue, not Instagram alone; no conversion-rate comparison. |
| 6 | Customer counts | New customers rise (780 → 910); repeat customers fall (430 → 410). This is not a cohort-retention metric. |
| 7 | Average order value | Computed revenue/orders is SAR 338.71 → 353.15; whole-number figures are rounded. |
| 8 | Operational context | Promotions, stock-outs, and delivery times are **simulated stakeholder statements**, not fields checked by the SQL tables. |
| 9 | Complaints | Late delivery: 62/186 complaints (33.33%); the data cannot establish a September or Abha complaint trend. |
| 10 | Missing evidence | Correctly requests margin, cohort, inventory, delivery, refunds, and marketing-cost data. |
| 11 | Hypothesis | Promotions and fulfillment are plausible explanations, but no causal effect or profit impact is measured. |
| 12 | Prioritization | Fulfillment investigation is a reasonable hypothesis-led priority, not an empirically proven intervention. |
| 13 | Summary | Separates largest absolute gains from percentage growth and distinguishes findings from recommendations. |

## Reproducible consistency checks

The accompanying SQLite project provides [12 queries](saudi-gift-store-sql/analysis.sql), [saved results](saudi-gift-store-sql/results.md), and a [Python runner](saudi-gift-store-sql/run_analysis.py).

- Monthly product, city, and channel totals **each** match reported revenue; they are separate breakdowns of the same amount.
- Average order value equals revenue divided by orders, rounded to two decimal places.
- Riyadh contributes the largest absolute city revenue increase (SAR 40,000); Abha has the highest city percentage growth (34.88%).
- Personalized gifts contribute the largest absolute product revenue increase (SAR 26,000); flowers remain highest by revenue.
- Instagram and WhatsApp are one combined category in this dataset.
- Combined complaints cover two months without time or city identifiers; a regional or monthly complaint rate cannot be computed.

## Interpretation limits

The customer counts do not measure cohort retention. The fictional stakeholder's descriptions of discounts, delivery delays, and stock-outs are scenario context rather than independently verified numerical observations. The aggregate data cannot establish causation, profitability, conversion, or the effectiveness of a proposed business intervention.

## Next steps for a stronger evaluation

- Develop a clearly defined response-level rubric and evaluate a fresh set of independently sampled responses.
- Obtain traffic, conversion, and cost data before comparing channel effectiveness.
- Collect order-level customer identifiers and dates for actual retention analysis.
- Add complaint dates and cities to evaluate geographic and time trends.
- Compare recommendations against measured outcomes rather than scenario assumptions.

## Portfolio summary

> Reviewed a 13-exchange Saudi Arabic and English business simulation, documenting numerical consistency, evidence limitations, and links to a reproducible 12-query SQLite analysis.
