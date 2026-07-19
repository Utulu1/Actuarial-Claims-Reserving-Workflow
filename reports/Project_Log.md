
## Project

**Actuarial Claims Reserving Workflow**

**Dataset:** CAS Workers' Compensation Database

---

# Session 1 – Project Setup

## Objectives

- Define the project scope.
- Obtain a real-world actuarial dataset.
- Establish professional project documentation.
- Perform an initial audit of the dataset.

---

## Tasks Completed

### Project Setup

- Created project folder structure.
- Created documentation files:
  - Project Brief
  - Business Assumptions
  - Data Dictionary
  - Data Audit Report
  - Project Log

### Data Acquisition

- Downloaded the CAS Workers' Compensation Loss Reserving Database.
- Imported the dataset into Python.
- Verified successful data loading.

### Data Audit

Completed the following quality checks:

- Dataset dimensions
- Variable types
- Missing value assessment
- Duplicate record assessment
- Portfolio structure
- Accident years
- Development periods

---

## Key Findings

### Dataset Summary

| Metric | Value |
|---------|------:|
| Observations | 12,100 |
| Variables | 13 |
| Insurance Groups | 132 |
| Accident Years | 10 |
| Development Periods | 10 |

The dataset contains a complete longitudinal claims history suitable for actuarial reserving analysis.

---

## Portfolio Selection

To replicate a realistic actuarial reserving engagement, **Allstate Insurance Group** was selected as the client portfolio.

Selected Portfolio:

- 100 observations
- 10 Accident Years
- 10 Development Periods

This forms a complete **10 × 10 claims development triangle**.

---

## Exploratory Portfolio Review

Completed:

- Summary statistics
- Distribution of cumulative paid losses
- Initial portfolio familiarisation

### Key Observations

- Claims exhibit a highly right-skewed distribution.
- Most observations contain relatively small claim values.
- A small number of claims contribute disproportionately large losses.
- Posted reserves remain constant across observations because they represent the insurer's total reported reserve at the valuation date.

---

## Data Validation

Negative claim values were investigated.

### Findings

| Variable | Negative Records | Percentage |
|----------|----------------:|-----------:|
| Cumulative Paid Loss | 73 | 0.60% |
| Incurred Losses | 60 | 0.50% |

### Decision

The negative observations were retained because they likely represent legitimate insurance accounting adjustments, including reserve revisions, recoveries, salvage, or subrogation recoveries.

No evidence suggests that these records are data quality errors.

---

## Skills Demonstrated

- Real-world actuarial data acquisition
- Data quality assessment
- Exploratory data analysis
- Insurance portfolio familiarisation
- Claims data validation
- Professional actuarial documentation

---

## Next Session

The next phase will focus on constructing the **claims development triangle**, which forms the foundation of actuarial reserving techniques such as:

- Chain Ladder
- Mack Chain Ladder
- IBNR estimation
- Outstanding claims reserve estimation

## Lessons Learned

- Real insurance datasets may legitimately contain negative claim values due to accounting adjustments.
- Data validation requires business understanding, not just statistical checks.
- Professional actuarial analysis begins with data quality assessment before any reserving model is developed.
- Clear documentation improves the transparency and reproducibility of actuarial work.

## Valuation Triangle and Development Factors
Constructed a realistic valuation triangle by removing future development periods.
Recalculated age-to-age development factors using only information available at the valuation date.
Selected actuarially appropriate development factors.
Calculated cumulative development factors (CDFs).
Saved selected development assumptions for reserve estimation.

## Ultimate Loss Estimation
Applied Chain Ladder cumulative development factors to the latest cumulative paid losses.
Estimated ultimate claim costs for each accident year.
Confirmed that mature accident years required no further development.
Preserved historical negative claim development identified during the data audit.
Saved projected ultimate losses for subsequent reserve calculations.

## Outstanding Reserve Estimation
Calculated outstanding reserves for each accident year.
Aggregated reserves across the portfolio.
Created a consolidated reserve estimation workpaper.
Saved reserve estimates for reporting.

## Deterministic Chain Ladder Completed

Completed the deterministic Chain Ladder reserving workflow.

Tasks completed:
- Constructed cumulative paid loss triangle.
- Calculated age-to-age development factors.
- Selected average development factors after removing invalid values.
- Computed cumulative development factors (CDFs).
- Estimated ultimate losses.
- Calculated accident-year outstanding reserves.
- Produced reserve summary table.
- Estimated total outstanding reserve (≈3.56).

Outputs saved:
- paid_loss_triangle.csv
- age_to_age_factors.csv
- selected_development_factors.csv
- cumulative_development_factors.csv
- outstanding_reserves.csv
- reserve_summary.csv