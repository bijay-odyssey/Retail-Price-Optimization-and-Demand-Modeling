# Retail Price Optimization with Competition & Lag Effects  
### Demand Modeling • Price Elasticity • Competitor-Aware Pricing • Profit Maximization

This project applies **data-driven pricing techniques** to retail sales data, integrating  
**competition, lag effects, and product attributes** into a full pricing intelligence workflow.

It is designed to replicate a realistic retail pricing environment using ML-based demand modeling and classical microeconomics concepts such as elasticity and marginal revenue.

---

## Table of Contents
1. [Project Overview](#project-overview)  
2. [Dataset](#dataset)  
3. [Key Features Engineered](#key-features-engineered)  
4. [Analysis Workflow](#analysis-workflow)  
5. [Modeling Approach](#modeling-approach)  
6. [Price Elasticity Estimation](#price-elasticity-estimation)  
7. [Competition-Adjusted Pricing](#competition-adjusted-pricing)  
8. [Profit Optimization](#profit-optimization)  
9. [Technologies Used](#technologies-used)  
10. [Results & Business Recommendations](#results--business-recommendations)  

---

##  Project Overview
Many retailers make pricing decisions using intuition or simple rules like fixed margins.  
This notebook demonstrates how **machine learning + economics** can produce  
*quantitatively defensible pricing strategies*.

We model demand using:
- Unit price  
- Competitor prices (3 competitors)  
- Lagged price effects  
- Product metadata  
- Time-based seasonality  
- Customer count and behavior signals  

From this model, we derive:
- Price elasticity of demand  
- Competition-adjusted sensitivity  
- Simulated price scenarios  
- Profit curves and optimal prices  

---

##  Dataset
The dataset includes product-level monthly retail sales with attributes:

- `unit_price`, `total_price`, `freight_price`  
- `qty` (target variable)
- Competitor prices: `comp_1`, `comp_2`, `comp_3`
- Lag features like `lag_price`
- Customer indicators
- Product metadata & seasonality signals

---

## Key Features Engineered
- `price_gap` vs average competition  
- Relative competitor price ratios  
- Price momentum via `lag_price`  
- Discount / margin measures  
- Time-based seasonality variables  

These adjustments allow realistic modeling of market-driven pricing.

---

## Analysis Workflow
1. **Load & Inspect Data**  
2. **Data Cleaning**  
3. **Feature Engineering (pricing, competition, lag effects)**  
4. **Exploratory Analysis**  
5. **Demand Modeling (regression)**  
6. **Elasticity Estimation**  
7. **Competition-Aware Pricing Simulations**  
8. **Profit Optimization**  
9. **Final Recommendations**

---

## Modeling Approach
A regression-based demand model predicts `qty` as a function of price and competition.

Experiments include:
- Linear Regression  
- Ridge  
- Random Forest Regressor  
- Gradient Boosting  

Performance is validated via:
- R²  
- RMSE  
- Visual error analysis  

---

## Price Elasticity Estimation

This helps classify product sensitivity:
- **Elastic** → price changes cause large quantity shifts  
- **Inelastic** → quantity stable regardless of price  

---

## Competition-Adjusted Pricing
By comparing product price to 3 competitors, we evaluate:
- Price positioning  
- Undercut/overcut strategies  
- Optimal competitive margins  

---

## Profit Optimization
We generate price-simulation curves:

- Predicted quantity for candidate prices  
- Associated revenue and profit  
- Identification of optimal price maximizing:

---

## Technologies Used
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Seaborn / Matplotlib  
- Statsmodels  

---

## Results & Business Recommendations
The notebook concludes with:
- Optimal price per product  
- Elasticity-informed strategy  
- Competitive pricing adjustments  
- Margin-aware recommendations  

---
