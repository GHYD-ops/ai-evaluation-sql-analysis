# AI Evaluation & SQL Data Analysis

**Self-directed portfolio project · 2026 · Synthetic data**

Two connected learning exercises exploring **bilingual AI conversation evaluation** and **reproducible business data analysis with SQL**. Both use a fictional Saudi gift-store scenario. This repository is a learning sample, not client work or a production system.

## At a glance

| Area | What's included |
| --- | --- |
| AI response evaluation | A 13-exchange simulated business conversation in Saudi Arabic and English, plus a documented quality review |
| Data analysis | 12 SQLite queries across synthetic sales, customer, channel, and complaint data |
| Reproducibility | Python runner, SQL schema, saved outputs, and consistency checks |
| Tools and concepts | Python, SQLite, SQL, CTEs, joins, window functions, data validation, and evidence-based interpretation |

## Explore the work

### 1. Bilingual AI Conversation Evaluation

A fictional business stakeholder answers questions about sales trends, customer behavior, promotions, and operational issues. The exercise progresses from descriptive questions to hypotheses, missing-data checks, and practical recommendations.

- [Conversation transcript](conversation.md) — 13 bilingual exchanges
- [Evaluation notes](evaluation.md) — consistency checks, strengths, weaknesses, and limits of the conclusions

**Scope:** This is a fictional conversation with AI-generated stakeholder responses. It is **not** a formal benchmark, translation assessment, or employer evaluation.

### 2. Saudi Gift Store SQL Analysis

A reproducible SQL companion to the conversation, using invented monthly aggregates for August and September 2026.

- [SQL project overview](saudi-gift-store-sql/README.md)
- [Schema and sample data](saudi-gift-store-sql/schema.sql)
- [12 analysis queries](saudi-gift-store-sql/analysis.sql)
- [Python execution and validation script](saudi-gift-store-sql/run_analysis.py)
- [Query results](saudi-gift-store-sql/results.md)
- [Findings and limitations](saudi-gift-store-sql/findings.md)

The SQL covers joins, aggregations, common table expressions, window functions, rankings, revenue reconciliation, customer mix, and missing-data handling.

## Selected findings from the fictional dataset

| Measure | August 2026 | September 2026 |
| --- | ---: | ---: |
| Revenue (SAR) | 420,000 | 505,000 |
| Orders | 1,240 | 1,430 |
| Average order value (SAR) | 338.71 | 353.15 |

- Revenue increased **20.24%**, while order volume increased **15.32%**.
- Repeat-customer counts fell from **430** to **410**; this does **not** measure cohort retention.
- Late delivery accounted for **62 of 186** complaints across the combined two-month dataset. The records do not identify a complaint month or city.

These are **synthetic figures**, not real business results. See the [detailed findings](saudi-gift-store-sql/findings.md) for what the data can and cannot support.

## Run the SQL analysis

Requires **Python 3.9+**. No external Python packages, API keys, or production database are required.

```bash
git clone https://github.com/GHYD-ops/ai-evaluation-sql-analysis.git
cd ai-evaluation-sql-analysis/saudi-gift-store-sql
python3 run_analysis.py
```

The runner creates an in-memory SQLite database, executes all 12 queries, checks key results, and regenerates `results.md`.

Expected terminal message:

```text
PASS: 12 SQL queries executed; integrity and business checks passed.
Saved results.md
```

A GitHub Actions workflow also checks that the script completes and that the committed results are reproducible.

## Interpretation and data limitations

- Product, city, and sales-channel tables are **separate views of the same monthly revenue**. Their totals must not be added together.
- Instagram and WhatsApp form **one combined channel** in the source data.
- Repeat-customer counts are **not** a cohort retention rate.
- Monthly aggregates cannot identify causes of changes in revenue, profit, or customer behavior.
- Missing city data, including Taif, is treated as **unknown**, not zero.

## Methodology and scope

This self-directed project uses fictional data and AI-generated stakeholder responses. AI tools were also used to prepare parts of the SQL and documentation. The included scripts and outputs make the analysis reproducible and verifiable. This is a learning exercise, not client work or a production system.

---

**Portfolio focus:** Artificial Intelligence · Data Analytics · SQL · Python
