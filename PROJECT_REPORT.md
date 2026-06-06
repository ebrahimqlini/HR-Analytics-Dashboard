# HR Analytics Project Report

## 1) Objective

Build a Power BI dashboard that gives HR leadership a single view of workforce size, department distribution, salary patterns, leave usage, overtime load, and growth over time.

## 2) Data Overview

The dataset contains **689 employees** across **15 fields**.

### Quality Check

- Missing values: **0**
- Duplicate records: **0**
- Countries covered: **5**
- Departments covered: **20**
- Time coverage: **2016-2020**

### Core Fields

- Employee identity and demographics
- Department and country
- Start date and years of service
- Salary data
- Job rate
- Sick leave, unpaid leave, and overtime hours

## 3) Executive KPIs

| KPI | Value |
|---|---:|
| Total Employees | 689 |
| Average Performance Rating | 3.6 |
| Average Sick Leaves per Employee | 1.61 |
| Average Unpaid Leaves per Employee | 0.76 |
| Average Overtime Hours per Employee | 13.70 |
| Total Annual Salary | 17.10M |
| Average Annual Salary | 24.8K |

## 4) Main Findings

### Workforce concentration

- **Manufacturing** is the largest department with **140 employees**.
- **Egypt** holds the largest workforce base with **379 employees**.
- **Male employees** represent **65%** of the dataset, while **female employees** represent **35%**.

### Growth trend

- Headcount increased steadily from **51 in 2016** to **248 in 2019**.
- It then dropped to **162 in 2020**, which deserves management review.

### Compensation

- The strongest average salary appears in **Human Resources** at about **30.7K**.
- The weakest average salary appears in **Research Center** at about **22.6K**.
- Overall salary levels vary across departments more than across countries.

### Leave and overtime

- Average sick leave is **1.61** days per employee.
- Average unpaid leave is **0.76** days per employee.
- The overtime-to-sick-leave correlation is approximately **-0.03**, which is effectively negligible.

### Performance and workforce quality

- Average job rate is **3.6**.
- The highest average job rates appear in:
  - Human Resources
  - Major Mfg Projects
  - Environmental Health/Safety
- The lowest average job rates appear in:
  - Green Building
  - Training
  - Research/Development

### Diagnostic Details

The diagnostic page shows that the organization does not have one single workforce issue, but rather a few department-specific patterns that need different responses.

- **Major Mfg Projects** has the highest overtime, making it the clearest workload-pressure department.
- **Human Resources** is the strongest overall department because it combines the highest salary and the highest job rate.
- **Research Center** is the main red flag because it combines the highest sick leave, the lowest salary, and a weaker job rate.
- **Manufacturing** drives the largest total payroll, which means headcount has a bigger impact on salary spend than average salary alone.
- The department-level view is more useful than the company-wide average because it exposes where risk and pressure are concentrated.

## 5) Business Interpretation

This dashboard is useful because it combines three HR views in one place:

1. **Workforce structure** - how people are distributed by department, country, and gender.
2. **Workforce cost** - how salaries differ across business units.
3. **Workforce usage** - how much overtime and leave activity exists across the organization.

That makes it suitable for:
- workforce planning
- compensation review
- leave policy analysis
- regional comparison
- executive reporting

The new diagnostic page strengthens the report by moving beyond simple averages and pointing to departments that may need HR follow-up.

## 6) Recommendations

1. Investigate the 2019 to 2020 headcount drop to identify whether it reflects attrition, hiring slowdown, or restructuring.
2. Review salary bands for departments at the top and bottom of the pay distribution.
3. Extend the model with tenure, attrition, promotions, and manager-level fields.
4. Add drill-through views for country and department deep dives.
5. Add a time-series page to distinguish growth seasonality from one-off changes.

## 7) Analytical Caveats

- The dataset is descriptive and does not contain exit data.
- Correlation does not imply causation.
- Some country and department groups are small, so averages for those segments are less stable.

## 8) Suggested Next Version

If this project is extended, the next version should include:

- turnover and retention analysis
- hiring funnel metrics
- tenure segmentation
- salary percentile bands
- manager-level performance and leave views
