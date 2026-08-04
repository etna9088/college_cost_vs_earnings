# The Return on Investment of a College Degree
An explanatory linear regression model built in R that analyzes U.S. Department of Education data to quantify how the cost of college tuition impacts future earnings.

## Business Problem or Objective
When evaluating higher education, students and families often make massive financial commitments based on prestige or "gut feeling" rather than quantitative data. The objective of this project is to treat a college degree as a financial asset. By analyzing historical tuition costs against median graduate earnings 10 years post-enrollment, this model provides a data-driven baseline to help determine if taking on higher student debt translates to proportionally higher long-term income.

## Core Features & Functionality
* **Explanatory Model:** Utilized linear regression to map the exact correlation between tuition and income, revealing that every $1 increase in attendance cost is associated with an approximate $4.59 increase in median earnings.
* **Variance Evaluation:** Calculated an R-squared value of 34.4%, indicating while tuition cost is a strong indicator of future earnings, other external variables (like major, location, and industry) play a heavier role in total income variation.
* **Categorical Profitability:** Designed distribution visualizations (violin plots) highlighting that private non-profit institutions generally yield higher and more varied long-term earnings compared to public or for-profit counterparts.

## Tech Stack & Tools
* **Language:** R 4.2 (`tidyverse`, `broom`, `infer`, `modelr`)
* **Environment:** RStudio (R Markdown)
* **Data Science:** Linear Regression, Exploratory Data Analysis, Residual Diagnostics
* **Version Control:** Git / GitHub

## Data Architecture & Pipeline
Raw data was extracted from the publicly available U.S. Department of Education College Scorecard dataset. The data was loaded into RStudio, where it underwent extensive wrangling to handle missing values and isolate the target variables (`COSTT4_A` and `MD_EARN_WNE_P10`). The clean data (3,075 institutions filtered from 6,429 raw records) was then modeled using standard regression algorithms to identify statistical significance and generate residual diagnostics.

## Installation & Deployment
To explore the code and final report locally:

1. Clone the repository to your local machine:
```bash
git clone [https://github.com/etna9088/college_cost_vs_earnings.git](https://github.com/etna9088/college_cost_vs_earnings.git)
```
2. Open the `college_cost_vs_earnings.Rproj` file using RStudio.
3. Install the required dependencies via the console:
```R
install.packages(c("tidyverse", "infer", "modelr", "broom"))
```
4. Open `final_project.Rmd` and click "Knit" to run the regression model and generate the final visualizations.
