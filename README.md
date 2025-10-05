Flight Difficulty Score at ORD

This repository contains all code, images, and outputs for the Flight Difficulty Score project developed during the United Airlines Hackathon. The workflow is organized into Google Colab notebooks, with supporting folders for visuals and final deliverables.

Repository Structure
├── data/                               # Local only (not uploaded)
│   ├── Flight Level Data.csv
│   ├── PNR Flight Level Data.csv
│   ├── PNR Remark Level Data.csv
│   ├── Bag Level Data.csv
│   └── Airports Data.csv
│
├── notebooks/                          # Main workflow (Google Colab)
│   ├── 1_Understanding_Data.ipynb
│   ├── 2_Deliverable_1_Exploratory_Data_Analysis_(EDA).ipynb
│   ├── 3_Deliverable_2_Flight_Difficulty_Score_Development.ipynb
│   └── 4_Deliverable_3_Post-Analysis_&_Operational_Insights.ipynb
│
├── images/                             # Labelled graphs & visuals for report
├── test_querykings.csv                 # Final submission file
├── report.pdf / presentation.pptx      # Final report
├── requirements.txt                    # Python dependencies
└── README.md                           

How to Run

Open notebooks in Google Colab.

Upload the five datasets into /content/.

Execute the notebooks as per requirement:

1_Understanding_Data.ipynb → data preview and checks

2_Deliverable_1_Exploratory_Data_Analysis_(EDA).ipynb → visual EDA and operational risks

3_Deliverable_2_Flight_Difficulty_Score_Development.ipynb → machine learning models, difficulty scoring, generates test_querykings.csv

4_Deliverable_3_Post-Analysis_&_Operational_Insights.ipynb → what-if scenarios and economic impact

Outputs

test_querykings.csv → per-flight difficulty scores, ranks, classifications

images → labelled visuals used in the report and slides

report → methodology, results, and business insights

Tech Stack

Python: pandas, numpy, scikit-learn, matplotlib, seaborn

SQL: DuckDB for database handling

Google Colab: execution environment

Built during the United Airlines Hackathon by Team QueryKings 
