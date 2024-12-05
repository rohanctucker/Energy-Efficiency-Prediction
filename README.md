# Energy Efficiency Prediction

This project focuses on predicting building energy loads (heating and cooling requirements) using machine learning techniques. The study evaluates the influence of architectural features on energy efficiency and explores different models for improved prediction accuracy.

## Overview

- **Objective**: Analyze and predict building energy efficiency based on architectural parameters.
- **Machine Learning Models Used**:
  - Linear Regression
  - Decision Trees
  - Random Forest
- **Performance Metrics**: Mean Absolute Error (MAE), Mean Squared Error (MSE), R²
- **Key Findings**: The Random Forest model significantly outperformed others with an R² of 0.99.

## Features

- **Data Preparation**:
  - The dataset includes features such as Relative Compactness, Surface Area, Wall Area, Roof Area, Overall Height, Orientation, Glazing Area, and Glazing Area Distribution.
  - A new target variable (average of heating and cooling loads) was created, simplifying the analysis.
  - Verified the dataset had no missing values, outliers, or data type issues.
- **Correlation Analysis**: Key insights include:
  - A strong positive correlation between Overall Height and energy load.
  - Negative correlations between Surface Area, Roof Area, and energy load.
- **Model Evaluation**: Used cross-validation and hyperparameter tuning for Decision Tree and Random Forest models to optimize performance.

## Project Structure

- `analysis/`: Contains the main R Markdown file for analysis and code.
  - `Energy Efficiency Prediction.Rmd`: The analysis and machine learning implementation.
- `docs/`: Includes reports and presentations.
  - `Final Report.pdf`: Detailed project report with statistical summaries and conclusions.
  - `Energy Efficiency Prediction Using ML.pptx`: A presentation summarizing findings.

## Getting Started

1. **Prerequisites**:
   - R (version ≥ 4.0.0)
   - Required R packages: `tidyverse`, `randomForest`, `rmarkdown`
2. **Usage**:
   - Open and run `Energy Efficiency Prediction.Rmd` in RStudio to reproduce the analysis.
   - View `Final Report.pdf` for a comprehensive breakdown of the study.

## Results

| Model            | MAE  | MSE  | R²   |
|-------------------|------|------|------|
| Linear Regression | 1.88 | 6.70 | 0.92 |
| Decision Trees    | 1.40 | 3.34 | 0.96 |
| Random Forest     | 0.49 | 0.61 | 0.99 |

## Conclusion

This study demonstrates how architectural parameters significantly influence energy load requirements. The Random Forest model proved most effective, achieving near-perfect predictions with an R² of 0.99. These insights can guide architects and engineers in designing energy-efficient buildings by prioritizing features like Overall Height and optimizing other structural components.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Author

[Rohan](mailto:Rohanctucker@yahoo.com)
