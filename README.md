# Conversion Funnel & Cohort Retention Analysis

**Goal:** Analyze user behavior from raw event logs to understand conversion funnel performance and retention over time.

---

## 📁 Project Overview

- **Tools:** Google Sheets, SQL (if used), basic visualization
- **Data:** Raw event logs (sign-ups, activations, purchases, etc.)
- **Focus:** Funnel conversion rates and cohort-based retention

---

## 🔍 Key Questions

1. What does the **end-to-end funnel** look like from first event to target action?
2. At which steps do we see the largest **drop-off**?
3. How well do users **retain** over their first weeks/months?
4. Which acquisition cohorts perform better or worse?

---

## 🧠 Approach

1. **Event Cleaning & Structuring**
   - Parsed raw logs into user-level timelines
   - Labeled key funnel steps (e.g., `visit → sign_up → activate → purchase`)
2. **Funnel Analysis**
   - Counted users at each step
   - Calculated step-to-step and overall conversion rates
3. **Cohort Setup**
   - Grouped users into cohorts based on **signup date**
   - Calculated retention (active/inactive) by cohort over time
4. **Visualization**
   - Built a funnel table and charts in Google Sheets
   - Created a cohort heatmap to quickly see retention decay

---

## 📊 Sample Metrics (Example)

- Overall conversion from first event → target action: **X%**
- Highest drop-off between **Step A → Step B** (Y% relative drop)
- Month 1 retention: **Z%**; Month 3 retention: **W%**

*(Replace X/Y/Z/W with your actual numbers.)*

---

## 📷 Preview

`![Funnel Table](assets/funnel_table.png)`  
`![Cohort Heatmap](assets/cohort_heatmap.png)`

---

## 🧪 How to Reproduce

1. Open `/sheets/cohort_funnel_analysis.xlsx` (or the linked Google Sheet).
2. Review the `Raw Data` tab to see the event logs.
3. Explore the `Funnel` and `Cohorts` tabs for formulas and visualizations.
4. (Optional) Run queries in `/sql` to rebuild tables from the raw event log.
