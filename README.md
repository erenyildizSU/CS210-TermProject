# CS210-TermProject

# 📊 Cryptocurrency Interest vs Bitcoin Prices Prediction

This project explores the relationship between public interest in cryptocurrencies—measured via Google Trends data—and Bitcoin price changes. Using statistical analysis and machine learning models (K-Nearest Neighbors and Random Forest), the project aims to predict future Bitcoin price variations based on online search trends.

## 📁 Dataset Sources

- `True.csv` — Bitcoin price data  
- `Google_Crypto Currency Interest Dataset.csv` — Weekly search interest in cryptocurrencies from Google Trends  

## 🎯 Objective

To analyze how online public interest in cryptocurrencies (especially Bitcoin) correlates with actual market prices, and to build predictive models that offer insights for investors and financial analysts.

---

## 🧠 Machine Learning Models

### 1. K-Nearest Neighbors (kNN)

- **Model Type:** Non-parametric (Regression)
- **Preprocessing:** Missing value handling, Min-Max normalization
- **Best k:** 13
- **Performance:**
  - RMSE: `8.52`
  - MSE: `72.59`

#### kNN Workflow:
1. Load & preprocess data
2. Normalize features for distance-based calculation
3. Split into training (80%) and testing (20%)
4. Test various `k` values using cross-validation
5. Visualize prediction vs actual
6. Evaluate via RMSE and MSE

---

### 2. 🌲 Random Forest Regressor

- **Model Type:** Ensemble learning (Regression)
- **Preprocessing:** Similar to kNN
- **Best Params:**
  - `n_estimators = 100`
  - `max_depth = 5`
- **Performance:**
  - RMSE: `8.49`
  - MSE: `72.52`

#### Random Forest Workflow:
1. Bootstrap & feature-randomized decision trees
2. Hyperparameter tuning for `n_estimators` and `max_depth`
3. Evaluate performance through RMSE/MSE
4. Visualize prediction distribution

---

## 📈 Visualizations

- Scatter plots of predicted vs actual values  
- k-value optimization graph for kNN  
- Grid-heatmap for Random Forest hyperparameter tuning  

---

## 🏁 Conclusion

Both models can predict Bitcoin interest based on online trends, but:

| Model         | RMSE  | MSE   |
|---------------|-------|--------|
| kNN           | 8.52  | 72.59  |
| Random Forest | 8.49  | 72.52  |

**✅ Winner: Random Forest** — due to its better generalization, lower error rates, and robustness to overfitting.

---

## ✅ Key Takeaways

- **kNN** is simple and interpretable, ideal for small datasets  
- **Random Forest** performs better on complex patterns, scalable for large datasets  
- **Hyperparameter tuning** is essential for improving prediction accuracy

---

## 🧑‍💻 Author

**Hüseyin Eren YILDIZ**  
CS210 - Introduction to Data Science  
