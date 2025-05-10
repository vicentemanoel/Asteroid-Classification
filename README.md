# 🚀 Asteroid Classification in the 4J-2S-1 Resonance Using Machine Learning

## 📚 Project Overview

This project develops an **automated machine learning classifier** to predict whether an asteroid is trapped in the **4J-2S-1 three-body mean-motion resonance** with **Jupiter and Saturn**.  
By using **proper orbital elements** (`a_p`, `e_p`, `sin(i_p)`) from the **AstDyS catalog**, the model replaces the need for intensive dynamical simulations.

### Data Sources:
- **AstDyS Catalog (`all.syn`)**: Proper elements for asteroids.
- **Resonant Asteroid List (`4J-2S-1_up_200000.csv`)**: Confirmed resonant asteroids.

### Machine Learning Models:
- k-Nearest Neighbors (kNN)
- Decision Tree
- Random Forest
- Gradient Boosting
- Logistic Regression (for baseline comparison)

### Evaluation Metrics:
- Accuracy
- Precision
- Recall
- F1-Score
- Cross-validation

---

## 📊 Main Results

- **Random Forest** and **Gradient Boosting** delivered the best performance.
- Best model results:
  - **Accuracy**: ~98%
  - **Precision**: ~96%
  - **Recall**: ~95%
  - **F1-Score**: ~95%
- Cross-validation showed consistent performance across different folds.

---

## 📌 Conclusions

- **Proper orbital elements** are powerful predictors for resonance membership.
- **Random Forest** emerged as the most effective classifier.
- This machine learning approach significantly **reduces computational costs** compared to full dynamical analysis.
- The trained model can assist researchers in **rapidly identifying candidate resonant asteroids**.

---

## 📂 Project Structure

```bash
├── Asteroid_Classification.ipynb    # Main analysis notebook
├── all.syn                           # AstDyS catalog data
├── 4J-2S-1_up_200000.csv             # Resonant asteroid list
└── README.md                         # Project description
