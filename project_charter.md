Title
Revenue Growth vs Employment Growth in Canadian Telecommunications (2020–2024)

Objective
Analyze whether revenue growth in the Canadian telecommunications sector is aligned with operational capacity over time using public, industry-level financial and workforce data. Identify productivity trends and potential resourcing misalignment signals.

Core Business Question
Is revenue growth in Canadian telecommunications outpacing operational capacity, and what does this imply for productivity and future resource planning?

Audience / Use
Operations / performance management stakeholders (industry-level view).
Portfolio context: demonstrates KPI definition, data preparation, and dashboard storytelling.

Scope

Geography: Canada

Industry: Telecommunications (NAICS 517; workforce series uses NAICS 5173 where applicable)

Time period: 2020–2024 (or earliest available through most recent in selected StatCan tables)

Level: Industry-level (aggregated; not firm-specific)

Out of scope: company-internal utilization, service-level/region-level performance, causal inference

KPIs (Definitions)

Total Telecom Revenue (CAD, millions): industry operating revenue

Revenue YoY Growth (%): (Revenue_t − Revenue_(t−1)) / Revenue_(t−1)

Employment Level (count): telecom employment proxy (wired & wireless carriers where applicable)

Employment YoY Growth (%): (Emp_t − Emp_(t−1)) / Emp_(t−1)

Revenue per Employee (CAD): (Revenue * 1,000,000) / Employment

Productivity Gap (%): Revenue YoY % − Employment YoY %

Data Sources

Statistics Canada — telecom financial statistics (industry operating/financial detail tables)

Statistics Canada — employment by telecom industry / carriers (employment proxy)

Deliverables

Excel model (telecom_ops_kpi_model.xlsx): cleaned tables + KPI calculations (YoY, revenue/employee, gap)

Tableau dashboard (Telecom Ops KPI Dashboard.png + Tableau Public link):

KPI tiles (year-selectable)

Growth quadrant (Revenue YoY vs Employment YoY)

Revenue vs Employment YoY trend

Revenue per Employee trend

README + documentation: short explanation, KPI dictionary (optional)

Success Criteria (Practical)

KPIs update correctly when changing the Selected Year parameter

Dashboard clearly communicates:

whether revenue growth is outpacing workforce growth

how revenue per employee changes over time

All metric definitions are consistent across Excel and Tableau

Assumptions & Limitations

“Operational capacity” is represented by industry employment proxy, not internal utilization metrics.

Analysis is based on public aggregated data; results reflect industry trends, not specific firms.

“Productivity” is inferred via financial-to-labour ratios; not a direct efficiency measurement.

Different NAICS cuts (e.g., 517 vs 5173) may create slight comparability differences; this is noted in documentation.
