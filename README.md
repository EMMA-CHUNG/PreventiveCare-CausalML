# Healthcare Outreach Program Effectiveness Analysis

## Overview

This project implements a sophisticated causal inference analysis to evaluate the effectiveness of multiple healthcare outreach programs using advanced statistical techniques including:
- Inverse Probability Weighting (IPW)
- Marginal Structural Models (MSM)
- Doubly Robust Estimation

The analysis simulates healthcare outreach data and estimates the causal effects of different intervention programs on patient checkup completion rates.

## Key Features

- **Data Simulation**: Generates synthetic healthcare outreach data with:
  - 1000 patients
  - 12-month observation period
  - 3 different outreach programs
  - Realistic patient characteristics and completion probabilities

- **Causal Inference Techniques**:
  - Inverse Probability Weighting
  - Marginal Structural Models
  - Doubly Robust Estimation
  - Naive logistic regression for comparison

- **Advanced Statistical Methods**:
  - Logistic regression for treatment probability estimation
  - Gradient Boosting for outcome prediction
  - Bootstrap confidence interval estimation

## Dependencies

- NumPy
- Pandas
- Scikit-learn
- Statsmodels
- Matplotlib
- Seaborn

## Installation

1. Clone the repository
2. Install required dependencies:
```bash
pip install numpy pandas scikit-learn statsmodels matplotlib seaborn
```

## Methodology

### Simulation Parameters
- Total Patients: 1000
- Observation Period: 12 months
- Outreach Programs: A, B, C
- Baseline Characteristics:
  - Prior physical examination
  - Number of office visits

### Causal Inference Approaches

1. **Inverse Probability Weighting (IPW)**
   - Estimates treatment probabilities
   - Adjusts for potential confounding
   - Provides unbiased treatment effect estimates

2. **Marginal Structural Models (MSM)**
   - Accounts for time-varying treatments
   - Handles sequential treatment assignments
   - Provides robust effect estimates

3. **Doubly Robust Estimation**
   - Combines outcome modeling with IPW
   - Offers additional robustness
   - Provides confidence intervals for treatment effects

## Results Interpretation

The analysis compares three methods to estimate program effects:
- Marginal Structural Model (MSM)
- Doubly Robust (DR) Estimation
- Naive Logistic Regression

### Estimated Percentage Point Differences in Checkup Completion

| Program | True Effect | MSM (95% CI) | DR (95% CI) | Naive |
|---------|-------------|--------------|-------------|-------|
| A       | 12.0%       | Varies       | Varies      | Varies|
| B       | 8.0%        | Varies       | Varies      | Varies|
| C       | 15.0%       | Varies       | Varies      | Varies|

## Visualization

The project includes visualizations:
- Stabilized Inverse Probability Weight Distribution
- Comparative Program Effects Bar Chart

## Key Insights

- Demonstrates the importance of advanced causal inference techniques
- Shows how different methodological approaches can yield varying treatment effect estimates
- Provides a robust framework for analyzing healthcare intervention programs

## Limitations

- Uses simulated data
- Assumes specific underlying data generation process
- Results are illustrative of methodology, not real-world data

## Future Work

- Apply methodology to real-world healthcare datasets
- Explore more complex treatment assignment mechanisms
- Develop more sophisticated confounder adjustment techniques

## Contributing

Contributions, issues, and feature requests are welcome. Feel free to check the issues page.

