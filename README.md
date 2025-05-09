# Predicting Breast Cancer Using Machine Learning

## Introduction
This notebook explores various Python-based machine learning techniques to build a predictive model capable of determining whether the cancer type is Malignant or Benign.

## Problem Definition
The goal of this predictive model is to classify breast cancer cases into **Malignan** or **Benign**.

## Best Model
After extensive evaluation and hyperparameter tuning, the **Random Forest Classifier** emerged as the best-performing model, achieving **94% accuracy** in classification.

## Required Libraries
We will utilize the following tools and libraries:
- `pandas` for data manipulation
- `sklearn` for machine learning models (`LogisticRegression`,`KNN`,`RandomForestClassifier`, `DecisionTreeClassifier`)
- `Seaborn` and `Matplotlib` for data visualization

## Approach
Our workflow follows these structured steps:
1. **Problem Definition**
2. **Exploratory Data Analysis (EDA)**
3. **Feature Engineering**
4. **Data Visualization**
5. **Model Evaluation**
6. **Feature Selection**

## Dataset
The dataset is sourced from the Kaggle Dataset Repository: [Breast Cancer Dataset](https://www.kaggle.com/datasets/yasserh/breast-cancer-dataset).

### Features Description
Below is a breakdown of features included in the dataset:

| Feature                  | Type        | Description                                      |
|--------------------------|------------|--------------------------------------------------|
| `id`                     | Unique ID  | Patient identifier                              |
| `diagnosis`              | Categorical | Cancer classification (`M` = Malignant, `B` = Benign) |
| `radius_mean`            | Continuous  | Mean of the tumor radius                        |
| `texture_mean`           | Continuous  | Mean texture of the tumor surface               |
| `perimeter_mean`         | Continuous  | Mean perimeter of the tumor                     |
| `area_mean`              | Continuous  | Mean area of the tumor                          |
| `smoothness_mean`        | Continuous  | Mean smoothness level                           |
| `compactness_mean`       | Continuous  | Mean compactness of tumor                       |
| `concavity_mean`         | Continuous  | Mean concavity of tumor structure               |
| `concave points_mean`    | Continuous  | Mean number of concave points                   |
| `symmetry_mean`          | Continuous  | Mean symmetry of the tumor                      |
| `fractal_dimension_mean` | Continuous  | Mean fractal dimension                          |
| `radius_se`              | Continuous  | Standard error of tumor radius                  |
| `texture_se`             | Continuous  | Standard error of texture                       |
| `perimeter_se`           | Continuous  | Standard error of perimeter                     |
| `area_se`                | Continuous  | Standard error of area                          |
| `smoothness_se`          | Continuous  | Standard error of smoothness                    |
| `compactness_se`         | Continuous  | Standard error of compactness                   |
| `concavity_se`           | Continuous  | Standard error of concavity                     |
| `concave points_se`      | Continuous  | Standard error of concave points                |
| `symmetry_se`            | Continuous  | Standard error of symmetry                      |
| `fractal_dimension_se`   | Continuous  | Standard error of fractal dimension             |
| `radius_worst`           | Continuous  | Worst-case radius measurement                   |
| `texture_worst`          | Continuous  | Worst-case texture measurement                  |
| `perimeter_worst`        | Continuous  | Worst-case perimeter measurement                |
| `area_worst`             | Continuous  | Worst-case area measurement                     |
| `smoothness_worst`       | Continuous  | Worst-case smoothness measurement               |
| `compactness_worst`      | Continuous  | Worst-case compactness measurement              |
| `concavity_worst`        | Continuous  | Worst-case concavity measurement                |
| `concave points_worst`   | Continuous  | Worst-case concave points measurement           |
| `symmetry_worst`         | Continuous  | Worst-case symmetry measurement                 |
| `fractal_dimension_worst`| Continuous  | Worst-case fractal dimension measurement        |

## Next Steps
The upcoming sections will cover:
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Model Training & Evaluation
- Hyperparameter Tuning
- Feature Importance

Create a virtual environment (optional but recommended):

```sh
python -m venv venv
```

Activate the virtual environment:

- On Windows:
  ```sh
  venv\Scripts\activate
  ```
- On macOS/Linux:
  ```sh
  source venv/bin/activate
  ```

Navigate to the repository folder:

```
cd Breast-cancer-classifier
```

Install the required packages:

```sh
pip install -r requirements.txt
