# Gym Analytics Dashboard

An interactive **Power BI dashboard** designed to explore gym membership, member demographics, fitness metrics, and financial performance.

## Project Overview

The Gym Analytics Dashboard brings key gym information into one report. It includes an overall performance page, a calorie calculator, and a member analysis page. The report is organized with page navigation to make it easy to move between views.

## Dashboard Pages

### 1. Home
- Landing page for the Fitness Analytics Dashboard.
- Provides navigation to the report sections.

### 2. Overall
- High-level view of gym activity and business performance.
- Includes KPI cards and visual summaries.
- Provides breakdowns using charts and slicers.
- Tracks key measures such as member count, trainer count, revenue, expenses, and profit.

### 3. Calculator
- Interactive calorie calculator page.
- Includes inputs for age, height, and weight.
- Displays BMI and a calorie result.
- Intended to provide an estimated daily calorie requirement and simple guidance for weight gain or weight loss.

### 4. Members
- Member information table.
- Member distribution by age and membership category.
- Member distribution by age and gender.
- Includes member-focused KPI cards and filtering.

## Key DAX Measures

The report includes the following DAX measures:

| Measure | Description |
|---|---|
| `Users_Count` | Counts rows in the `Users` table. |
| `Trainer` | Counts distinct trainer names in the `Users` table. |
| `Revenue` | Sums `Payments[Amount]`. |
| `Expanses` | Sums `Expenses[Amount]`. |
| `Profit` | Calculates revenue minus expenses. |
| `Gold_Active` | Counts active Gold members. |
| `Gold_Expired` | Counts expired Gold members. |
| `Platinum_Active` | Counts active Platinum members. |
| `Platinum_Expired` | Counts expired Platinum members. |
| `Silver_Active` | Counts active Silver members. |
| `Silver_Expired` | Counts expired Silver members. |

## Tools and Technologies

- **Microsoft Power BI Desktop** — report development and data visualization
- **DAX** — measures and calculations
- **Power Query** — data preparation, if used in the report workflow

## How to Use

1. Download or clone this repository.
2. Open `Gym dashboard.pbix` using **Power BI Desktop**.
3. Allow the report to load. If Power BI prompts for data-source credentials or file paths, update the source settings to match your environment.
4. Use the page navigation and available slicers/filters to explore the report.
5. On the Calculator page, enter the requested values to view the displayed BMI and calorie estimate.

## Repository Contents

```text
.
├── Gym dashboard.pbix
├── README.md
└── screenshots/
    ├── overall-dashboard.png
    ├── calculator.png
    └── members.png
```

Add your dashboard screenshots to the `screenshots/` folder and update the image links below when the screenshots are available.

## Dashboard Preview

### Overall Dashboard
![Overall Dashboard](screenshots/overall-dashboard.png)

### Calorie Calculator
![Calorie Calculator](screenshots/calculator.png)

### Members Analysis
![Members Analysis](screenshots/members.png)

## Notes

- The `.pbix` file is the interactive Power BI report. GitHub may not display its contents as a dashboard preview; users generally need to download it and open it in Power BI Desktop.
- The dashboard's displayed results depend on the data loaded into the report and its refresh configuration.
- The calorie calculator provides estimates and should not be treated as medical advice.

## Author

**Dhaneshwari**
