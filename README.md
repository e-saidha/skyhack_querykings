README — Flight Difficulty Score

Project Overview

Frontline teams at United Airlines face unequal challenges in turning around flights at Chicago O’Hare (ORD).
Some flights are harder due to short ground time, transfer baggage, or special passenger needs.

This project builds a **Flight Difficulty Score (FDS)** to **quantify flight complexity daily**, replacing ad-hoc manual judgment with a scalable, data-driven framework.



Objectives

1. **Exploratory Data Analysis (EDA)**

   * Understand delay patterns, ground-time constraints, passenger loads, baggage handling, and service requests.
   * Provide clear visualizations of operational bottlenecks.

2. **Flight Difficulty Score Development**

   * Use Machine Learning (Logistic Regression & Random Forest) to model drivers of flight complexity.
   * Create **daily ranks** and classify flights as **Easy, Medium, Difficult**.
   * Generate `test_<teamname>.csv` with flight details, features, and final score.

3. **Post-Analysis & Operational Insights**

   * Identify destinations and operational factors consistently linked with high difficulty.
   * Deliver practical “what-if” scenarios and quantify **economic impact** of interventions.



Repository Structure

```
├── data/                         # (Local only, not uploaded to GitHub)
│   ├── Flight Level Data.csv
│   ├── PNR Flight Level Data.csv
│   ├── PNR Remark Level Data.csv
│   ├── Bag Level Data.csv
│   └── Airports Data.csv
│
├── notebooks/
│   ├── 1_EDA.ipynb               # Exploratory Data Analysis
│   ├── 2_FlightDifficulty.ipynb  # ML modeling & difficulty scoring
│   └── 3_Insights.ipynb          # Post-analysis, what-if, economic impact
│
├── figures/                      # Saved plots for report & slides
│
├── test_querykings.csv           # ✅ Required submission file
│
├── README.md                     # This document
└── requirements.txt              # Python dependencies
```

Tech Stack

* **Python** (pandas, numpy, matplotlib, seaborn, scikit-learn)
* **SQL via DuckDB** for feature engineering & dataset joins
* **Google Colab** as execution environment

## Deliverables

* **Report (PPT/PDF)**: Visual storytelling of methodology, EDA, modeling, and insights.
* **Difficulty Score File**: `test_querykings.csv` with per-flight scoring.
* **Code**: Clean notebooks with step-by-step process (EDA → ML → Insights).
* **Figures**: High-quality charts for replication.

---

## How to Run

1. Open notebooks in **Google Colab**.
2. Upload the 5 provided datasets to `/content/`.
3. Run in sequence:

   * `1_EDA.ipynb` → exploratory visuals & checks
   * `2_FlightDifficulty.ipynb` → builds ML models, outputs `test_querykings.csv`
   * `3_Insights.ipynb` → post-analysis, what-if, economic impact
4. Final artifacts will be saved in the workspace.

---

## Conclusion

This project demonstrates how **data-driven flight difficulty scoring** can replace subjective judgment with a repeatable framework.
By combining **SQL feature engineering, ML modeling, and operational what-if analysis**, we provide both **predictive power** and **business-ready insights**.
The framework equips frontline teams with actionable intelligence to **allocate staff, pre-empt risks, and cut costs**, ultimately enhancing **on-time performance and customer satisfaction**.


*Built with passion during the United Airlines Hackathon by Team QueryKings* 
