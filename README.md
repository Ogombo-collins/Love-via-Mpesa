# ❤️ Love in the Time of Mobile Money  
### Valentine’s Day Spending Behaviour Using Synthetic M-Pesa Transactions (Kenya)

---

## 📌 Project Overview

This project explores **Valentine’s Day–driven spending behaviour** in Kenya using a **fully synthetic M-Pesa transaction dataset**.

The objective is not to reproduce real transaction data, but to **simulate realistic behavioural patterns** based on:
- Publicly reported M-Pesa usage statistics  
- Documented Valentine’s spending trends  
- Academic and behavioural research on mobile money usage in Kenya  

The resulting dataset enables rigorous **before–during–after analysis** of how emotionally driven financial behaviour manifests in transaction volume, timing, value, demographics, and recovery dynamics.

---

## 🎯 Objectives

- Demonstrate how **event-driven behaviours** can be modeled using synthetic data  
- Explore **temporal, demographic, and behavioural shifts** during Valentine’s period  
- Provide a **reproducible framework** for behavioural analytics, storytelling, and dashboard prototyping  
- Serve as a **portfolio-quality analytical case study**

---

## 🧪 Data & Methodology Summary

- **Data Type:** Fully synthetic M-Pesa P2P transactions  
- **Simulation Period:** February 2025  
- **Population Size:** 50,000 simulated users  
- **Data Generation:** Python-based probabilistic simulation  
- **Grounding Sources (Conceptual):**
  - Safaricom PLC annual usage averages (2024–2025)
  - Mastercard Love Index (2017–2020 sentiments & trends)
  - Academic and practitioner studies (Busara x CGAP, TIFA, fintech literature)

> ⚠️ No real user data is used. No affiliation with Safaricom or M-Pesa is implied.

---

## 📂 Project Structure

