# TikTok Analysis: EDA & Visualization

---

## Overview

This analysis focuses on exploring a provided dataset to better understand the variables, with a specific focus on identifying what separates claim videos from opinion videos. The goal is to continue the initial analysis and dig deeper using exploratory data analysis (EDA) techniques.

The data is:

* Loaded and reviewed to better understand its structure, variables, and overall data quality
* Cleaned and prepared by checking for inconsistencies, missing values, and outliers
* Visualized to examine engagement patterns and compare claim versus opinion content
* Results are interpreted to identify key differences and highlight features relevant for predictive modeling

---

## Key Insights

* Claim videos account for a much larger share of total views despite similar counts to opinion videos, showing that they reach a wider audience.
* Higher engagement, especially view count, is consistently tied to claim content, making it a strong signal for distinguishing claim versus opinion videos.
* Authors who post claim videos are more likely to be under review or banned, suggesting a clear link between claim content and moderation outcomes.
* Verified users are more likely to post opinion videos, indicating that account status may influence the type of content being shared.
* Engagement data is heavily skewed by a small number of high-performing videos, meaning outliers will need to be handled carefully in any predictive model.

---

## Visualization

* Python (matplotlib, seaborn) used for exploratory analysis
* Tableau dashboard used to present key patterns in a more interactive format

Link to Tableau Dashboard: https://public.tableau.com/app/profile/alfred.rico/viz/TiktokAnalysisEDAVisualization/Dashboard1#1

## Reproducibility

This project uses **UV** for fast, deterministic environment management.

### 🔧 Prerequisites

Install UV (official guide):  
https://docs.astral.sh/uv/getting-started/

---

### ▶️ Run Locally (Step-by-Step)

```bash
# 1. Clone the repository
git clone https://github.com/AlfredRico/TikTok-Analysis-EDA-Visualization.git
cd TikTok-Analysis-EDA-Visualization

# 2. Sync environment (installs Python + dependencies)
uv sync

# 3. Launch Jupyter Lab
uv run jupyter lab
```

---

### 📂 Open the Project

Once Jupyter Lab opens in your browser:

1. Navigate to the project root directory  
2. Open the notebook:

   ```
   tiktok_analysis_eda_visualization.ipynb
   ```

3. Run all cells from top to bottom  

---

### 🧠 Notes

- The environment is fully defined by:
  - `pyproject.toml`
  - `uv.lock`
- No manual package installation is required  
- Results are fully reproducible across systems  

---

## Project Structure

```
tiktok_analysis_eda_visualization/
├── data/tiktok_dataset.csv   # sample dataset (tracked)
├── tiktok_analysis_eda_visualization.ipynb
├── pyproject.toml
├── uv.lock
└── README.md
```

---

## Data Source

* Simulated TikTok dataset used to explore engagement patterns and content classification
* The dataset(3mb) is included in the github repo for reproducibility and can be cloned

---

## Ecosystem

* Portfolio webpage → Project hub and navigation: https://alfredrico.github.io/  
* GitHub → Project repositories featuring UV management for reproducibility: https://github.com/AlfredRico  