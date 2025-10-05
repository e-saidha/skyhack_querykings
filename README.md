# ✈️ Flight Difficulty Score at ORD

[![Hackathon](https://img.shields.io/badge/United_Airlines-Hackathon-blue)](https://github.com)
[![Python](https://img.shields.io/badge/Python-3.8+-green)](https://www.python.org/)
[![Colab](https://img.shields.io/badge/Google-Colab-orange)](https://colab.research.google.com/)

> **Predicting operational complexity for flights at Chicago O'Hare International Airport using machine learning and data-driven insights.**

Developed by **Team QueryKings** during the United Airlines Hackathon, this project analyzes flight operations to calculate difficulty scores that help identify high-risk flights and optimize resource allocation.

---

## 🎯 Project Overview

The Flight Difficulty Score system evaluates multiple operational factors—passenger connections, baggage complexity, gate constraints, weather conditions, and scheduling—to assign each flight a quantifiable difficulty metric. This enables proactive decision-making and improved operational efficiency at one of the world's busiest airports.

### Key Features
- **Predictive Difficulty Scoring**: ML-powered classification of flight operational complexity
- **Comprehensive EDA**: Deep-dive analysis of 5 interconnected datasets
- **What-If Scenarios**: Simulate operational changes and measure economic impact
- **Actionable Insights**: Data-driven recommendations for resource optimization

---

## 📁 Repository Structure

```
├── data/                               # Dataset folder (local only, not tracked)
│   ├── Flight Level Data.csv          # Core flight operations data
│   ├── PNR Flight Level Data.csv      # Passenger booking records
│   ├── PNR Remark Level Data.csv      # Special service requests & notes
│   ├── Bag Level Data.csv             # Baggage tracking information
│   └── Airports Data.csv              # Airport metadata and codes
│
├── notebooks/                          # Analysis workflow (Google Colab)
│   ├── 1_Understanding_Data.ipynb                              # Data profiling & validation
│   ├── 2_Deliverable_1_Exploratory_Data_Analysis_(EDA).ipynb  # Visual analysis & risk identification
│   ├── 3_Deliverable_2_Flight_Difficulty_Score_Development.ipynb # ML modeling & scoring
│   └── 4_Deliverable_3_Post-Analysis_&_Operational_Insights.ipynb # Scenario testing & ROI
│
├── images/                             # Visualizations for reporting
├── test_querykings.csv                 # Final scored output
├── report.pdf                          # Detailed methodology & findings
├── presentation.pptx                   # Hackathon presentation deck
├── requirements.txt                    # Python dependencies
└── README.md                           # You are here
```

---

## 🚀 Quick Start

### Prerequisites
- Google Account (for Colab access)
- Dataset files (contact team for access)

### Setup & Execution

1. **Open in Google Colab**
   - Navigate to [Google Colab](https://colab.research.google.com/)
   - Upload the notebooks from `/notebooks/` folder

2. **Upload Data**
   ```python
   # In Colab, run this in the first cell:
   from google.colab import files
   uploaded = files.upload()  # Upload all 5 CSV files
   ```

3. **Run Notebooks Sequentially**

   | Notebook | Purpose | Output |
   |----------|---------|--------|
   | `1_Understanding_Data` | Data quality checks, schema validation | Data profiling report |
   | `2_Deliverable_1_EDA` | Exploratory visualizations, correlation analysis | EDA insights, risk factors |
   | `3_Deliverable_2_Scoring` | Model training, difficulty score calculation | `test_querykings.csv` |
   | `4_Deliverable_3_Insights` | What-if analysis, economic modeling | Business recommendations |


## 📊 Methodology

### Data Sources
- **Flight Operations**: Scheduled vs. actual times, delays, cancellations
- **Passenger Records**: Connection times, special services, booking patterns
- **Baggage Data**: Transfer complexity, mishandling risk
- **Airport Metadata**: Gate constraints, weather conditions

### Difficulty Score Components
1. **Connection Complexity** (30%): Tight connections, international transfers
2. **Baggage Risk** (25%): Transfer volumes, historical mishandling
3. **Schedule Pressure** (20%): Turn times, slot constraints
4. **Passenger Services** (15%): Special assistance, group bookings
5. **External Factors** (10%): Weather, ATC delays

### Machine Learning Pipeline
```
Data Ingestion → Feature Engineering → Model Training → Score Generation → Validation
     ↓                  ↓                    ↓                ↓              ↓
  DuckDB SQL      Aggregations      Random Forest      0-100 Scale    Business Rules
```

---

## 📈 Key Outputs

### `test_querykings.csv` Schema
```csv
flight_id, difficulty_score, difficulty_rank, risk_classification, top_risk_factors
UA1234, 87.3, High, Critical, "tight_connections|baggage_volume|weather"
```

### Visualization Examples
- Difficulty distribution by time of day
- Risk factor correlation heatmaps
- Economic impact projections
- Gate utilization optimization

---

## 🛠️ Tech Stack

| Category | Technologies |
|----------|-------------|
| **Data Processing** | pandas, numpy, DuckDB (SQL) |
| **Machine Learning** | scikit-learn, XGBoost |
| **Visualization** | matplotlib, seaborn, plotly |
| **Environment** | Google Colab, Jupyter |
| **Version Control** | Git, GitHub |

---

## 📦 Installation

For local execution (optional):

```bash
# Clone repository
git clone https://github.com/yourusername/flight-difficulty-score.git
cd flight-difficulty-score

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
```

**requirements.txt:**
```
pandas>=1.5.0
numpy>=1.23.0
scikit-learn>=1.2.0
matplotlib>=3.6.0
seaborn>=0.12.0
duckdb>=0.8.0
plotly>=5.14.0
```

---

## 🏆 Team QueryKings

This project was developed during the United Airlines Hackathon as a solution to optimize flight operations through data-driven difficulty scoring.

**Contributors:**
- [Ekom and Rayan]

---


## 🤝 Acknowledgments

- United Airlines for providing the hackathon opportunity and datasets
- Google Colab for computational resources
- Open-source community for ML tools and libraries

---


<div align="center">

**Built with ❤️ by Team QueryKings**

[⬆ Back to Top](#-flight-difficulty-score-at-ord)

</div>
