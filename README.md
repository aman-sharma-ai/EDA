# 🔍 Exploratory Data Analysis

Two exploratory analyses on real-world retail and restaurant data, covering data cleaning, visual exploration and feature engineering in Python.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat-square)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

---

## 📂 Notebooks

| Notebook | Dataset | What it covers |
|---|---|---|
| [`Black friday eda and feature engineering.ipynb`](Black%20friday%20eda%20and%20feature%20engineering.ipynb) | Black Friday retail transactions (`train.csv`, `test.csv`) | Combining train and test, encoding gender, age, city category and years in city, filling missing product categories, visual analysis, then scaling and a train/test split ready for purchase-amount prediction |
| [`ZomatoEDA .ipynb`](ZomatoEDA%20.ipynb) | Zomato restaurants (`zomato.csv`) joined with `Country-Code.xlsx` | Missing values, numerical and categorical features, rating distribution, which countries dominate the data, and where online delivery is available |

## 💡 Key findings

### Zomato
- Most restaurant records come from **India**, followed by the **USA** and the **UK**.
- **"Not rated"** is the largest rating group; most rated restaurants score between **2.9 and 3.9**.
- Most zero ratings come from Indian customers.
- **Online delivery** is only offered in **India and the UAE**.

### Black Friday
- **550,068 transactions** from **5,891 customers** across **3,631 products**.
- **Men account for 77% of total spend** and also spend more per purchase on average (9,438 vs 8,735).
- The **26–35 age group drives 40% of revenue**, while customers aged **51–55 have the highest average purchase**.
- **City B brings in the most revenue (42%)**, but **City C** has the most customers and the highest average purchase.
- Marital status makes almost no difference to purchase value.
- `Product_Category_3` is missing in **70%** of rows and `Product_Category_2` in **32%**, so imputation is a key feature-engineering step.

## ▶️ Run it locally

```bash
git clone https://github.com/AmanDataverse/EDA.git
cd EDA
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl jupyter
jupyter notebook
```

> **Note:** the Black Friday CSVs (about 34 MB) are included so the notebook runs as-is.
