# Construction Project Performance Dashboard

Power BI dashboard analysing cost, duration, and risk across 1,300 construction tasks, helping identify which tasks drive the most cost and risk exposure.

## Project Overview

This project analyses a task-level construction dataset covering duration, labor, equipment, material cost, and risk classification. The goal is to help project teams quickly identify high-cost, high-risk, and resource-heavy tasks that need closer management attention.

## Objectives

- Track total project cost and task volume at a glance
- Compare cost and duration across risk levels (Low / Medium / High)
- Identify which tasks are the biggest cost and risk drivers
- Support resourcing decisions using labor and equipment data

## System Architecture

- **Data Collection Layer** — task-level construction dataset (1,300 tasks)
- **Data Processing Layer** — Power Query type validation
- **Analysis Layer** — DAX measures for totals, averages, and risk segmentation
- **Visualisation Layer** — Power BI dashboard (2 pages)

## Key Features

- KPI cards: total tasks, total material cost, average duration, average labor, high-risk task %
- Cost breakdown by risk level (bar chart)
- Duration vs cost scatter plot, sized by labor requirement, coloured by risk
- Sortable task-level cost and risk table
- Interactive slicers for risk level and dependency count

## Technologies Used

- Microsoft Power BI (Power Query, DAX)
- Python (pandas) for initial data validation

## Data Pipeline Workflow

1. Data import (task-level construction dataset)
2. Data type validation in Power Query
3. DAX measure creation (totals, averages, risk segmentation)
4. Dashboard visualisation across 2 pages

## Use Cases

- Construction project cost monitoring
- Risk-based task prioritisation
- Resource (labor/equipment) planning
- Project management reporting

## Data Limitations

This dataset is task-level and does not include actual project dates, a start/end timeline, or an on-time-vs-delayed flag. It supports cost, duration, and risk analysis, but not calendar-based progress tracking. A future version could add scheduling data for true delay analysis.

## Screenshots

![Overview Page](screenshots/overview.png)
![Cost and Risk Analysis Page](screenshots/cost_risk_analysis.png)

## Key Learnings

- DAX measure design for segmented KPI reporting (COUNTROWS, CALCULATE with filter conditions)
- Scatter plot analysis for multi-variable comparison (cost, duration, labor, risk)
- Dashboard structuring for stakeholder-ready reporting

## Future Improvements

- Add real project timeline/date data for true delay and schedule-variance analysis
- Add budget-vs-actual comparison if budget data becomes available
- Add site/location breakdowns

## Author

Anne Subashini Sritharan

## Project Note

This project demonstrates how Power BI can turn task-level construction data into a clear view of cost drivers and risk exposure to support project management decisions.

