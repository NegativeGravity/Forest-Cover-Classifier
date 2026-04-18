# Forest Cover Type Prediction

## 📌 Overview
This project focuses on predicting forest cover types from strictly cartographic variables (as opposed to remotely sensed data). Using the **UCI Forest Cover Type dataset**, the goal is to classify 30x30 meter cells into seven different forest cover types based on features such as elevation, slope, soil type, and distance to hydrology.

The analysis involves rigorous data preprocessing, feature engineering, and a comparative study of classification algorithms, with a particular focus on **Linear Discriminant Analysis (LDA)** for multiclass separation.

## ✨ Key Features
* **Multi-Class Classification:** Identifying 7 distinct forest cover types (e.g., Spruce/Fir, Lodgepole Pine, Ponderosa Pine).
* **Dimensionality Reduction & Separation:** Implementation of **Linear Discriminant Analysis (LDA)** to maximize class separability.
* **Rigorous Evaluation:** Detailed performance analysis using:
    * **Macro F1-Score:** Used as the primary metric to handle potential class imbalances.
    * **Confusion Matrix Visualization:** To identify specific misclassifications between similar forest types.
* **Geospatial Insights:** Analyzing how variables like `Elevation`, `Wilderness_Area`, and `Soil_Type` influence ecological distribution.

## 📊 Dataset Highlights
The project utilizes 54 features, including:
* **Quantitative:** Elevation, Aspect, Slope, Horizontal/Vertical Distance to Hydrology, Distance to Roadways, etc.
* **Qualitative (Binary):** 4 Wilderness Areas and 40 Soil Type designations.
* **Target:** `Cover_Type` (Integers 1 to 7).

## 🛠 Tech Stack
* **Language:** Python
* **Data Science:** `Pandas`, `NumPy`
* **Machine Learning:** `Scikit-learn`
* **Visualization:** `Seaborn`, `Matplotlib`

## 🚀 Methodology
1.  **Exploratory Data Analysis (EDA):** Investigating feature distributions and ecological correlations.
2.  **Preprocessing:** Scaling features and handling categorical wilderness/soil variables.
3.  **Model Selection:** Comparative analysis of supervised learning models, highlighting the effectiveness of **LDA** in high-dimensional feature spaces.
4.  **Performance Tuning:** Optimization of decision thresholds and holdout validation strategies.

## 📈 Results
The model demonstrates high accuracy in distinguishing between ecologically distinct zones. The **LDA Confusion Matrix** included in the notebook provides a "Comparative View" of how the model manages the subtle boundaries between overlapping forest types.

## ⚙️ Installation
1. Clone this repository:
   ```bash
   git clone [https://github.com/NegativeGravity/Forest-Cover-Classifier.git](https://github.com/NegativeGravity/Forest-Cover-Classifier.git)
