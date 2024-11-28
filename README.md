# Power BI Insurance Sentiment Analysis and Deployment Framework
A Power BI project for insurance data analysis featuring advanced visualizations, sentiment analysis, role-based security (RLS), and seamless deployment for insightful decision-making and reporting.

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
3. [Conclusion](#conclusion)

---

## Introduction

This project focuses on analyzing insurance data using Power BI, a powerful business analytics tool that helps users visualize and analyze data interactively. The goal was to use various Power BI features to transform raw data into meaningful insights, which could help insurance companies make informed decisions. The analysis includes different types of visualizations, dynamic filtering, and real-time data refresh, along with implementing sentiment analysis on customer feedback. The project aims to provide a comprehensive understanding of insurance trends, key metrics, and customer sentiments that drive decision-making processes.

---

## Project Steps

### 1. Importing Data to MSSQL Server

The initial phase of the project involved importing the insurance data into Microsoft SQL Server, which is a reliable and secure relational database management system. This step ensures that all the raw data is stored in an organized manner, allowing for efficient querying, data retrieval, and further analysis. The data is typically structured in tables, where each table holds a different type of information related to policies, claims, premiums, and customers. Importing data into MSSQL Server provides the necessary foundation for building a robust data analysis pipeline, and it enables the integration of Power BI to fetch data seamlessly.

### 2. Loading Data to Power BI Desktop

Once the data was successfully imported into the MSSQL Server, the next step was to load the data into Power BI Desktop. Power BI Desktop is a powerful tool for data transformation, visualization, and report creation. By connecting to the MSSQL Server through Power BI, the dataset was pulled into Power BI's environment, where data can be cleaned, transformed, and modeled to suit analytical needs. This step involved defining relationships between tables, transforming columns (e.g., creating new calculated fields or cleaning invalid data), and preparing the dataset for visualization. 

### 3. Visualizations

#### Table View & Data Profiling

The first step in visualizing the data was to display it in a simple Table View to get an overview of the dataset. Data profiling was done to assess the quality of the data, check for missing values, inconsistencies, or outliers, and ensure that the data is ready for analysis. This process involves examining each field of the dataset to understand its structure and determine any required data transformations or cleaning before deeper analysis can take place.

#### Adding Slicers & Text

To enhance the interactivity of the report, slicers were added to the dashboard. Slicers are interactive filters that allow users to slice the data based on different parameters like policy type, customer location, or claim status. This empowers users to drill down into the data and explore different subsets of information dynamically. Additionally, text boxes were added to the report for labels and descriptions, helping to guide users through the dashboard and explain what each visualization represents, thereby improving the overall user experience.

#### Adding Card Visuals

Card visuals were used to display key metrics such as total policies, claims, premiums, and customer counts. These visuals help to highlight important KPIs (Key Performance Indicators) that provide a quick overview of the business's performance. By using card visuals, decision-makers can easily track significant numbers and assess the health of the business at a glance. This visual format is concise and focused, offering insight into metrics that directly influence strategic decisions.

#### Adding Donut Chart & Matrix Visual

A Donut Chart was utilized to visually represent the distribution of different insurance categories, such as claims by type or premiums by policy. This chart provides a simple, intuitive view of how various parts of the business contribute to the whole. The Matrix Visual, on the other hand, was used for multi-dimensional analysis, showing data in a tabular form but allowing for hierarchies and drill-downs, making it easier to compare and analyze the data across different categories such as policy type, region, or age group.

#### Adding Multi Row Card & Ribbon Chart

The Multi Row Card was added to display multiple pieces of information in a compact format. This is particularly useful for showcasing a list of related metrics for a specific dimension, such as a customer or policy. A Ribbon Chart was introduced to visualize trends over time, such as premium growth or claims frequency. The Ribbon Chart provides a clear view of how metrics change across periods, which is useful for identifying patterns and understanding the dynamics of insurance business operations.

#### Adding Bar & Line Chart

Bar and Line Charts were used to track numerical trends over time or across various categories. Bar Charts are excellent for comparing different categories side by side, such as the number of claims by region or the total premiums by insurance type. Line Charts, on the other hand, were used to visualize changes in data over time, such as how claims frequency or revenue has evolved over the past years, helping stakeholders to identify trends and predict future outcomes.

### 4. Create Power BI Account

A Power BI account was created to facilitate collaboration and sharing of the reports. Power BI accounts are essential for using Power BI Service, which is the cloud-based version of Power BI that enables users to access reports from any device and share them with stakeholders. By creating an account, the project was set up to be shared with authorized users and collaborators, ensuring everyone involved can access the analysis and contribute to decision-making.

### 5. Publishing the Report to Power BI Service

After the analysis was complete and the visuals were ready, the final step was to publish the report from Power BI Desktop to Power BI Service. Publishing makes the report accessible to other users via a web browser or mobile device. The report is hosted on the Power BI cloud platform, where it can be shared with team members, clients, or stakeholders, allowing for real-time collaboration and discussions around the insights presented in the report.

### 6. Creating a Workspace

In Power BI Service, a workspace was created to organize and manage the reports and datasets. Workspaces serve as containers that group together related reports, dashboards, and datasets. This allows for better organization and control over who has access to the data. By creating a workspace, you can assign specific roles and permissions to different users, ensuring that sensitive information is only accessible by authorized personnel.

### 7. Scheduling Data Refresh

To ensure that the data remains up-to-date, a data refresh schedule was set up in Power BI Service. This feature automatically refreshes the dataset at predefined intervals, such as daily or weekly. Scheduled refresh ensures that the report always reflects the latest data without manual intervention, keeping decision-makers informed with real-time or near-real-time insights.

### 8. Drill Through Filters

Drill Through Filters were added to allow users to click on specific data points within the report and navigate to a more detailed analysis of that particular data. For example, a user can click on a region in a map and view more detailed metrics, such as claims frequency, premium revenue, and customer demographics specific to that region. This feature enhances the report’s interactivity and allows users to explore the data in-depth without leaving the report.

### 9. Testing Scheduled Refresh & Updating Report

After setting up the data refresh, the process was tested to ensure that the reports were updating as
