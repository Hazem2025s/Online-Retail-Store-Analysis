# Online-Retail-Store-Analysis
Online Retail: Full Data Analysis

# Online Retail: Full Data Analysis

An end-to-end analysis of **541,909 transactions** from a UK-based online gift retailer (Dec 2010 – Dec 2011): data quality checks, cleaning, business analysis and visualization, all in one notebook.

## What's inside
- **Data cleaning:** removed 5,268 duplicate rows, handled missing descriptions and the ~25% of rows with no customer ID, and separated cancellations from real sales.
- **Business analysis:** top products, country performance, customer ranking, cancellations and monthly revenue.
- **Visualization:** Matplotlib, Seaborn and interactive Plotly charts, each with a written insight.

## Key findings
- **Fake "bestsellers":** two of the largest orders (80,995 and 74,215 units) were cancelled by the same customers within 20 minutes, and "DOTCOM POSTAGE" topped the revenue ranking even though it isn't a product. After cleaning, the top product is the **Regency Cakestand 3 Tier (~£174K)**.
- **UK dominates, but exports order more:** the UK is about **85%** of revenue, while international invoices are about **70% larger** (£813 vs £474).
- **Q4 drives the year:** November revenue (~£1.45M) is about **2.9x** February's, and September–November produce about **40%** of January–November revenue.

## Tools
Python · Pandas · NumPy · Matplotlib · Seaborn · Plotly · Jupyter Notebook

## Files
| File | Description |
|---|---|
| `Online_Retail_Full_Data_Analysis.ipynb` | Full analysis notebook |
| `OnlineRetail.csv` | Raw dataset |

## How to run
1. Clone the repo and keep the notebook and CSV in the same folder.
2. Install the libraries: `pip install pandas numpy matplotlib seaborn plotly jupyter`
3. Open the notebook and choose **Run All**.

## Author
[Hazem Aboelabas] · [LinkedIn][((https://www.linkedin.com/in/hazem-aboelabas-3323aa29a/))](https://www.linkedin.com/in/hazem-aboelabas-3323aa29a/)


markdown
# Online Retail: Full Data Analysis

An end-to-end analysis of **541,909 transactions** from a UK-based online gift retailer, covering December 2010 to December 2011. The project takes a messy raw export through data-quality checks, cleaning, business analysis and visualization, all in a single Jupyter notebook.

## Why this project
Retail data is rarely clean. This dataset contains duplicates, missing customer IDs, cancellations, postage and fee codes mixed in with real products, and orders that were reversed minutes after being placed. The goal was to clean it carefully and then answer real business questions: What sells best? Where does revenue come from? When is demand highest?

## Dataset
Transactions include invoice number, stock code, description, quantity, invoice date, unit price, customer ID and country, across 38 countries.

## What I did
- **Data quality:** found and removed 5,268 duplicate rows, handled 1,454 missing descriptions, and flagged the roughly 25% of rows with no customer ID as "Guest" so revenue is kept without distorting customer rankings.
- **Cleaning decisions:** separated cancellations from real sales, excluded non-product codes (postage, manual adjustments, fees), and removed two huge orders that were fully cancelled shortly afterwards.
- **Analysis:** top products, country performance, customer ranking and monthly revenue trends.
- **Visualization:** Matplotlib, Seaborn and interactive Plotly charts, each with a written insight.

## Key findings
1. **Fake bestsellers:** two of the largest orders (80,995 and 74,215 units) were cancelled by the same customers within 20 minutes. After cleaning, the top product is the Regency Cakestand 3 Tier, with about £174K in revenue.
2. **UK dominates, exports order more:** the UK generates about 85% of revenue, yet international invoices are about 70% larger (£813 vs £474).
3. **Q4 drives the year:** November revenue (about £1.45M) is roughly 2.9x February's, and September to November produce about 40% of January to November revenue.

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly, Jupyter Notebook.

## How to run
1. Clone the repository and keep the notebook and `OnlineRetail.csv` in the same folder.
2. Install the libraries: `pip install pandas numpy matplotlib seaborn plotly jupyter`
3. Open the notebook and select **Run All**.
