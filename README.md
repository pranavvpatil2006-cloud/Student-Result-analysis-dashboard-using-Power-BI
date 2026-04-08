Student Result Analytics Dashboard
An interactive Power BI dashboard designed to track, analyze, and visualize the academic performance of over 80 students. This project transforms raw academic records into actionable insights, allowing educators to identify trends, top performers, and students requiring additional support.

📊 Project Overview
The primary goal of this dashboard is to provide a comprehensive view of student progress. By leveraging Power BI’s analytical capabilities, the project moves beyond static spreadsheets to offer dynamic, drill-down insights into subject-wise and student-wise performance.

Key Features
Performance KPIs: Real-time tracking of average marks, pass rates, and total enrollment.

Dynamic Filtering: Filter data by student name, subject, or grade level.

Trend Analysis: Visualize performance across different assessment periods.

Drill-Down Capability: Navigate from high-level class averages down to individual student scorecards.

🛠️ Technical Stack
Tool: Power BI Desktop

Data Cleaning: Power Query (M Language)

Analytical Calculations: DAX (Data Analysis Expressions)

Data Source: Excel/CSV student records

🚀 Workflow & Implementation
1. Data Transformation (Power Query)
Before visualization, raw data underwent extensive cleaning to ensure accuracy:

Removed duplicates and handled missing values.

Standardized naming conventions for subjects and students.

Unpivoted columns to create a "Long Format" data structure, making it optimized for Power BI filtering.

2. Data Modeling
Implemented a Star Schema to ensure efficient data processing. The model connects the central "Results" fact table with dimension tables such as "Students" and "Calendar."

3. DAX Measures
Created custom calculations to drive the dashboard KPIs. Examples include:

Average Marks: AVERAGE(Results[Marks])

Performance Category: Used SWITCH and IF logic to categorize students into "Exceeding," "Meeting," or "Below" expectations based on percentage thresholds.

Rank: Utilized RANKX to dynamically rank students within their respective classes.

📈 Dashboard Insights
Average Marks: Provides a snapshot of the overall class health.

Subject Distribution: A bar chart showing which subjects students struggle with most.

Student Leaderboard: Highlights top-performing individuals based on weighted averages.

Pass/Fail Ratio: A donut chart indicating the percentage of students meeting the passing criteria.

📂 How to Use
Clone the Repo: git clone https://github.com/YourUsername/Student-Result-Analytics.git

Open the File: Ensure you have Power BI Desktop installed.

Explore: Open the .pbix file to interact with the visualizations.

💡 Conclusion
This dashboard serves as a powerful tool for academic data storytelling. It demonstrates the ability to take messy data, structure it effectively using Power Query, and derive meaningful business logic using DAX.
