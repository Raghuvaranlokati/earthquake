# 🏔️ Richter's Predictor: Nepal Earthquake Building Damage Prediction | DrivenData

![DrivenData Competition](https://img.shields.io/badge/DrivenData-Richter's_Predictor-blue?style=for-the-badge)
![Rank](https://img.shields.io/badge/Leaderboard_Rank-%23481-brightgreen?style=for-the-badge)
![Score](https://img.shields.io/badge/Micro--Averaged_F1_Score-0.7489-orange?style=for-the-badge)
![Model](https://img.shields.io/badge/Model-HistGradientBoosting-yellow?style=for-the-badge)

Welcome to the ultimate repository for the **[Richter's Predictor: Modeling Earthquake Damage](https://www.drivendata.org/competitions/57/nepal-earthquake/)** competition hosted by **DrivenData**. This repository provides an end-to-end Machine Learning pipeline to predict building damage caused by the 2015 Gorkha earthquake in Nepal using the official **Nepal Earthquake Dataset**.

## 🏆 Competition Results & Leaderboard
To track competition progress, submissions are scored against public test data.
- **Evaluation Metric:** Micro-averaged F1 Score
- **My Best Public Score:** **0.7489**
- **Current Leaderboard Rank:** **#481**

## 📌 Problem Statement
The goal of this competition is to predict the level of damage to buildings caused by the 2015 Gorkha earthquake in Nepal based on aspects of building location and construction. The target variable is `damage_grade`, which represents the severity of the damage on a scale from 1 to 3:
- **1:** Low damage
- **2:** Medium damage
- **3:** High damage (Complete destruction)

## 📊 About the Nepal Earthquake Dataset
If you are searching for the **Nepal Earthquake Dataset** or solutions to the DrivenData competition, this repository contains exactly what you need. The dataset features comprehensive building survey data collected by the Central Bureau of Statistics under the National Planning Commission Secretariat of Nepal.

- **Features:** 39 categorical and numerical columns, including geographic identifiers, building construction materials (foundation, roof, floor types), building characteristics (age, height, area), and secondary uses.
- **Dataset Size:** Over 260k training samples.

## 🚀 Machine Learning Pipeline & Methodology
The entire workflow is open-sourced in the `nepal_earthquake_model.ipynb` notebook. It demonstrates a highly accurate and scalable approach to building damage prediction.

### Key Highlights:
1. **Automated Data Retrieval:** The dataset (`train_values.csv`, `train_labels.csv`, `test_values.csv`) is automatically downloaded via Google Drive APIs inside the notebook.
2. **Data Preprocessing:** Categorical features are efficiently encoded using Scikit-Learn's `OrdinalEncoder`.
3. **Advanced Modeling:** The core algorithm used is the **`HistGradientBoostingClassifier`**, which handles categorical features naturally and scales beautifully for large datasets.
4. **Validation Strategy:** Robust model evaluation using **Stratified K-Fold Cross-Validation** to ensure generalizability.
5. **Feature Analysis:** Utilized `permutation_importance` to identify the most critical geographic and structural features predicting earthquake damage.

## 📂 Repository Structure
```text
📦 earthquake
 ┣ 📜 nepal_earthquake_model.ipynb  # End-to-End ML Pipeline (Main Code)
 ┣ 📜 train_values.csv              # Nepal Earthquake Dataset - Training features
 ┣ 📜 train_labels.csv              # Nepal Earthquake Dataset - Training labels
 ┣ 📜 test_values.csv               # Nepal Earthquake Dataset - Test features
 ┣ 📜 submission.csv                # Final DrivenData submission file
 ┗ 📜 README.md                     # You are here!
```

## ⚙️ How to Run the Code
You don't need to manually download the dataset! The notebook handles everything.
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Raghuvaranlokati/earthquake.git
   cd earthquake
   ```
2. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook nepal_earthquake_model.ipynb
   ```
3. **Run All Cells:** Sit back as the notebook downloads the data, trains the `HistGradientBoostingClassifier`, evaluates the F1 score, and generates the final `submission.csv`.

## 👤 Author
- **Raghuvaran Lokati**
- **DrivenData Profile:** [raghuvaran_lokati](https://www.drivendata.org/users/raghuvaran_lokati/)

## 🔍 Tags & SEO Keywords
`Nepal Earthquake Dataset`, `DrivenData Richter's Predictor`, `Modeling Earthquake Damage`, `DrivenData Competition Solution`, `Machine Learning`, `Data Science`, `HistGradientBoostingClassifier`, `Micro-averaged F1 Score`, `Building Damage Prediction`, `Scikit-Learn`, `Python`

---
⭐ *If this repository helped you understand the dataset or improve your score on DrivenData, please consider giving it a star!*
