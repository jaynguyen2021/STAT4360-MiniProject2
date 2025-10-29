# STAT4360 Mini Project 2 – Regression, LDA, and QDA Analysis

**Author:** Van Nguyen  
**Course:** STAT 4360 – Introduction to Statistical Learning (Fall 2025)  
**University:** The University of Texas at Dallas  
**Instructor:** Dr. Wang  

---

## Overview

This project explores two datasets using regression and classification techniques to understand prediction accuracy, model selection, and bias–variance tradeoff.

1. **Wine Quality Analysis**  
   - Built multiple linear regression models to predict wine *Quality* using features such as *Clarity, Aroma, Body, Flavor, Oakiness,* and *Region*.  
   - Selected the reduced model:
     \[
     \hat{Quality} = 7.0943 + 1.1155 \times Flavor - 1.5335 \times Region_2 + 1.2234 \times Region_3
     \]
   - \( R^2 = 0.82 \), showing strong positive correlation between *Flavor* and *Quality*.  
   - Diagnostic plots confirmed normal residuals and stable variance.

2. **Diabetes Classification**  
   - Compared **Linear Discriminant Analysis (LDA)** and **Quadratic Discriminant Analysis (QDA)**.  
   - Results summary:

     | Model | Misclassification | Sensitivity | Specificity | AUC |
     |--------|------------------|--------------|--------------|-----|
     | LDA | 22.0% | 56.4% | 89.2% | 0.837 |
     | QDA | 23.6% | 57.6% | 86.2% | 0.835 |

   - Chosen model: **LDA** (simpler and slightly higher accuracy).

3. **Bonus – James–Stein Estimator Simulation**  
   - Compared **James–Stein** vs **MLE** estimators for multivariate normal means.  
   - Findings: James–Stein has lower risk (MSE) due to bias–variance tradeoff when \( p \ge 3 \).

---

## Skills Demonstrated
- Multiple Linear Regression  
- LDA and QDA Classification  
- Model Selection & Diagnostics  
- ROC Curve and AUC Evaluation  
- Bias–Variance and Shrinkage Estimation  
- R Markdown + LaTeX Reporting  
- Data Visualization and Simulation  

---

## Technologies Used
- **Language:** R  
- **Libraries:** `MASS`, `pROC`, `car`, `corrplot`  
- **Tools:** RStudio, Git, GitHub, LaTeX  

---

## 📁 Repository Contents
| File | Description |
|------|--------------|
| `mini_project_2_report.Rmd` | R Markdown source code |
| `mini_project_2_report.pdf` | Final report with outputs |
| `Mini_Project_2_Latex.pdf` | LaTeX formatted version |
| `wine.txt` | Wine dataset |
| `diabetes.csv` | Diabetes dataset |
| `mini_project_2 Q.pdf` | Original project instructions |

---

## 🔗 Links
-  [Course: STAT 4360 – Introduction to Statistical Learning](https://catalog.utdallas.edu/2025/undergraduate/courses/stat4360)
-  [GitHub Repository](https://github.com/jaynguyen2021/STAT4360-MiniProject2)
-  [LinkedIn – Van Nguyen](https://www.linkedin.com/in/jaynguyen2021)

---

##  Acknowledgment
Special thanks to **Dr. Wang** for insightful lectures and guidance on statistical learning and model evaluation.
