# 🌍 World Happiness Report - Data Pipeline & Analysis (2015-2019)

This project focuses on a complete **Data Engineering and Analysis** journey using the World Happiness Report datasets from 2015 to 2019. It covers everything from a robust ETL pipeline to deep exploratory insights regarding global well-being. 🚀

---

## 📌 Project Overview

The main objective is to understand what drives happiness across different nations and how these metrics (GDP, Health, Freedom, Trust) evolved over a 5-year period.

The project is divided into two main stages:
1.  **ETL Pipeline (`etl.ipynb`):** Consolidating scattered raw data into a standardized "Golden Table".
2.  **Exploratory Data Analysis (`analysis.ipynb`):** Visualizing trends, correlations, and regional performance.

---

## 🛠️ Tech Stack

* **Language:** Python 🐍
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / VS Code

---

## 🔄 ETL Process (Extract, Transform, Load)

The data was initially spread across five different CSV files with inconsistent column names. The pipeline handles:

* **Extraction:** Loading multiple CSVs and injecting temporal markers (`Year`). 📥
* **Transformation:** 🧪
    * Standardizing column names (e.g., `Happiness Rank` -> `Rank`).
    * Handling missing values (e.g., pre-processing Corruption data in 2018).
    * Feature selection (keeping essential metrics).
* **Loading:** Concatenating all records into a single `happiness_complete.csv` for optimized analysis. 💾

---

## 📊 Key Analysis Insights

* **Wealth vs. Happiness:** A strong positive correlation (0.79) between GDP and Happiness Score. 💰
* **Health & Longevity:** Health is the second strongest predictor (0.74). 🏥
* **The Trust Paradox:** Global trust in government saw a noticeable decline in the studied period. 📉
* **Brazil's Spotlight:** An in-depth look at Brazil's happiness evolution and how it compares to global averages. 🇧🇷

---

## 📂 Project Structure

```text
.
├── data/
│   ├── raw/                # Original yearly CSV files
│   └── processed/          # The final "Golden Table" (happiness_complete.csv)
├── notebooks/
│   ├── world_happiness_etl.ipynb    # Data cleaning and pipeline
│   └── world_happiness_analysis.ipynb # Charts and insights
└── README.md               # You are here!
```

---

## 🚀 How to Run

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/world-happiness-analysis.git
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas matplotlib seaborn numpy
    ```
3.  **Run the notebooks:**
    Open `world_happiness_etl.ipynb` first to generate the processed data, then explore the `world_happiness_analysis.ipynb`.


Developed with 💻 and ☕ by Felipe César Martins