# Employee Presence Dashboard_HR

This project analyzes employee presence, sick leave, and work-from-home (WFH) trends based on HR data. The data is visualized in a comprehensive Power BI dashboard, providing insights into attendance patterns over a period of time.

## Project Overview

The **Employee Presence Dashboard** tracks and visualizes employee attendance, categorizing it into:
- **Presence %**: The percentage of time employees are physically present at work.
- **Work From Home (WFH) %**: The percentage of time employees worked remotely.
- **Sick Leave (SL) %**: The percentage of time employees were on sick leave.

The dashboard displays trends and allows filtering based on dates to highlight fluctuations in attendance, WFH, and sick leave patterns over months and weekdays.

### Key Insights

- **Overall Metrics:**
  - **Presence %**: 91.8%
  - **Work From Home (WFH) %**: 10.0%
  - **Sick Leave (SL) %**: 1.1%
  
- **Daily Trends**:
  - **Presence %** peaks on **Monday** with 93.2%.
  - **WFH %** shows higher activity on **Thursday** at 11.5%.
  - **Sick Leave (SL) %** has the highest rate on **Thursday** at 1.2%.

- **Employee Breakdown**:
  - The table shows individual employee percentages for Presence, WFH, and Sick Leave.
  - Employees like **Gregory Carr** had a **100% WFH** rate, while **Kaylah Schultz** recorded **25.6% WFH** and **0% Sick Leave**.

- **Time-Based Trends**:
  - **Presence % by Date**: Fluctuations observed across April to June, with an overall increase towards June.
  - **WFH % by Date**: Shows consistent remote working patterns with some spikes in May.
  - **SL % by Date**: Sick leave occurrences show variability, with peaks in early June.

## Files and Resources

- **Dashboard File**: The dashboard was created using Power BI and leverages various visualization techniques, such as line charts and data tables, for effective reporting.
  
- **Data Source**: The HR data for this analysis includes employee attendance records from April 2022 to June 2022, segmented by dates, WFH days, and sick leave days.

  ## Preview:

![dashboard](https://github.com/prashantsingh8962/HR_Data_Analysis/blob/main/Resources/Screenshot%202024-09-21%20141819.png)  


## How to Use the Dashboard

1. **Filter by Date**: Use the date filters on the top-right of the dashboard to view trends for specific time frames.
2. **Analyze Key Metrics**: The cards at the top of the dashboard display overall percentages for Presence, WFH, and Sick Leave.
3. **Explore Time-Based Trends**: Review the line charts to understand how these percentages vary over time.
4. **Employee-Level Insights**: Scroll through the table to view individual employee data on Presence, WFH, and Sick Leave.

## Future Enhancements

- Include more granular analysis by department or team.
- Add advanced filtering options such as job roles or location-based metrics.
- Incorporate predictive analytics to forecast employee presence and absenteeism trends.

---

### Tools Used:
- **Power BI**: For data visualization and dashboard creation.
- **Excel/CSV**: For raw data storage and initial processing.
- **DAX**: To calculate measures and perform data transformations.

### Files in the Repository:
- **AttendanceData.xlsx**: The source dataset.
- **EmployeePresenceDashboard.pbix**: The Power BI file with the final dashboard.
- **README.md**: Overview of the project (this document).
- **Dashboard_Screenshots/**: Folder containing dashboard screenshots for preview.
