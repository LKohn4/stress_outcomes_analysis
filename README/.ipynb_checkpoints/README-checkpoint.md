## Stress and Cognitive Performance Analysis

## Overview
This project analyzes the relationship between stress levels and cognitive performance using a dataset of 14,003 students.

## Dataset
- Source: Zenodo _ Student Performance and Learning Behavior Dataset
- Downlload: https://zenodo.org?records/16459132
- Sample Size: 14,003 students (12,469 after removing duplicates)

## Key Findings
- Stress affects cognitive performance
- Preparation moderates the stress effect

## Main Effect of Stress
- ANOVA Results: F(2, 12466) = 13.81, p < 0.001, n**2 = 0.002
- Performance by Stress Level:
  - Low Stress: Mean = 71.88 (SD = 17.52)
  - Medium Stress: Mean = 69.75 (SD = 17.84)
  - High Stress: Mean = 70.08 (SD = 17.63)

## Non-Linear Relationship
The relationship between stress and cognitive performance is not simply linear. Medium stress students performed significantly worse than both low and high stress groups. This suggests a complex interaction between perceived levels of stress and cognitive performance, and validates the theory of ideal zones of functioning (IZOF).

## Multiple Regression Analysis
- R**2 = .0022, explaining 2% of variance in exam scores
- Significant predictors: Preparation ('StudyHours')

## Methodology
1. Data Cleaning:
   - Removed 1,534 duplicate records (10.9% of original df)
   - Verified no missing values
   - Created categorical variables for analysis
   - Validated data quality and identified impossible values
2. Exploratory Data Analysis
   - Univariate analysis of key variables
   - Correlation analysis identifying relationships between predictors
   - Visualization of stress-performance relationship across subgroups
   - Exploration of moderating effects
3. Statistical Analysis
   - One-way ANOVA with effect size calculation
   - Post-hoc pairwise comparisons (Bonferroni corrected)
   - Simple and multiple linear regression
   - Moderation analysis with interaction terms
   - Regression diagnostics and assumption validation
4. Technologies Used
   - Python
   - Data analysis: pandas, numpy
   - Statistics: scipy, statsmodels, scikit-learn
   - Visualization: matplotlib, seaborn
   - Development: Jupyter Notebooks
## Practical Implications
- For students:
 - Low stress associated with optimal performance
 - Medium and high stress levels are detrimental to performance
 - Preparation and motivation can moderate stress effect
- For educators:
 - Encourage preparation and coping mechanisms
 - Stress management interventions may improve outcomes

## Future Directions
- Longitudinal analysis, analyze effect over time
- Machine learning models for performance prediction
- Causal inference using propensity score matching
- Interactive dashboard

## Project Structure
stress_outcomes_analysis/
|-data/
|--|-raw/
   |--najeemetal25.csv
   |-processed/
   |--cleaned_data.csv
|--|-notebooks/
   |--01_initial_data_exploration.ipynb
   |--02_data_cleaning.ipynb
   |--03_targeted_EDA.ipynb
   |--04_statistical_analysis
|--|-figures/
   |--comprehensive_eda_dashboard.png
   |--correlation matric.png
   |--high_stress_factors.png
   |--model_comparisson.png
   |--moderation_stress_study.png
   |--performance_distribution_by_stress.png
   |--regression_diagnostics.png
   |--stress_gender_interaction.png
   |--stress_motivation_interaction.png
   |--stress_performance_main_finding.png
   |--stress_study_interaction.png
|--|-README/
   |--README.md
   |--gitignore.txt
   |--requirements.txt

## License
This project uses data licensed under CC-BY 4.0. Data is available for educational and research purposes.

## Acknowledgements
Data sourced from Najeem, Kamal (2025). Student Performance and Learning Behavior Dataset for Educational Analytics. Zenodo. https://doi.org/10.5281/zenodo.16459132

## Contact
Leo Kohn
leo@kohn.be
https://www.linkedin.com/in/leo-kohn-955258195/
https://github.com/LKohn4/stress_outcomes_analysis.git
