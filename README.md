# python-data-foundations

A set of small, from-scratch Python exercises covering core statistics, NumPy array analysis, and Pandas data wrangling — culminating in a full clean → analyze → visualize workflow on the Titanic dataset.

## Overview

Each piece builds on the last: raw statistics implemented without libraries, then NumPy for numerical/array-based analysis, then Pandas for real tabular data, ending with a complete exploratory data analysis and visualization pass on a public dataset.

## Project Structure

```
python-data-foundations/
├── 01_stats_cli.py              # Mean/median/mode from scratch (no external libraries)
├── 02_numpy_outlier_detection.py  # Rolling-window + z-score outlier detection on sensor data
├── 03_pandas_basics.ipynb       # Core Pandas: loading, filtering, indexing, aggregation
├── 04_pandas_advanced.ipynb     # groupby, merging, missing-value handling (Titanic dataset)
├── 05_data_visualization.ipynb  # EDA visualizations: histograms, bar charts, correlation plots
└── data/
    ├── Titanic-Dataset.csv
    └── titanic_cleaned.csv      # Cleaned output from the advanced-Pandas notebook
```

## What Each Script Covers

| # | Topic | Highlights |
|---|-------|------------|
| 1 | Statistics CLI | Implements `mean`, `median`, and `mode` from first principles — no NumPy/statistics module — to reinforce the underlying algorithms |
| 2 | NumPy Outlier Detection | Rolling mean/std over a sliding window, plus z-score thresholding (\|z\| > 2) across multiple sensor features to flag anomalous readings |
| 3 | Pandas Basics | Loading, filtering, indexing, and aggregating tabular data |
| 4 | Advanced Pandas | `groupby`, merging, and missing-value handling on the Titanic dataset to prepare it for analysis |
| 5 | Data Visualization | Histograms, bar charts, and correlation plots to surface patterns and relationships in the cleaned data |

## Tech Stack

- Python (no libraries, for the stats CLI)
- NumPy
- Pandas
- Matplotlib / Seaborn
- Jupyter Notebook

## Getting Started

```bash
git clone https://github.com/<your-username>/python-data-foundations.git
cd python-data-foundations
pip install -r requirements.txt
python 01_stats_cli.py          # run the CLI directly
jupyter notebook                # open the notebooks (03–05)
```

## License

MIT