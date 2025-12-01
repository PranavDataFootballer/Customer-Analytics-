# Retail Customer Behavior Analysis and Price Elasticity Modeling

## Project Overview
This project delivers a comprehensive, data-driven analysis of customer behavior in the retail sector. The goal was to transform raw demographic and transactional data into **actionable business intelligence** by segmenting the customer base and modeling their sensitivity to price changes (elasticity).

The final output is a differentiated pricing strategy tailored to unique customer segments, aiming to optimize promotional spending and maximize revenue.

## Business Goal
To move away from a "one-size-fits-all" pricing and promotion strategy by answering three key questions:
1.  **Who** are our distinct customer groups (segmentation)?
2.  **What** are the buying patterns and brand preferences of these groups?
3.  **How** sensitive is each group to price changes (Price Elasticity of Demand)?

## Methodology & Analytical Pipeline

The project followed a three-phase data science workflow:

### Phase 1: Customer Segmentation (Notebook: `Customer Analytics.ipynb`)
1.  **Data Preparation:** Standardized demographic features (`Age`, `Income`, `Education`, etc.).
2.  **Dimensionality Reduction:** Applied **Principal Component Analysis (PCA)** to reduce feature space and capture the most variance in a lower dimension.
3.  **Clustering:** Implemented **K-Means Clustering** to partition the customer base into 4 optimal, distinct behavioral segments (e.g., *Urban Achievers*, *Rural Beginners*).

### Phase 2: Descriptive Purchase Analysis (Notebook: `Purchase Analytics Descriptive Analysis.ipynb`)
1.  Merged segment tags onto the transaction data.
2.  Analyzed purchase metrics, including brand preference, purchase frequency, and response to promotions, **by segment**.

### Phase 3: Purchase Probability Modeling (Notebook: `Modeling Purchase Incidence.ipynb`)
1.  **Model Selection:** Used **Logistic Regression** to model `Purchase Incidence` (the probability of a customer making a purchase during a store visit).
2.  **Elasticity Calculation:** Calculated the **Price Elasticity of Purchase Probability** for the overall market and, critically, for *each individual customer segment*.

## Key Findings & Business Impact

| Segment Example | Elasticity | Strategic Implication |
| :--- | :--- | :--- |
| **Rural Beginners** | **Highly Elastic** | **Volume Focus:** Most price sensitive. Use frequent, aggressive promotions (discounts on Brands 1 & 2) to capture transaction volume. |
| **Urban Achievers** | **Inelastic** | **Margin Focus:** Least price sensitive. Maintain premium pricing and focus marketing on convenience and product exclusivity (Brands 4 & 5). |
| **Overall Impact** | | The project validated that **blanket promotions were inefficient**, allowing the business to redirect marketing spend and secure higher margins from inelastic segments. |

## Technologies & Libraries
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-learn (StandardScaler, PCA, KMeans, LogisticRegression)
* **Statistical Analysis:** Scipy
* **Visualization:** Matplotlib, Seaborn

## Repository Structure
