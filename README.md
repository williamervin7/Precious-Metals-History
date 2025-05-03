# Precious Metals History Project

## 📈 Project Summary

This project explores the relationship between **sentiment** and **Close-to-Open price movements** for four metals — **Gold**, **Silver**, **Palladium**, and **Platinum** — from **April 2020 to April 2025**. The analysis includes:

- Sentiment distribution visualizations  
- Yearly price movement trends  
- Correlation between sentiment and price movement  

Additionally, the project contains a **Crisis Event Analysis** covering:

- **9/11 Attacks (2001)**
- **2008 Financial Crisis**
- **2020 COVID Crisis**

These insights highlight safe-haven behavior vs. industrial demand sensitivity.

> **Note:** The `volume` column includes 4796 rows with a value of 0. These likely represent non-trading days or missing data. No action has been taken, but further review may be needed.

> **Sentiment Tool:** VADER (Valence Aware Dictionary and sEntiment Reasoner) — Open-source and licensed under MIT.

---

## 🧠 Sentiment Over Time

### 📊 Sentiment Distribution (04/2020 - 04/2025)

Pie charts illustrate the distribution of **Positive**, **Neutral**, and **Negative** sentiment for each metal:

| Metal      | Chart Location     |
|------------|--------------------|
| Gold       | Top-left           |
| Silver     | Top-right          |
| Palladium  | Bottom-left        |
| Platinum   | Bottom-right       |

**Key Insight:**  
Sentiment types for all metals were closely similar, suggesting low sentiment diversity — likely due to overlapping news cycles or macroeconomic influences.

---

## 📉 Yearly Price Movement Trends (Close - Open)

Line plots display yearly differences between closing and opening prices for all four metals:

- **X-axis:** Years (2020–2025)  
- **Y-axis:** Close-to-Open difference  

**Color Codes:**

- Gold: default color  
- Silver: red  
- Palladium: green  
- Platinum: orange  

### 🔍 Observations

- **Silver:** No clear trend; stable yearly differences.
- **Gold:** Gradual increase over time; lowest in 2020, highest in 2025.
- **Platinum:** Negative in 2020, positive in 2025 — shows upward trend.
- **Palladium:** Sharp peak in 2022 (+1250), declined sharply after.

---

## 🔗 Sentiment and Price Movement Correlation

Sentiment types were converted into numerical values:

- `POSITIVE` → 1  
- `NEUTRAL` → 0  
- `NEGATIVE` → -1  

Then, Pearson correlation coefficients were calculated between sentiment and Close-to-Open price differences.

### 📌 Observations

- **Gold & Silver:** Slight negative correlation — sentiment had almost no predictive power.
- **Palladium & Platinum:** Slight positive correlation — minor alignment between sentiment and price movement.
- **Conclusion:** Sentiment alone is a weak predictor of short-term price movements.

---

## 🧨 Crisis Event Analysis

### 📅 9/11 Attacks (9/5/2001 - 9/21/2001)

- **Gold:** Spiked from $270 to $290 post-9/11; safe-haven demand.
- **Silver:** Mild increase; less pronounced impact.
- **Palladium:** Rose initially, then dropped sharply.
- **Platinum:** Rose steadily; likely supported by industrial/alternative investment demand.

---

### 📅 2008 Financial Crisis (9/5/2008 - 9/25/2008)

- **Gold:** Surged post-crash (from $800 → $875); strong safe-haven asset.
- **Silver:** Rebounded from $10 → $13; significant investor demand.
- **Palladium:** Declined, then slow recovery — less safe-haven appeal.

---

### 📅 COVID Crisis (Mar–Apr 2020)

- **Gold:** Fell sharply, then surged (from $1483 → $1676) — classic safe-haven behavior.
- **Silver:** Sharp drop ($17.4 → $10); delayed recovery.
- **Palladium:** Largest drop ($2797 → $1449), then partial recovery.
- **Platinum:** Sustained weakness (from $858 → $595); sensitive to industrial demand.

---

## 🧭 Crisis Conclusions

Across all three crises:

- **Gold:** Consistently outperforms — strong safe-haven.
- **Silver:** Dual behavior — part safe-haven, part industrial.
- **Palladium & Platinum:** More volatile and industrial-driven; slower recovery.

---

## 📌 Prediction for Future Crises

If another major global crisis occurs:

- **Gold** is expected to surge as investors seek security.
- **Silver** may follow but will reflect industrial pressures.
- **Palladium & Platinum** may decline more heavily due to industrial exposure and slower recovery.

---

## 🛠 Technologies Used

- Python (Pandas, Matplotlib, Seaborn)
- VADER Sentiment Analyzer
- Jupyter Notebook
