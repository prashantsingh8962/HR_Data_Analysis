# Step-by-Step Workflow for Employee Presence Dashboard

This documentation outlines the steps involved in analyzing HR attendance data and creating a Power BI dashboard to visualize employee presence, work-from-home (WFH), and sick leave (SL) trends.

---

## Step 1: Data Collection and Import

1. **Collect Employee Attendance Data**:
   - Gather the required attendance data. The data should contain:
     - **Employee Name**
     - **Dates**
     - **Attendance Status** (Present, WFH, Sick Leave, etc.)

2. **Prepare the Data**:
   - Ensure the data is structured in a tabular format (e.g., Excel, CSV).
   - Common columns include:
     - `Name`
     - `Date`
     - `Attendance Status` (e.g., P = Present, WFH = Work from Home, SL = Sick Leave)
  
3. **Import Data into Power BI**:
   - Open Power BI and select **Get Data**.
   - Import your dataset (e.g., Excel or CSV file).
   - Load the data into Power BI for analysis.

---

## Step 2: Data Cleaning and Preprocessing

1. **Review Data Quality**:
   - Ensure there are no missing or duplicate records.
   - Check for inconsistencies in attendance codes (P, WFH, SL).
   
2. **Create Calculated Columns**:
   - Use Power BI’s **Data** tab to create calculated columns for presence, WFH, and sick leave percentages.
     - For example: `Presence % = COUNTIF([Attendance Status] = "P") / Total Days`
   - You can use DAX formulas to create these calculations:
     ```DAX
     Presence % = 
     CALCULATE(
        COUNTROWS(AttendanceData),
        AttendanceData[Attendance Status] = "P"
     ) / COUNTROWS(AttendanceData)
     ```

3. **Create Date Columns**:
   - Extract additional date-based columns like **Day of Week**, **Month**, and **Year** if necessary.
     - Example: `Day of Week = FORMAT([Date], "DDD")`
     - Example: `Month = FORMAT([Date], "MMM")`

---

## Step 3: Build the Dashboard Layout

1. **Design the Dashboard Theme**:
   - Choose a consistent color scheme (e.g., yellow, blue, and green in the current dashboard).
   - Add a title section and your company logo for branding.

2. **Create KPI Cards**:
   - Insert **Card Visualizations** to display key metrics at the top of the dashboard:
     - **Presence %**
     - **WFH %**
     - **Sick Leave %**

3. **Design Data Tables**:
   - Add a table to display individual employee details (e.g., Presence %, WFH %, and Sick Leave %).
   - Ensure that the total values are calculated and displayed at the bottom of the table.

---

## Step 4: Visualize Time-Based Trends

1. **Create Line Charts for Time Trends**:
   - Use line charts to show how Presence %, WFH %, and SL % change over time.
   - X-axis: **Date** (grouped by month)
   - Y-axis: Corresponding percentage metrics.

2. **Breakdown by Day of Week**:
   - Create bar charts or line charts to show daily patterns for each metric (e.g., Presence % by day of the week).
   - This helps to see if specific days of the week have higher absenteeism or WFH rates.

3. **Filter the Data by Date**:
   - Add date filters (slicers) to allow users to focus on specific date ranges.
   - Place the date slicer at the top-right corner for easy access.

---

## Step 5: Add Interactivity

1. **Enable Drill-Down**:
   - Allow users to drill down from high-level trends to individual employee data.
   - For example, users can click on a day in the line chart and see the breakdown of attendance for that day.

2. **Cross-Filtering Between Visuals**:
   - Enable cross-filtering so that selecting an employee in the table will adjust other visualizations (e.g., the line charts will update to show that employee's attendance trends).

3. **Use Tooltips for Detail**:
   - Add tooltips to your visualizations so users can hover over data points and get more detailed information.

---

## Step 6: Validate and Finalize the Dashboard

1. **Validate Calculations**:
   - Verify that all calculated metrics (Presence %, WFH %, SL %) match expectations.
   - Cross-check the total percentages and individual employee data to ensure accuracy.

2. **Test Interactivity**:
   - Test all filters, slicers, and cross-filtering functionalities to make sure they work as intended.
   
3. **Adjust Visualizations**:
   - Fine-tune the dashboard’s visual aesthetics, ensuring the font sizes, colors, and layout are optimized for readability.

---

## Step 7: Share the Dashboard

1. **Publish the Dashboard**:
   - Publish the Power BI dashboard by selecting the **Publish** option.
   - Share the link with relevant stakeholders or embed it in a company portal for easy access.

2. **Export to PDF or PowerPoint**:
   - For static reporting, you can export the dashboard as a PDF or PowerPoint presentation and share it via email.
