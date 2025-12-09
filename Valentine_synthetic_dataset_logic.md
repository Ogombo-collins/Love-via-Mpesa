# Synthetic M-Pesa Valentine’s Transactions Dataset (Kenya)

## Overview

This repository contains a **synthetically generated M-Pesa transaction dataset** designed to replicate realistic spending behaviour in Kenya around Valentine’s Day.

The dataset is created entirely through simulation and **does not contain real customer data**, personally identifiable information (PII), or proprietary Safaricom transaction records.

It is intended for **exploratory analysis, visualisation, behavioural research, and analytical storytelling**, particularly in contexts where real/accurate mobile money data cannot be shared.

---

## Key Characteristics of the Synthetic Dataset

- 🇰🇪 Kenyan mobile money context (M-Pesa)
- ❤️ Valentine’s Day behavioural dynamics
- 📊 Transaction-level synthetic data
- 🧪 Behaviourally grounded, not observational
- 🔁 Fully reproducible Python logic

---

## Data Sources and Conceptual Foundations

The synthetic data generation logic is informed by three main reference categories:

### 1. Safaricom PLC Reports (2024–2025)
- Approx. **37 chargeable transfers per user per month**
- Equivalent to **~1.23 transactions per user per day**
- High-level urban concentration and national usage trends

### 2. Mastercard Love Index (2017–2020)
- Seasonal spending surges around Valentine’s Day
- Late-hour and last-minute (“panic buying”) behaviour
- Increased average transaction values during gifting periods

### 3. Academic Research (Busara × CGAP)
- Mpesa usage behaviour among Kenyan userbase

These sources inform **probability distributions, time dynamics, and behavioural assumptions**, not raw transactional values.

---

## Time Coverage & Behavioural Phases

The dataset covers **February 2025** and models three behavioural phases:

| Phase | Dates | Description |
|------|------|-------------|
| Baseline | Feb 1–10 | Normal M-Pesa usage patterns |
| Valentine’s Surge | Feb 11–14 | ~2.45× volume increase, higher amounts, late-hour peaks |
| Post-Valentine Recovery | Feb 15–28 | Spending dip, apology spike, gradual return to baseline |

---

## Dataset Structure

- Format: CSV file
- Granularity: One row per synthetic transaction
- Key dimensions:
  - Time (date, hour)
  - Geography (county, location type)
  - Transaction characteristics (amount, category)
  - Behavioural context (gender direction, relationship, event type)

For full field definitions and examples, see **`Data_dictionary.md`**.

---

## Intended Use

✅ Suitable for:
- Exploratory data analysis (EDA)
- Dashboards and visual storytelling
- Behavioural finance demonstrations
- Teaching and technical interviews

❌ Not suitable for:
- Revenue forecasting
- Market sizing
- Policy, regulatory, or investment decisions

---

## Reproducibility

The dataset is generated using a **probability-weighted simulation method** implemented in Python.

Key features:
- Configurable user counts
- Explicit behavioural assumptions
- Transparent generation logic
- No dependency on private or proprietary data

---

## Disclaimer

This dataset is **synthetic and illustrative**.

While grounded in real research and public reporting, it should be interpreted as **directionally realistic**, not factual. Absolute values should not be treated as observed M-Pesa activity.

---

## License

This project is released for **educational, research, and demonstration purposes**.

No affiliation with or endorsement by Safaricom PLC is implied.





