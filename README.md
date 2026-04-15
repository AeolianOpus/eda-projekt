# Automobile Price Analysis: Data Cleaning & EDA

A comprehensive exploratory data analysis and regression modeling project analyzing factors that influence car prices.

## 📊 Project Overview

This project performs data cleaning, exploratory data analysis (EDA), hypothesis testing, and linear regression modeling on the Kaggle Automobile Dataset to understand what drives car prices.

**Authors:** Nicklas Skoglund & Constantine Diamantis  
**Institution:** Jensen Yrkeshögskola  
**Date:** April 2026

## 🎯 Objectives

- Clean and prepare automobile data for analysis
- Identify key factors affecting car prices
- Perform statistical hypothesis testing
- Build and validate a predictive linear regression model
- Communicate findings through data storytelling

## 📁 Project Structure

    eda-projekt/
    ├── data/
    │   ├── Automobile_data.csv          # Original dataset
    │   └── Automobile_data_clean.csv    # Cleaned dataset
    ├── analys/
    │   └── analysis.ipynb               # Main analysis notebook
    ├── output/
    │   ├── 01_price_distribution.png
    │   ├── 02_correlation.png
    │   ├── 03_scatter_plots.png
    │   ├── 04_categorical_analysis.png
    │   ├── 05_regression.png
    │   ├── 06_residual_analysis.png
    │   └── 07_outliers.png
    ├── requirements.txt
    ├── .gitignore
    └── README.md

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- pip

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/automobile-eda-project.git
cd automobile-eda-project
```

2. Create virtual environment:
```bash
python -m venv venv
```

3. Activate virtual environment:

**Windows (PowerShell):**
```powershell
.\venv\Scripts\Activate
```

**macOS/Linux:**
```bash
source venv/bin/activate
```

4. Install dependencies:
```bash
pip install -r requirements.txt
```

5. Run the analysis:
```bash
jupyter notebook analys/analysis.ipynb
```

## 📈 Key Findings

### Data Cleaning
- **Original:** 205 rows, 26 variables
- **Cleaned:** 201 rows, 0 missing values
- Handled missing values ('?'), corrected data types, imputed with median

### Exploratory Analysis
- **Strongest correlations with price:**
  - engine-size (r = 0.87)
  - curb-weight (r = 0.83)
  - horsepower (r = 0.82)
- **Price distribution:** Right-skewed (mean > median)
- **Body-style impact:** Convertible/Hardtop most expensive (~$22k)

### Statistical Testing
- **ANOVA:** Body-style significantly affects price (p < 0.001)
- **T-test:** Fuel-type does not significantly affect price (p = 0.12)

### Regression Model
- **R² = 0.76** (76.1% variance explained)
- **RMSE = $3,876** (average prediction error)
- **Equation:** Price = -7963 + 167 × engine-size
- **Interpretation:** Each unit increase in engine-size → +$167 in price

## 🛠️ Technologies Used

- **Python 3.14**
- **pandas** - Data manipulation
- **numpy** - Numerical computing
- **matplotlib** - Visualization
- **seaborn** - Statistical visualization
- **scipy** - Statistical testing
- **statsmodels** - Regression modeling
- **scikit-learn** - Model evaluation

## 📊 Dataset

**Source:** Kaggle Automobile Dataset

**Variables:**
- Numerical: price, engine-size, horsepower, curb-weight, mpg, dimensions
- Categorical: make, body-style, fuel-type, drive-wheels, num-of-cylinders

## 📝 License

This project is for educational purposes at Jensen Yrkeshögskola.

## 👥 Contributors

- **Nicklas Skoglund**
- **Constantine Diamantis**

## 🙏 Acknowledgments

- Jensen Yrkeshögskola for the course framework
- Kaggle for the dataset
