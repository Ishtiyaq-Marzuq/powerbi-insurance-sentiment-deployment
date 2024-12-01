# Power BI Insurance Sentiment Analysis and Deployment Framework
A Power BI project for insurance data analysis featuring advanced visualizations, sentiment analysis, role-based security (RLS),scheduling refresh and seamless deployment for insightful decision-making and reporting.

![Alt text](https://github.com/Ishtiyaq-Marzuq/powerbi-insurance-sentiment-deployment/blob/main/Insurance%20Analysis.png)

![Alt text](https://github.com/Ishtiyaq-Marzuq/powerbi-insurance-sentiment-deployment/blob/main/Sentiment%20Analysis.png)

## Table of Contents

1. [Introduction](#introduction)
2. [Project Steps](#project-steps)
   - [1. Importing Data to MSSQL Server](#importing-data-to-mssql-server)
   - [2. Loading Data to Power BI Desktop](#loading-data-to-power-bi-desktop)
   - [3. Visualizations](#visualizations)
     - [Table View & Data Profiling](#table-view--data-profiling)
     - [Adding Slicers & Text](#adding-slicers--text)
     - [Adding Card Visuals](#adding-card-visuals)
     - [Adding Donut Chart & Matrix Visual](#adding-donut-chart--matrix-visual)
     - [Adding Multi Row Card & Ribbon Chart](#adding-multi-row-card--ribbon-chart)
     - [Adding Bar & Line Chart](#adding-bar--line-chart)
   - [4. Create Power BI Account](#create-power-bi-account)
   - [5. Publishing the Report to Power BI Service](#publishing-the-report-to-power-bi-service)
   - [6. Creating a Workspace](#creating-a-workspace)
   - [7. Scheduling Data Refresh](#scheduling-data-refresh)
   - [8. Drill Through Filters](#drill-through-filters)
   - [9. Testing Scheduled Refresh & Updating Report](#testing-scheduled-refresh--updating-report)
   - [10. Creating & Testing Roles in Power BI Desktop](#creating--testing-roles-in-power-bi-desktop)
   - [11. Implementing Row-Level Security (RLS)](#implementing-row-level-security-rls)
   - [12. Sentiment Analysis in Power Query](#sentiment-analysis-in-power-query)
   - [13. Deployment into Workspace](#deployment-into-workspace)


---

## Introduction

This project demonstrates the analysis of insurance data using Power BI, a powerful data visualization and business intelligence tool. By transforming raw insurance data into meaningful visualizations and reports, this project aims to provide stakeholders with actionable insights for decision-making. The project involves multiple steps, including importing and processing data, creating interactive visualizations, implementing security features like Row-Level Security (RLS), and integrating sentiment analysis. The outcome is a dynamic Power BI report that enables users to interact with the data, view key metrics, and make informed decisions based on the trends and insights presented.

---

## Project Steps

### 1. Importing Data to MSSQL Server

The first step of the project was to import the raw insurance dataset into an MSSQL Server database. This process involved connecting to the database, creating tables, and ensuring that the data was organized and properly structured. By storing the data in an MSSQL Server, the dataset became easily accessible for data analysis and reporting, allowing us to work with large datasets efficiently. The database connection was set up in Power BI, ensuring seamless integration and extraction of the data for further processing.

### 2. Loading Data to Power BI Desktop

Once the insurance data was imported into MSSQL Server, the next step was to load it into Power BI Desktop. Power BI Desktop provides powerful data modeling capabilities, where users can connect to a variety of data sources, including SQL databases, Excel files, and online services. After loading the data into Power BI, various transformations and cleaning procedures were performed, including renaming columns, handling missing values, and creating relationships between tables. This step ensures that the data is well-structured and ready for visualization.

### 3. Visualizations

Visualization is one of the key features of Power BI, allowing users to present data insights in an engaging and comprehensible way. Several types of visualizations were used in this project to represent different aspects of the insurance data:

#### Table View & Data Profiling

The first visualization technique was to display the raw data in a Table View. This helped in the initial understanding of the dataset, where users could view all individual data points in tabular format. Data profiling was done to identify data quality issues such as missing or incorrect values, ensuring the data is clean and consistent before further analysis.

#### Adding Slicers & Text

Slicers were added to the report to allow users to dynamically filter the data based on certain parameters, such as policy type , claim
number and customerid.These interactive filters make it easy for users to segment and explore different subsets of the data. Text visuals were also included to provide context and explanations of each visualization, making the report more user-friendly and informative.

#### Adding Card Visuals

Card visuals were utilized to display key metrics, such as, number of Male, and Females. These simple yet effective visualizations help in summarizing large volumes of data into easy-to-understand numbers. Card visuals allow users to quickly grasp the most important metrics at a glance.

#### Adding Donut Chart & Matrix Visual

The Donut Chart was used to display categorical data, such as the Active and Inactive policies .This chart type provides a clear representation of proportions. The Matrix Visual, on the other hand, was used for displaying multi-dimensional data, where rows and columns represent different categories, and the intersections display aggregated values. This was helpful for analyzing relationships between different factors.

#### Adding Multi Row Card & Ribbon Chart

The Multi Row Card displayed several key metrics in a compact layout, allowing users to see multiple data points at once. The Ribbon Chart was employed to display trends over time, showing the number of claims by status or claims have changed over the course of several periods. This visual is particularly useful for identifying patterns and seasonality.

#### Adding Bar & Line Chart

Bar and Line Charts were added to further analyze data trends over time or across categories. The Bar Chart helped to compare values across different categories, such as travel,health,auto,life,home. while the Line Chart allowed for tracking changes in key metrics like claims amount by age group. Both visualizations are essential for understanding trends and identifying potential opportunities or issues.

### 4. Create Power BI Account

To share and collaborate on the report, a Power BI account was created. The Power BI service allows for report sharing, collaboration, and remote access to reports. By creating an account, the project became accessible to other users, enabling stakeholders to view the insights and interact with the data remotely.

### 5. Publishing the Report to Power BI Service

After creating the visualizations in Power BI Desktop, the next step was to publish the report to Power BI Service. This cloud-based service allows users to share reports with others, access reports on any device, and schedule automatic data refreshes. Publishing the report to Power BI Service made it accessible to stakeholders and provided a platform for collaboration.

### 6. Creating a Workspace

A workspace was created in Power BI Service to organize the reports, datasets, and dashboards related to this project. A workspace acts as a container where all project files can be stored, and permissions can be managed. In this workspace, team members can collaborate, view reports, and track changes in a centralized location.

![Alt text](https://github.com/Ishtiyaq-Marzuq/powerbi-insurance-sentiment-deployment/blob/main/Deployment.png)


### 7. Scheduling Data Refresh

To ensure the reports always reflect the most up-to-date data, scheduling data refreshes was essential. This feature allows reports to automatically pull the latest data from the source, ensuring accuracy and reducing the need for manual updates. Scheduling refreshes helps maintain data integrity and ensures that stakeholders always see the latest available information.

![Alt text](https://github.com/Ishtiyaq-Marzuq/powerbi-insurance-sentiment-deployment/blob/b99aef4fe406ec371c07744912b3cf529cbc6855/Schedule%20Refresh.png)

### 8. Drill Through Filters

Drill Through Filters were implemented to allow users to right-click on a specific data point and navigate to a detailed report. This feature enables a deeper analysis of specific subsets of data, making it easier to explore the information in greater detail. For example, users could drill through to see detailed claim information by selecting a particular policy type or claim status.

### 9. Testing Scheduled Refresh & Updating Report

After configuring the scheduled refresh, it was crucial to test the functionality to ensure that the reports were being updated correctly. The scheduled refresh was tested by monitoring the report updates at regular intervals and verifying that the data matched the latest available information. Additionally, any changes made to the report were validated to confirm that updates appeared as expected.


### 10. Creating & Testing Roles in Power BI Desktop

Roles were created in Power BI Desktop to define user access levels for the report. This step ensures that different users have appropriate access to different parts of the data based on their role in the organization. Testing the roles helped confirm that users with different permissions could only access the data they were authorized to view.

![Alt text](https://github.com/Ishtiyaq-Marzuq/powerbi-insurance-sentiment-deployment/blob/665b1c4c53992831200b05d9f4c0c144fb593f2c/Creating%20and%20Testing%20Roles.png)

### 11. Implementing Row-Level Security (RLS)

Row-Level Security (RLS) was implemented to restrict access to data at the row level. This security feature ensures that users only see the data relevant to them, based on predefined rules. For example, an insurance agent might only see the policies related to their region or department. RLS is crucial for protecting sensitive data and maintaining privacy within the report.

![Alt text](https://github.com/Ishtiyaq-Marzuq/powerbi-insurance-sentiment-deployment/blob/be197a5fc114277761631d3aa6ccdc40fb7c8779/Row%20Level%20Security.png)

### 12. Sentiment Analysis in Power Query

Sentiment analysis was performed using Power Query to analyze customer feedback or policyholder comments. By extracting sentiment from text fields such as claims descriptions, we were able to classify them as positive, negative, or neutral. This added an extra layer of analysis, allowing stakeholders to understand the emotional tone of feedback and better respond to customer needs.

### 13. Deployment into Workspace

Finally, after testing and refining the report, it was deployed into the Power BI workspace. This deployment made the report accessible to authorized users and ensured that the report was ready for production use. By deploying the report, it became part of the organization's shared knowledge base, enabling easy access to key insights for decision-making.

---

### Conclusion
This project showcases how Power BI can be used to perform detailed insurance data analysis,sentiment analysis  and create visually appealing reports.
