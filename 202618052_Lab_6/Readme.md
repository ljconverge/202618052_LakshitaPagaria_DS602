# DS602 Lab 6 - Hypothesis Testing

## Overview

This repository contains the DS602 Lab 6 submission on applying statistical hypothesis tests to practical scenarios using Python. The accompanying notebook states the hypotheses, performs each test at a 5% significance level, and interprets the results.

## Contents

- `202618052_Assignment06_DS602.ipynb`: Jupyter notebook containing the hypothesis tests, Python implementation, and interpretations.
- `Readme.md`: Project overview, methodology, requirements, and reproducibility instructions.

## Topics Covered

1. **One-sample *t*-test**: Tests whether the mean restaurant total bill differs from $18.00 using Seaborn's `tips` dataset.
2. **Independent two-sample *t*-test**: Compares lunch and dinner tip amounts using the `tips` dataset, with Levene's test to assess equality of variances.
3. **Paired *t*-test**: Compares pulse measurements at 1 minute and 15 minutes using Seaborn's `exercise` dataset.
4. **Chi-square goodness-of-fit test**: Compares Titanic passenger-class proportions with a 25% / 25% / 50% baseline using Seaborn's `titanic` dataset.

## Methodology

- Uses pandas and Seaborn to load and inspect the datasets.
- Uses `scipy.stats` to perform the *t*-tests, Levene's variance test, and chi-square goodness-of-fit test.
- Applies a significance level of \(\alpha = 0.05\) to all hypothesis tests.
- Uses a two-sided alternative for each test and determines whether to reject the null hypothesis by comparing the p-value with the significance level.

## Requirements

- Python 3.x
- NumPy
- pandas
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook or JupyterLab

The required Python packages can be installed using:

```bash
pip install -r ../requirements.txt
```

## Reproducibility

1. Open `202618052_Assignment06_DS602.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
2. Ensure the required Python packages are installed.
3. Run the notebook cells sequentially from top to bottom.
4. Review the test statistics, p-values, and conclusions for each scenario.

## Implementation Notes

- The notebook uses Seaborn's `tips`, `exercise`, and `titanic` datasets. The first run may require an internet connection if the datasets are not already cached.
- The paired *t*-test compares pulse observations at 1 minute and 15 minutes from the assignment-specified `exercise` dataset.
- A statistically significant result does not, by itself, establish practical importance or causation.
