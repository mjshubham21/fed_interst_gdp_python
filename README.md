# 🏛️ Federal Reserve Transmission: Interest Rate & GDP Factor Model

**By Shubham Pawar**

---

## 📊 Automated Monetary Policy & Transmission Lag Pipeline

---

## 📌 Overview

This project develops an institutional-grade research engine to quantify the **"Policy Transmission Lag"**—the delay between Federal Reserve interest rate shifts and their measurable impact on the U.S. economy. By synchronizing disparate scales (**Trillions in GDP** vs. **Percentages in Fed Rates**), the model identifies the peak impact window of monetary policy tightening.

This workflow simulates the high-level responsibilities of a **Macro Strategist**, focusing on statistical normalization (Z-scores), time-series lead-lag analysis, and automated executive reporting.

---

## Project Link

[Fed Rates & GDP Factor Research Project](https://github.com/mjshubham21/fed_interst_gdp_python/blob/main/GDP_Fed_Intrest_Project.ipynb)

---

## 🛠️ Tools & Tech Stack

- **Python** (Jupyter Notebook)
- **NumPy & Pandas** — Vectorized Z-score standardization and multi-quarter frequency resampling.
- **Fredapi** — Direct programmatic access to the Federal Reserve Economic Data (FRED) system.
- **Seaborn & Matplotlib** — Advanced diagnostic plotting including rolling correlation heatmaps and regression residuals.
- **Python-pptx** — Automated Generation of Executive PowerPoint decks directly from Python dataframes.
- **Dotenv** — Secure credential management for institutional API keys.

---

## 📂 Data Sources & API Setup

- **Source:** [St. Louis Fed (FRED API)](https://fred.stlouisfed.org/)
- **Series IDs Used:** - `GDPC1` (Real Gross Domestic Product - Billions of Chained 2017 Dollars)
  - `FEDFUNDS` (Federal Funds Effective Rate - Percent)

> ### 🔑 API Configuration
> To execute the research pipeline:
> 1. Duplicate the `sample.env` file and rename it to `.env`.
> 2. Insert your FRED credentials: `FRED_API_KEY=your_api_key_here`.
> 3. The pipeline includes error handling for API timeouts and rate limits.

---

## 🎯 Key Performance Indicators (KPIs) & Statistical Metrics

- 📈 **Standardized Growth (GDP_Z):** Real GDP mapped to a Z-score to identify periods of "Hyper-Growth" vs. "Stagnation."
- 📉 **Standardized Policy (Fed_Rates_Z):** Interest rates centered at a mean of 0 to identify "Restrictive" vs. "Accommodative" cycles.
- ⏱️ **Transmission Lag (0Q to 5Q):** Cross-correlation testing to find the exact quarter where rates exert maximum pressure on growth.
- 🔄 **12-Quarter Rolling Correlation:** Tracking how the relationship between policy and growth changes across different economic regimes.

---

## 📈 Key Insights

- **The 15-Month Peak:** The analysis identifies a **negative correlation of -0.456 at a 5-Quarter Lag**. This mathematically validates the economic theory that Fed rate hikes take approximately 15 months to reach "peak impact" on GDP growth.
- **Regime Decoupling:** During the 2008 Financial Crisis and the 2020 Pandemic, the rolling correlation shows a sharp break, indicating that fiscal stimulus or global shocks overridden traditional monetary policy during these windows.
- **Inverse Sensitivity:** The regression model confirms a statistically significant downward slope; as the **Fed_Rates_Z** moves into restrictive territory (+1.0 to +2.0), GDP growth consistently trends toward its lower historical bounds.
- **Predictive Power:** By shifting the GDP series, the model demonstrates that today's interest rate is a more reliable predictor of *next year's* growth than *today's* growth.

---

## 🔍 Professional Features (The "Analyst" Edge)

- **Statistical Bridge (Z-Scores):** Solves the "Apples vs. Oranges" problem by converting Trillions and Percentages into a universal unit of Standard Deviations.
- **Automated PPTX Reporting:** The script doesn't just analyze data; it automatically generates an **Executive PowerPoint Deck** with the latest charts, ready for a Monday morning investment committee meeting.
- **Lead-Lag Heatmap:** Uses a custom color-mapped correlation matrix to visualize the "Policy Brake" effect as it moves through time, providing a high-fidelity alternative to stagnant tables.

---

## 📚 Data Story

Monetary policy is often described as a "blunt instrument" with long and variable lags. This project transforms that abstract concept into a quantitative model. By automating the data retrieval and standardization process, we can see that the Fed doesn't just "stop" the economy; it sets a process in motion that matures over 12 to 15 months.

**Recommendations for Junior Analysts:**
1. **Watch the Lag:** Do not judge the success of a rate hike in the first quarter; wait for the "Lag 4Q" window for the true economic signal.
2. **Contextualize with Z-Scores:** Always look at the Z-score (+2.0 is a historical extreme) rather than the nominal rate to understand the true level of "Restriction."
3. **Automate the "Slides":** In an institutional setting, the analyst who can generate a 10-slide deck with a single Python command has a massive competitive advantage.

---

## 📇 Contact
**Shubham Pawar** *Data Analytics | Financial Research* [Linkedin Profile](https://www.linkedin.com/in/mjshubham21/)