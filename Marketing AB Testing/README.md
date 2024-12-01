# A/B Testing Analysis

## Project Overview
> This project aims to conduct an A/B test using a marketing dataset. The objective is to compare conversion rates between a **control group** and a **test group**, determining whether the test group results in a statistically significant improvement in conversions.

## Dataset Description
The dataset includes the following columns:
- **`user id`**: Unique identifier for each user.
- **`test group`**: Indicates whether the user is in the control (`ad`) or test (`psa`) group.
- **`converted`**: Indicates if the user converted (1 for Yes, 0 for No).
- **`total ads`**: Total number of ads viewed by the user.
- **`most ads day`**: Day of the week with the most ads viewed.
- **`most ads hour`**: Hour of the day with the most ads viewed.

## Steps Involved

### 1. Data Loading and Exploration
> Load the dataset and explore its structure to understand its contents and identify any anomalies.

### 2. Data Cleaning and Preparation
- Drop unnecessary columns.
- Segment the data into **control** and **test** groups.
- Check for missing values and data imbalance.

### 3. Calculate Conversion Rates
> Compute the conversion rate for both groups using the formula:
\[
\text{Conversion Rate} = \frac{\text{Number of Conversions}}{\text{Total Users}} \times 100
\]

### 4. Compare Conversion Rates
> Use visualizations to compare the conversion rates between the two groups for a clear understanding of the difference.

### 5. Statistical Testing
- Perform a **two-sample proportion z-test** to assess if the difference in conversion rates is statistically significant.
- Interpret the z-statistic and p-value to determine significance.

### 6. Interpretation of Results
> Based on the statistical test, provide actionable insights on whether the changes introduced in the test group are effective.

## Key Results
- **Control Group Conversion Rate**: 2.55%
- **Test Group Conversion Rate**: 1.79%
- **Statistical Test Outcome**: The difference in conversion rates is statistically significant 
                                (P-value: 1.7052807161559727e-13).

## Technologies Used
- **Python**: For data analysis and visualization.
  - `pandas` for data manipulation.
  - `matplotlib` and `seaborn` for visualizations.
  - `statsmodels` for statistical testing.


