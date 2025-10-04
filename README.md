# skyhack_querykings
Title: Flight Difficulty Score — ORD (United Airlines Hackathon)
Objective: Predict a flight’s difficulty (probability 0–1) using operational features; rank daily; classify (D/M/E); deliver insights & actions.

Data (not included in repo):
Flight Level, PNR Flight Level, PNR Remark Level, Bag Level, Airports (ORD, 2 weeks).

How to Run (Colab):

Open notebooks/01_eda_ml_scoring.ipynb in Google Colab.

Place organizer CSVs in /data/ (Colab or Drive).

Run all cells top → bottom.

Outputs:

output/scores/test_<yourname>.csv

figures in output/figs/ (duplicates in additional/figs/ for slides)

What the Notebook Does:

Build flight-level features → EDA → label (delay>15 OR slack≤0) → ML (LogReg + RF/XGB) → score (probability) → daily ranks + tiers → export CSV.

Repo Structure: (folders as created)
License: MIT
