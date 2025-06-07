# 📊 Creditworthiness Prediction using CART and Random Forest

This project explores the prediction of creditworthiness using machine learning, specifically Decision Tree (CART) and Random Forest algorithms. It handles class imbalance using ROSE and compares model performance with various configurations (balanced vs. unbalanced, pruned vs. unpruned).

## 🛠️ Tech Stack

- **Language**: R
- **Key Libraries**:
  - `rpart`, `rpart.plot` – CART modeling and visualization
  - `randomForest` – Random Forest modeling
  - `ROSE` – Class imbalance handling
  - `caret` – Evaluation metrics
  - `ggplot2`, `dplyr`, `tidyr` – Data manipulation and plotting

## 🗃️ Dataset Description

This project uses the **German Credit Dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data)).

- **Samples**: 1000 customers
- **Target Variable**: Creditworthiness (`Good` or `Bad`)
- **Features**: 20 predictor variables, including demographic and financial attributes

| Feature               | Description                                                |
|-----------------------|------------------------------------------------------------|
| Account Status        | Status of checking account (e.g., < 0 DM, ≥ 200 DM)        |
| Duration              | Duration of the credit in months                           |
| Credit History        | Past payment record                                        |
| Credit Purpose        | Purpose of the loan (e.g., car, furniture, education)      |
| Credit Amount         | Amount of credit in Deutsche Marks                         |
| Savings/Bonds         | Amount in savings or bonds                                 |
| Employment Duration   | Length of current employment                               |
| Installment Rate      | Installment rate in percentage of income                   |
| Personal Status/Sex   | Marital status and gender                                  |
| Other Debtors         | Presence of other guarantors or co-debtors                |
| Residence Since       | Years at current address                                   |
| Property              | Type of owned property                                     |
| Age                   | Age of the applicant                                       |
| Other Installment Plan| Other installment plans (bank, stores, none)               |
| Housing               | Housing status (own, rent, free)                           |
| Existing Credits      | Number of existing credits at this bank                    |
| Job                   | Applicant's job category                                   |
| Number of Dependents  | Number of people being financially supported               |
| Telephone             | Whether the customer has a phone                           |
| Foreign Worker        | Whether the applicant is a foreign worker                  |

The dataset is publicly available and widely used as a benchmark in credit scoring research. It contains no missing values and a class imbalance of 70% `Good` vs 30% `Bad` credit records.

## 🔍 Workflow Overview

1. **Exploratory Data Analysis & Cleaning**
2. **Class Balancing** using `ROSE`
3. **Modeling**:
   - CART (with and without pruning)
   - Random Forest (with and without balancing)
4. **Evaluation** using:
   - Accuracy, Recall, Specificity, F1-Score
   - Kappa
   - Balanced Accuracy

---

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
 
## 🚀 How to Run

1. Clone the repository
2. Open R or RStudio
3. Download the dataset
4. Execute the scripts in order from the `R/` directory

---

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

- [UCI German Credit Dataset](https://doi.org/10.24432/C5NC77)
- Breiman et al. (1984). *Classification and Regression Trees*
- Breiman (2001). *Random Forests*
- Menardi & Torelli (2014). *ROSE*
- Mingers (1989). *Pruning Decision Trees*

---
