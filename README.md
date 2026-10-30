# HR Analytics Dashboard

## Project Overview

This project analyzes employee data to understand workforce composition,
work-location patterns, hiring activity, and employee diversity. The
dashboard was created in **Microsoft Power BI** for the PRDA-03 HR
Analytics assignment.

## Project Objectives

-   Display total employee count.
-   Compare remote and headquarters (HQ) work percentages.
-   Show average employee age.
-   Explore hiring activity over time.
-   Analyze employee distribution by state, department, and race.
-   Visualize employee gender distribution.
-   Present findings that can support HR planning and decision-making.

## Dataset

The assignment describes an HR dataset containing employee information
such as: - Employee ID and name - Birthdate and age - Race - Department
and job title - Work location (HQ or Remote) - Hire date and termination
date - City and state

The supplied dashboard screenshot shows a gender field as well. The
assignment's written list of dataset attributes does not include gender,
so confirm that this field exists in the actual source table.

**Data privacy:** Database credentials and employee-identifying
information are intentionally not included in this README. Do not
publish credentials, employee names, or other personal information in a
public repository.

## Tools Used

-   Microsoft Power BI
-   Power Query for data preparation
-   DAX for KPI calculations and measures
-   MySQL database as the stated data source

## Dashboard KPIs

The dashboard screenshot displays the following values:

  KPI                        Displayed value
  ------------------- ----------------------
  Total employees       1K (rounded display)
  Remote percentage                   25.00%
  HQ percentage                       75.00%
  Average age                    38.55 years

The total employee card is rounded to `1K`; use the exact underlying
count when reporting final KPI values.

## Dashboard Visualizations

1.  **Employee Hiring Trend** --- line chart using hire date.
2.  **Employee Gender Distribution** --- donut chart.
3.  **Employees by State** --- bar chart.
4.  **Employees by Department** --- bar chart.
5.  **Employee Diversity by Race** --- bar chart.

## Key Observations from the Dashboard

These observations are based on the dashboard screenshot: - 25% of
employees are shown as remote and 75% as HQ-based. - The displayed
average employee age is 38.55 years. - Ohio is the largest state
category in the state chart. - Engineering is the largest department in
the department chart. - White is the largest displayed race category. -
Gender distribution is shown as Male: 531 (53.1%), Female: 440 (44.0%),
and Non-Conforming: 29 (2.9%).

State and department chart counts are not stated here because exact
values are not legible in the screenshot.

## Recommendations

-   Review Engineering staffing levels against workload and business
    needs.
-   Monitor geographic concentration, particularly the high employee
    count shown for Ohio.
-   Review remote and HQ working arrangements using productivity and
    employee-engagement measures.
-   Monitor diversity representation and support fair, inclusive
    recruitment and development.
-   Track annual hiring alongside employee exits to understand workforce
    growth and retention.

## Validation Notes

-   Confirm the exact total employee count from the underlying dataset;
    the dashboard card currently displays a rounded `1K`.
-   Check that the hiring trend is grouped by **year** (not individual
    hire dates). Use a Year field from `hire_date` on the X-axis and
    employee count on the Y-axis, sorted in ascending year order.
-   Verify that the `gender` field is present in the actual loaded
    dataset.
-   Keep blank termination dates as blank/null where they indicate no
    recorded termination.
-   Validate all observations against the underlying data before using
    them for business decisions.

## Project Deliverables

-   Power BI dashboard (`.pbix`)
-   Dashboard screenshots
-   HR analysis report (`.pdf`)
-   Project presentation (`.pptx`)
-   This README file

## Conclusion

The dashboard provides a snapshot of workforce size, work location, age,
hiring, geography, departments, race, and gender. It can help HR teams
identify workforce patterns and areas for further investigation.
Findings should be validated against the source dataset before final
submission or operational decisions.
