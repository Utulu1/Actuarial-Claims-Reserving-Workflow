# Actuarial Claims Reserving Workflow Using Python

## Executive Summary

This project presents an end-to-end actuarial claims reserving workflow developed in Python, demonstrating the practical application of both deterministic and stochastic reserving techniques.

Using the **Chain Ladder** and **Mack Chain Ladder** methodologies, the analysis estimates outstanding insurance claim liabilities, evaluates reserve uncertainty and illustrates how actuarial analytics supports financial reporting, capital management and risk governance within general insurance.

Designed to reflect a real-world actuarial engagement, the project combines data preparation, actuarial modelling, validation and business interpretation into a transparent and reproducible analytical workflow.

![Python](https://img.shields.io/badge/Python-3.13-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange)
![Chain Ladder](https://img.shields.io/badge/Method-Chain%20Ladder-success)
![Mack Chain Ladder](https://img.shields.io/badge/Method-Mack%20Chain%20Ladder-success)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Business Problem

Insurance companies must estimate the value of claims that have already occurred but have not yet been fully settled. These estimates, known as **claims reserves**, are essential for maintaining financial stability, meeting regulatory requirements and ensuring that policyholder obligations can be met.

Underestimating reserves may expose an insurer to solvency risk, while overestimating reserves can reduce profitability and distort financial performance. Reliable reserving therefore plays a central role in actuarial practice, financial reporting and strategic decision-making.

This project demonstrates how actuarial techniques can be applied using Python to estimate outstanding claim liabilities while providing transparent, evidence-based insights for business decision-makers.

## Business Questions

This project addresses several key actuarial and business questions:

- What is the estimated value of outstanding insurance claim liabilities?
- Which accident years contribute most significantly to reserve risk?
- How reliable are the reserve estimates produced by deterministic methods?
- How does the Mack Chain Ladder method improve reserve assessment by quantifying uncertainty?
- What insights can support actuarial judgement and reserving decisions?

## Business Objective

The objective of this project is to estimate outstanding insurance claim liabilities by:

- Assessing historical claims development.
- Constructing cumulative paid loss triangles.
- Calculating development factors.
- Estimating ultimate losses.
- Quantifying outstanding reserves.
- Measuring reserve uncertainty using the Mack Chain Ladder method.

## Dataset

The project uses a historical insurance claims development dataset containing:

- Insurance Group Code
- Insurance Group Name
- Accident Year
- Development Year
- Development Lag
- Incurred Losses
- Cumulative Paid Losses
- Bulk Losses
- Earned Premium
- Posted Reserves

For demonstration purposes, the analysis focuses on the **Allstate Insurance Group** portfolio.

## Project Workflow

The reserving workflow follows a practical actuarial process:

1. Data Audit
2. Data Dictionary
3. Portfolio Familiarisation
4. Data Validation
5. Construction of Cumulative Paid Loss Triangle
6. Calculation of Age-to-Age Development Factors
7. Selection of Development Factors
8. Calculation of Cumulative Development Factors (CDFs)
9. Ultimate Loss Estimation
10. Outstanding Reserve Estimation
11. Mack Chain Ladder Reserve Uncertainty Analysis
12. Reserve Comparison
13. Actuarial Interpretation and Reporting

## Actuarial Methods

### Deterministic Reserving

- Chain Ladder Method

### Stochastic Reserving

- Mack Chain Ladder Method

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Chainladder (Python Library)
- Jupyter Notebook

## Repository Structure

```text
Actuarial-Claims-Reserving-Workflow/
│
├── data/
├── notebooks/
├── reports/
├── visualizations/
├── README.md
└── requirements.txt
```

## Key Results

The project successfully produced:

- Cumulative Paid Loss Triangle
- Age-to-Age Development Factors
- Selected Development Factors
- Cumulative Development Factors
- Estimated Ultimate Losses
- Outstanding Reserves by Accident Year
- Mack Chain Ladder Reserve Estimates
- Mack Standard Errors
- Reserve Comparison between Chain Ladder and Mack Chain Ladder

All generated figures are stored in the `visualizations/` directory.

## Model Assumptions

The Chain Ladder methodology relies on several important assumptions:

- Historical claims development patterns are representative of future claim development.
- Claims are reported and settled consistently over time.
- There are no material changes in claims handling practices, underwriting strategy, legislation, inflation, or the operating environment.
- Development factors remain reasonably stable across accident years.
- Past claims development provides a reliable basis for projecting future development.

## Model Limitations

Although widely used in actuarial practice, the Chain Ladder methodology has several limitations:

- Sensitive to unusual claims experience and large outliers.
- Assumes homogeneous development across accident years.
- Performance deteriorates when historical development patterns change.
- Does not explicitly model inflation or operational changes.
- Requires sufficient historical development data.

The Mack Chain Ladder extends the deterministic approach by providing reserve uncertainty estimates but still relies on the same underlying development assumptions.

## Skills Demonstrated

### Actuarial Skills

- Insurance Claims Reserving
- Chain Ladder Reserving
- Mack Chain Ladder
- Loss Development Triangle Analysis
- Development Factor Selection
- Reserve Estimation
- Reserve Uncertainty Analysis

### Technical Skills

- Python Programming
- Data Cleaning
- Data Validation
- Exploratory Data Analysis
- Statistical Analysis
- Data Visualisation
- Actuarial Reporting
- Reproducible Analytical Workflows

## Future Improvements

Potential extensions include:

- Bornhuetter–Ferguson Reserving
- Bootstrap Chain Ladder
- Generalised Linear Models (GLMs)
- Bayesian Reserving Techniques
- Interactive dashboards using Power BI or Streamlit

## Conclusion

This project demonstrates a complete actuarial claims reserving workflow implemented entirely in Python.

The analysis illustrates how deterministic and stochastic reserving methods can be combined to estimate outstanding claim liabilities while quantifying reserve uncertainty. The resulting workflow is transparent, reproducible, and closely reflects practical actuarial reserving processes performed within general insurance companies.

## Author

**Onyema Anthony Utulu**

*MSc. Actuarial Science | Aspiring Actuarial Analyst*

- **Email:** utulu.an@gmail.com
- **GitHub:** https://github.com/Utulu1
- **LinkedIn:** https://www.linkedin.com/in/utulu-an/