```text
├── notebook/
│   └── love_in_the_time_of_mobile_money.ipynb
├── data/
│   └── synthetic_mpesa_valentine_transactions.csv
├── docs/
│   ├── Data_dictionary.md
│   └── Valentine_synthetic_dataset_logic.md
├── visuals/
│   └── Insights visuals/images of analysis
├── README.md


## ⏱️ Analytical Time Frame

The simulated data covers **February 2025** and is segmented into three periods:

| Period | Dates | Analytical Purpose |
|------|------|-------------------|
| Baseline(Pre-valentine) | Feb 1–10 | Normal spending behaviour |
| Valentine’s Surge | Feb 11–14 | Event-driven behaviour |
| Post-Valentine Recovery | Feb 15–28 | Financial correction & normalization |

This structure enables **before–during–after comparisons**.

---

## ⚙️ Synthetic Dataset Generation Logic

Synthetic transactions are generated programmatically using Python, with **explicit assumptions encoded into the simulation logic**.

### 1️⃣ Baseline Behaviour (Feb 1–10)

- ~1.23 transactions per user per day  
- Normal hour-of-day distribution  
- Typical micro-to-mid-value transfers  
- Balanced gender-direction flows  
- Urban–rural and county weighting based on financial activity intensity  

This period establishes a **reference behavioural baseline**.

---

### 2️⃣ Valentine’s Surge (Feb 11–14)

Valentine’s period assumptions reflect documented gifting and spending patterns:

- ~145% increase in transaction volume  
- Significant increase in transfer amounts  
- Late evening dominance (**7pm–11pm**)  
- Strong gender skew toward **male → female** transfers  
- Increased number of recipients per sender  

Additional simulated attributes include:
- Relationship status  
- Event type (dinner, gifts, transport, experiences)  
- Message sentiment categories  

---

### 3️⃣ Post-Valentine Recovery (Feb 15–28)

Post-event behaviour captures **budget fatigue and emotional repair**:

- Sharp decline in total transfer volumes  
- Feb 15 “apology transfer” spike  
- Apology transfers are ~22% higher in value than baseline  
- Gradual return to baseline transaction patterns  

---

## 📊 Analytical Approach

The notebook follows a structured analytical flow:

- Dataset construction & validation  
- Temporal trend analysis  
- Transaction value analysis  
- Demographic & behavioural segmentation  
- Post-event recovery dynamics  

Each section combines:
- Visualizations  
- Summary statistics  
- Behavioural interpretation  

---

## 🔍 Key Insights

### 📈 1. Transaction Volume Surge Is Highly Concentrated

- Valentine’s week shows a **~145% increase** in transaction volume versus baseline  
- Feb 13–14 alone account for a disproportionate share of transfers  
- A minority of users drive most of the volume increase  

**Insight:** Event-based spending behaviour is highly concentrated among “active romantics".

---

### ⏰ 2. Spending Shifts to Late Evening Hours

- Baseline activity peaks during daytime working hours  
- Valentine’s transactions cluster between **7pm and 11pm**  
- Late-night transactions are also higher in value  

**Insight:** Sending intensifies as the day unfolds, **culminating in evening gifting**..

---

### 💰 3. Transaction Values Increase, Not Just Frequency

- Mean and median transaction amounts rise significantly  
- Spend distribution shifts toward higher value tiers  
- A noticeable increase in “large” transfers during Valentine’s days  

**Insight:** Valentine’s spending reflects **intentional splurging**, not just increased usage.

---

### 👩‍❤️‍👨 4. Clear Gender-Directional Patterns Emerge

* **Male → Female:** **62%**, resulting in an average of KES 4,524
* Female → Male: 28%
* Male → Male: 4%
* Female → Female: 6%, resulting in an average of KES 4,579  

**Insight:** **Traditional gifting patterns persist** — men send more often, while wommen send in higher amounts.

---

### 🌍 5. Urban & High-Income Counties Drive the Spike

* **Top Counties:**
    1.  **Nairobi:** **34%** of Valentine transfers.
    2.  Mombasa: 12%
    3.  Kilifi: 10%
    4.  Kiambu: 9.9%
    5.  Narok:  8.1%
* **Urban vs Rural:**
    * Urban senders: **61%** of transactions, resulting in an average of KES 4,534
    * Rural senders: 32% of transactions, resulting in an average of KES 4,522

> **Insight:** **Urban economic hubs drive digital gifting**, with Nairobi alone handling one-third of Valentine transfers. 

---

### 💔 6. Post-Valentine Recovery & Other Behavourial Insights

- Transaction volumes drop immediately after Feb 14   
- Spending stabilizes gradually rather than instantly
- **The "Last-Minute Lover" Phenomenon**: 9.4% of all Valentine's transfers (represented by 186,837 transfers) occur on February 13 (Reasons: Late birds coming from work or reminded by gazillion Valentine's updates on social media platforms).
- **The "Apology Tour Transfer"**:February 15 shows a spike in transfers with "apology" keywords; about 7,175 messages containing “apology” were sent.Average "apology transfer" amount is KES 3,903.  

**Insight:** Financial behaviour reflects emotional cycles — celebration, regret, correction.

---

### 🔄 7. Serial Romantic Behaviour Exists

- A Total value of serial romantic transfers: KES 626,801,492.65 ($ 483,6431.27)
- Average amount per serial romantic transfer: KES 4,530.98 ($ 34.96)
- Total number of serial romantics: 138,337 users (representing 23% of all users)  sent Valentine's transfers to multiple recipients

**Insight:** Event-driven spending reveals distinct behavioural archetypes (planners vs splurgers).

---

## 🧠 Interpretation Notes

✅ **Appropriate uses:**
- Behavioural research demonstrations  
- Portfolio projects  
- Teaching and learning material  
- Dashboard prototyping  
- Storytelling with data  

❌ **Not appropriate for:**
- Market sizing  
- Revenue estimation  
- Policy or credit decisions  
- Real-world forecasting  

---

## 🔁 Reproducibility & Extensibility

- Parameterized simulation logic  
- Clear assumptions documented in code  
- Easily extensible to other events:
  - Christmas  
  - Back-to-school spending  
  - Elections  
  - National holidays  

---

## 📄 Supporting Documentation

- **DATA_DICTIONARY.md** – Detailed variable definitions and usage notes  

---

## ⚠️ Disclaimer

This project uses **fully synthetic data**.

All values, entities, and behaviours are simulated for analytical demonstration only.  
No affiliation with Safaricom PLC or M-Pesa is implied.

---

## ✨ Final Note

This project emphasizes **how to reason about behaviour using data**, not just how to analyze numbers.

> **The data is simulated — the behaviours are not.**

