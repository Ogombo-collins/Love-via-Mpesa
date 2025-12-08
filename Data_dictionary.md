# Data Dictionary  
_Synthetic M-Pesa Valentine’s Transactions Dataset_

Each row in the dataset represents a **single synthetic M-Pesa transaction for the month of Februrary 2025**, generated via probability-based simulation.

---

## Time Variables

| Column | Type | Description |
|------|-----|-------------|
| `date` | Date | Transaction date (February 2025) |
| `hour` | Integer | Hour of transaction (0–23) |
| `period` | String | Behavioural phase: `baseline`, `valentine`, `post_valentine` |
| `day_type` | String | Sub-phase (e.g., *Early Planners*, *Panic Mode*, *Valentine’s Day*, *Recovery*) |

---

## Transaction Value & Type

| Column | Type | Description |
|------|-----|-------------|
| `amount` | Float | Transaction amount in KES |
| `amount_category` | String | Spend tier (baseline or Valentine-specific categories) |
| `is_valentine_related` | Boolean | Whether transaction is Valentine-related |
| `is_apology` | Boolean | Indicates apology-driven transfers (mainly Feb 15) |

---

## Geographic Attributes

| Column | Type | Description |
|------|-----|-------------|
| `county` | String | Kenyan county (weighted by economic activity) |
| `location_type` | String | `Urban` or `Rural` |

---

## Behavioural & Demographic Attributes

| Column | Type | Description |
|------|-----|-------------|
| `gender_pattern` | String | Direction of transfer (e.g., `M_to_F`, `F_to_M`) |
| `relationship_status` | String | Synthetic relationship context (Valentine’s only) |
| `is_serial_romantic` | Boolean | Whether sender transacts with multiple recipients |

---

## Event & Context Fields (Valentine’s Only)

| Column | Type | Description |
|------|-----|-------------|
| `event_type` | String | Purpose of transfer (e.g., Dinner, Gift, Transport) |
| `message_type` | String | Simulated transaction message category |

---

## Field Usage Notes

- All behavioural labels are **synthetic constructs**
- No field corresponds to real individuals or real transactions
- Missing values (`NULL`) are expected outside Valentine-specific periods
- Probabilities vary by period to reflect behavioural dynamics

---

## Example Row

```text
date: 2025-02-14  
hour: 21  
amount: 5000  
amount_category: big-spender  
county: Nairobi  
location_type: Urban  
gender_pattern: M_to_F  
period: valentine  
event_type: Dinner  
relationship_status: Dating  
is_apology: False
