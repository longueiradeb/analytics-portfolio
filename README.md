# Analytics Portfolio

Reproducible data-analytics projects, each a self-contained notebook on simulated data.

---

## Product and Marketing Analytics

**[`analytics.ipynb`](analytics.ipynb)** — runs top to bottom in seconds, with
plain-English narrative and a clean chart for every technique.

Worked examples of the core methods across both disciplines — funnel analysis, A/B
testing, cohort retention, segmentation, attribution, incrementality, and marketing
mix modeling. Each is a short, self-contained example.

### What's inside

**Product analytics**
- **Funnel &amp; conversion analysis** — find the biggest drop-off in the signup funnel.
- **A/B testing** — lift, significance, a guardrail metric, and a power/sample-size check.
- **Cohort retention** — retention curves showing where retention settles and whether newer cohorts are improving.
- **Customer segmentation (RFM)** — score users by recency/frequency/monetary and find the high-value segment.

**Marketing analytics**
- **Channel economics** — CAC, ROAS, LTV:CAC and payback per channel.
- **Attribution comparison** — how last-touch vs. first-touch vs. position-based change the story.
- **Incrementality / geo-lift** — why attribution over-credits, measured causally with a holdout.
- **Marketing mix modeling** — estimate adstock + saturation to recover channel ROI with credible intervals, including an offline channel clicks can't see.

### Product analytics vs. marketing analytics

| | **Marketing analytics** | **Product analytics** |
|---|---|---|
| **Core question** | Which spend actually drives signups, and where should the next dollar go? | Where do users drop off, what makes them stick, and what should we build next? |
| **Unit of analysis** | Channel, campaign, dollar | User, event, session, cohort |
| **Typical data** | Spend, impressions, clicks, conversions, geo | Event streams, funnels, feature usage |
| **Headline metrics** | CAC, ROAS, ROI, LTV:CAC, payback, incrementality | Activation, retention, DAU/MAU, funnel conversion, churn, LTV |
| **Signature methods** | Attribution, marketing mix modeling, geo-lift / incrementality, budget allocation | Funnel analysis, cohort retention, A/B testing, segmentation |

### Run it

```bash
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
jupyter lab analytics.ipynb     # or run all cells
```

Everything is seeded and reproducible. Stack: pandas · NumPy · SciPy · statsmodels · Matplotlib.
