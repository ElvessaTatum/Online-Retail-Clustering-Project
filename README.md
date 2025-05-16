# Customer Segmentation via Clustering

This project segments customers based on **return and spending behavior** using clustering algorithms. It helps identify patterns like high spenders, frequent returners, and low-engagement customers.

---

## Dataset

- Online Retail data from UCI
- Includes transactions with `CustomerID`, `InvoiceNo`, `Quantity`, `UnitPrice`, etc.
- Returns flagged using negative quantities or invoice codes

---

## Preprocessing

- Removed rows without `CustomerID`
- Engineered key features per customer:
  - `ReturnRate`
  - `TotalReturns`
  - `TotalQuantityReturned`
  - `TotalMoneyReturned`
  - `NetSpending`
- Standardized & normalized data

---

## Clustering Workflow

- **K-Means Clustering**
  - Optimal `k` found via Elbow Method (k=6)
  - Evaluated with Silhouette Score
- **Hierarchical Clustering**
  - Dendrogram analysis (9 clusters)
- PCA used for 2D visualization

---

## Insights

- Identified distinct customer profiles
- Visualized cluster differences with bar plots
- Some clusters return a lot but still spend significantly

---

## Tools Used

- Python, Pandas, Seaborn, Scikit-learn, Matplotlib

---
