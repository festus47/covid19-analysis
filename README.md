# COVID-19 Global Analysis 🦠

An end-to-end data science project analyzing global COVID-19 case data — from exploratory data analysis (EDA) through machine learning modeling.

## 📊 Project Overview

This project explores the spread, mortality, and recovery patterns of COVID-19 across the globe using daily and country-level case data. It demonstrates a complete data science workflow:

1. **Data Loading & Cleaning** — handling multiple datasets, fixing data types, treating missing values
2. **Exploratory Data Analysis** — global trends, country comparisons, mortality/recovery rates, regional breakdowns, correlation analysis
3. **Feature Engineering** — per-capita metrics, ratios, and severity tiers
4. **Machine Learning**
   - **Regression:** predicting total deaths from country metrics (Linear Regression vs. Random Forest)
   - **Classification:** categorizing countries into Low/Medium/High severity tiers
5. **Conclusions** — key findings, limitations, and next steps

## 📁 Repository Structure

```
covid19-analysis/
├── data/                       # Raw CSV datasets
├── notebooks/
│   └── covid19_eda_and_ml.ipynb
├── visuals/                    # Generated charts and plots
├── environment.yml             # Conda environment (primary)
├── requirements.txt            # pip alternative
├── .gitignore
└── README.md
```

## 🗂️ Dataset

The dataset contains daily counts of confirmed, death, and recovered cases across the globe.

| File | Description |
|------|-------------|
| `full_grouped.csv` | Daily country-wise cases (with province/state) |
| `covid_19_clean_complete.csv` | Daily country-wise cases |
| `country_wise_latest.csv` | Latest country-level snapshot |
| `day_wise.csv` | Global daily aggregates |
| `usa_county_wise.csv` | Daily county-level cases (USA) |
| `worldometer_data.csv` | Latest country stats (population, tests, etc.) |

## 🛠️ Tech Stack

- **Python 3**
- **pandas / numpy** — data manipulation
- **matplotlib / seaborn / plotly** — visualization
- **scikit-learn** — machine learning

## 🚀 Getting Started

This project uses **Conda** for environment management and runs in **VS Code's built-in notebook editor**.

```bash
# Clone the repository
git clone https://github.com/festus47/covid19-analysis.git
cd covid19-analysis

# Recreate the Conda environment
conda env create -f environment.yml
conda activate covid19
```

Then open `notebooks/covid19_eda_and_ml.ipynb` in VS Code and select the `covid19` kernel (top-right corner → **Select Kernel** → **Python Environments** → `covid19`).

> **Note:** Make sure the Microsoft **Python** and **Jupyter** extensions are installed in VS Code. A `requirements.txt` is also included for users who prefer `pip`.

## 📈 Key Findings

- Global confirmed cases showed exponential growth in the early pandemic period
- Mortality and recovery rates varied significantly across countries
- Random Forest substantially outperformed Linear Regression in predicting deaths, pointing to non-linear relationships
- Total confirmed cases was the strongest predictor of total deaths

## 🔮 Next Steps

- Time-series forecasting (ARIMA, Prophet)
- Incorporate policy and vaccination data
- Build an interactive Streamlit/Plotly Dash dashboard

## 📝 License

This project is licensed under the MIT License.

---

*Part of my data science portfolio. Feedback and contributions welcome!*
