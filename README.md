# Movie Industry Correlation Analysis

## Overview

This project investigates which movie attributes are most strongly associated with box office success.

Using a dataset containing movie information such as budget, ratings, votes, production companies, cast members, release dates, and gross earnings, the goal was to identify the factors that have the greatest relationship with revenue generation.

The analysis was conducted using Python and focused on data cleaning, and correlation analysis.

---

## Business Question

What factors are most strongly associated with high movie gross earnings?

Potential influencing variables include:

- Budget
- Production company
- Movie rating
- Cast
- Director
- Writer
- Runtime
- Critic and audience votes

---

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Visual Studio Code

---

## Data Cleaning

Several preprocessing steps were performed before analysis:

### Missing Values

- Identified missing data across columns
- Handled missing values appropriately to avoid biased results

### Data Types

- Inspected and corrected inconsistent data types
- Converted columns to suitable formats for analysis

### Duplicate Records

- Checked for duplicate entries
- Removed duplicates where necessary

### Feature Standardization

- Cleaned and standardized columns to ensure consistency during analysis

---

## Correlation Analysis
Visualizations were created to highlight patterns and detect potential correlations.
<img width="567" height="447" alt="image" src="https://github.com/user-attachments/assets/dedc187e-0fb5-4033-828e-18e5ea9522ef" />


Pearson correlation was used to measure relationships between numerical variables.

Categorical variables were encoded to allow further correlation analysis.

Example:

```python
correlation_matrix = df_numeric.corr(
    method='pearson',
    numeric_only=True
)
```

Heatmaps were generated using Seaborn to visualize correlation strength across features.
<img width="881" height="790" alt="image" src="https://github.com/user-attachments/assets/1b558678-3921-4d85-89da-5b42e0f752a4" />

---

## Key Findings

The analysis revealed that:

| Variable | Correlation with Gross Earnings |
|-----------|-----------|
| Budget | 0.75 |
| Votes | 0.63 |

Main observations:

- Budget has the strongest positive correlation with gross earnings.
- Movies receiving a higher number of votes also tend to generate higher revenue.
- Variables such as company, director, writer, and star actors showed considerably weaker correlations.
- Financial investment appears to be a stronger predictor of box office success than individual creative contributors.

---

## Conclusion

The study suggests that budget allocation and audience engagement, measured through votes, are the factors most strongly associated with movie revenue.

While correlation does not imply causation, the findings indicate that larger productions and movies generating higher audience attention are more likely to achieve stronger box office performance.

---


## Author

Aram Samb

