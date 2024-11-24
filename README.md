# IS362 Assignment: Preprocessing Data for scikit-learn

## Overview
This project involves preprocessing a simulated Mushroom dataset to prepare it for use with machine learning models, particularly scikit-learn. The dataset is inspired by the UCI Mushroom Dataset and includes features such as mushroom edibility (`is_edible`), odor (`mushroom_odor`), and cap color (`cap_color`).

The assignment focuses on:
- Data preprocessing: cleaning, transforming, and encoding categorical variables into numerical format.
- Exploratory data analysis (EDA): visualizing distributions and relationships between features to draw insights.
- Preparing the data for machine learning tasks.

---

## Project Contents
- **Simulated Dataset**: A mock Mushroom dataset created within the Jupyter Notebook.
- **Data Preprocessing**: Transformation of categorical variables into numeric format to ensure compatibility with scikit-learn.
- **Exploratory Data Analysis (EDA)**:
  - Distribution plots for key variables.
  - Scatterplots to visualize relationships between the target variable (`is_edible`) and other features.

---

## Key Steps

1. **Dataset Creation**: 
   - A small mock dataset was created with three columns:
     - `is_edible` (edible or poisonous mushrooms).
     - `mushroom_odor` (types of odors).
     - `cap_color` (cap colors).
   - The dataset was converted into a pandas DataFrame.

2. **Column Renaming**:
   - Columns were renamed to have meaningful names:
     - `class` → `is_edible`
     - `odor` → `mushroom_odor`
     - `cap-color` → `cap_color`

3. **Data Transformation**:
   - Categorical variables were encoded into numeric values:
     - `is_edible`: `e` (edible) → `1`, `p` (poisonous) → `0`.
     - `mushroom_odor`: Encoded into numeric labels.
     - `cap_color`: Encoded into numeric labels.

4. **Exploratory Data Analysis (EDA)**:
   - Visualized the distribution of each column using count plots.
   - Created scatterplots to analyze the relationship between `is_edible` and other features.

---

## Key Findings
- **Odor (`mushroom_odor`)** is the most significant feature for determining edibility, with certain odors strongly associated with poisonous mushrooms.
- **Cap Color (`cap_color`)**, while showing some differences between edible and poisonous mushrooms, is less predictive than odor.

---

## Recommendations
1. Future work can explore additional features such as habitat and spore print color to improve prediction models.
2. `mushroom_odor` should be prioritized as a key feature when training machine learning classifiers.
3. Additional analysis on a larger dataset can enhance insights and improve model accuracy.
