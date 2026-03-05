KPI Dictionary — Canadian Telecom Efficiency Dashboard (2020–2024)

Dataset & Model Context

Grain: Year (industry-level, Canada)

Units: Revenue is provided in CAD millions by StatCan; employment is persons.

| KPI                   | Field / Calculation Name   | Definition                                                                                         | Formula (plain)                                     | Unit              | Interpretation                                                                                                                                             |
| --------------------- | -------------------------- | -------------------------------------------------------------------------------------------------- | --------------------------------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Total Revenue         | `Revenue_Million_CAD`      | Total telecom operating revenue (industry-level).                                                  | Sum of annual revenue values.                       | CAD (millions)    | Higher = larger industry revenue base.                                                                                                                     |
| Revenue YoY Growth    | `Revenue_YoY_Pct`          | Year-over-year revenue growth rate.                                                                | (Revenue_t − Revenue_(t−1)) / Revenue_(t−1)         | %                 | Positive = revenue growth; negative = decline.                                                                                                             |
| Total Employees       | `Employees_Count`          | Telecom employment proxy (industry-level headcount).                                               | Sum of annual employment values.                    | Persons           | Higher = larger workforce/capacity proxy.                                                                                                                  |
| Employment YoY Growth | `Employment_YoY_Pct`       | Year-over-year workforce change rate.                                                              | (Emp_t − Emp_(t−1)) / Emp_(t−1)                     | %                 | Positive = hiring/expansion; negative = contraction.                                                                                                       |
| Revenue per Employee  | `Revenue_Per_Employee_CAD` | Productivity proxy: revenue generated per employee. Revenue is converted from millions to dollars. | (Revenue_Million_CAD × 1,000,000) / Employees_Count | CAD per employee  | Higher = more revenue per employee (proxy for productivity/efficiency).                                                                                    |
| Productivity Gap      | `Growth_Gap_Pct`           | Difference between revenue growth and workforce growth.                                            | Revenue_YoY_Pct − Employment_YoY_Pct                | percentage points | Positive = revenue growing faster than workforce (efficiency/prod gain); negative = workforce growing faster than revenue (potential efficiency pressure). |

Notes & Conventions

Revenue unit conversion: StatCan revenue is in millions. For per-employee metrics, revenue is converted to dollars by multiplying by 1,000,000.

YoY metrics: First year in the series has no prior year; YoY values may be null/blank for that year.

Interpretation caution: These are industry-level proxies, not firm-specific operational efficiency measures.

Revenue (Selected Year): IF Year = [Selected Year] THEN Revenue_Million_CAD END

Revenue (Prev Year): IF Year = [Selected Year]-1 THEN Revenue_Million_CAD END

Revenue YoY % (Selected): computed from the selected + previous year values.
