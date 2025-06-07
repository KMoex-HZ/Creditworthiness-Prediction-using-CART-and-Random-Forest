# 📊 Creditworthiness Prediction using CART and Random Forest

This project explores the prediction of creditworthiness using machine learning, specifically Decision Tree (CART) and Random Forest algorithms. It handles class imbalance using ROSE and compares model performance with various configurations (balanced vs. unbalanced, pruned vs. unpruned).

## 📁 Project Structure

- `data/` – contains dataset used for modeling.
- `notebooks/` – Jupyter notebook for EDA and modeling workflow.
- `src/` – modular Python scripts for preprocessing, modeling, and evaluation.
- `results/` – saved figures and result metrics.
- `requirements.txt` – list of dependencies.
- `README.md` – this file.

## 🧪 Models Implemented

- **CART (Classification and Regression Trees)**  
  + With and without pruning  
  + On balanced and unbalanced data

- **Random Forest**  
  + With and without class balancing using ROSE

## ⚖️ Handling Class Imbalance

ROSE (Random Over Sampling Examples) was used to balance the dataset and improve the detection of minority class (credit "Bad").

## 📈 Performance Highlights

- **Best Model**: Random Forest with ROSE balancing
- **Balanced Accuracy**: 67.67%
- **Recall (Bad credit)**: 68.57%
- **Top Predictors**: 
  - Account Status
  - Savings/Bonds
  - Credit Purpose
  - Credit History
  - Employment

## 📌 Conclusion

This study shows that Random Forest with class balancing via ROSE provides the best trade-off between performance and fairness. However, CART remains useful for interpretability. Further improvements may include feature engineering and use of more advanced models (e.g., Gradient Boosting, Neural Networks).

## 👨‍🔬 Authors

Project by:  
- Khairunnisa Maharani  
- Azzahra Putri Kamilah  
- Cindy Laura Manik  
- Adit Taufiqurrohman  
- Muhammad Dzikra  

Institute: Institut Teknologi Sumatera – Data Science

## 📚 References

See the `pdf` for a detailed list of academic references.
