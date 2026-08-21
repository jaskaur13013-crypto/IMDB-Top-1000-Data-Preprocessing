# IMDB Movie Ratings — Data Cleaning & Predictive Analysis

A data analysis project exploring what drives IMDB movie ratings, using a Kaggle movie dataset. The project covers data cleaning, exploratory data analysis (EDA), and preparation of a clean, leak-free dataset for a movie-rating prediction model.

## Overview

This project analyzes a **1,000-row, 16-column** movie dataset to understand which factors most strongly influence IMDB ratings. It focuses heavily on rigorous data cleaning and exploratory analysis before any modeling is attempted, ensuring the dataset is reliable and free of bias introduced by missing or skewed values.

## Dataset

- **Source:** Kaggle
- **Size:** 1,000 rows × 16 columns
- **Content:** Movie-level data including titles, genres, ratings, critic scores (Metascore), revenue, and other metadata

## Key Steps

### 1. Missing Value Treatment
- Applied **mode imputation** for missing values in categorical columns
- Applied **median imputation** for two numeric columns that were right-skewed, avoiding distortion that mean imputation would introduce from outlier values

### 2. Exploratory Data Analysis (EDA)
- Explored relationships between variables using Python (Pandas, NumPy)
- Built visualizations with Matplotlib and Seaborn to identify trends and correlations
- Worked collaboratively as part of a team to validate findings

### 3. Data Preparation for Modeling
- Applied an **80/20 train-test split**
- Performed **feature scaling** to keep the pipeline clean and free of data leakage ahead of model training (Scikit-learn)

## Key Findings

- **Metascore (critic score)** showed the strongest correlation with IMDB user ratings, more so than other available features.
- **Revenue** was heavily right-skewed, driven by a small number of top-grossing blockbuster titles rather than being evenly distributed across the dataset.

## Tools & Libraries

| Category | Tools |
|---|---|
| Language | Python |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning Prep | Scikit-learn |

## Project Structure

```
├── data/
│   └── imdb_movies.csv          # Raw dataset
├── notebooks/
│   └── imdb_analysis.ipynb      # Cleaning, EDA, and preprocessing steps
├── README.md
└── requirements.txt
```

*(Update this section to match your actual folder/file names.)*

## How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/jaskaur13013-crypto/<your-repo-name>.git
   cd <your-repo-name>
   ```
2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```
3. Open and run the notebook
   ```bash
   jupyter notebook notebooks/imdb_analysis.ipynb
   ```

## Future Work

- Train and evaluate the actual rating-prediction model (e.g., Linear Regression, Random Forest) on the cleaned dataset
- Add cross-validation and hyperparameter tuning
- Expand the dataset with more recent titles for broader generalization

## Author

**Jasmeet Kaur**
[LinkedIn](https://www.linkedin.com/in/jasmeet-kaur-730096363) · [GitHub](https://github.com/jaskaur13013-crypto)
