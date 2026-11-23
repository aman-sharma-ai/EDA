# Exploratory Data Analysis

This repository contains two exploratory analyses of real-world retail and restaurant data. Each covers data cleaning, visual exploration and feature engineering in Python.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat-square)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

---

## Notebooks

| Notebook | Dataset | Scope |
|---|---|---|
| [`Black friday eda and feature engineering.ipynb`](Black%20friday%20eda%20and%20feature%20engineering.ipynb) | Black Friday retail transactions (`train.csv`, `test.csv`) | Combination of the training and test sets; encoding of gender, age, city category and years in the current city; imputation of missing product categories; visual analysis; and feature scaling with a train/test split in preparation for purchase-amount prediction. |
| [`ZomatoEDA .ipynb`](ZomatoEDA%20.ipynb) | Zomato restaurants (`zomato.csv`), joined with `Country-Code.xlsx` | Assessment of missing values, numerical and categorical features, rating distribution, geographic coverage and online-delivery availability. |

## Key Findings

### Zomato
- The majority of restaurant records originate from **India**, followed by the **United States** and the **United Kingdom**.
- **"Not rated"** is the largest rating category; most rated restaurants score between **2.9 and 3.9**.
- Most zero ratings are given by customers in India.
- **Online delivery** is offered only in **India and the United Arab Emirates**.

### Black Friday
- The dataset contains **550,068 transactions** from **5,891 customers** across **3,631 products**.
- **Male customers account for 77% of total spending** and also have a higher average purchase value (9,438 compared with 8,735).
- The **26–35 age group generates 40% of revenue**, while customers aged **51–55 record the highest average purchase value**.
- **City category B contributes the largest share of revenue (42%)**, whereas **City category C** has the largest customer base and the highest average purchase value.
- Marital status has a negligible effect on purchase value.
- `Product_Category_3` is missing in **70%** of records and `Product_Category_2` in **32%**, which makes imputation a key feature-engineering step.

## Running Locally

```bash
git clone https://github.com/aman-sharma-ai/EDA.git
cd EDA
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl jupyter
jupyter notebook
```

> **Note:** The Black Friday CSV files (approximately 34 MB) are included so that the notebook runs without additional downloads.
