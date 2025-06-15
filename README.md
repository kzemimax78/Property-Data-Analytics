# Property-Data-Analytics
Property Data Analytics and Visualization Tool
##################################################################################################################################################################################
Software Requirements Specification (SRS)
1. Introduction
This document specifies the requirements for a web-based data analytics and visualization tool that enables property owners to upload CSV files containing property data. The application processes the data, performs financial calculations, and presents visual insights for better decision-making.
1.1 Project Scope
The purpose of this project is to enable property owners to upload data in a predefined CSV format, which allows them to analyze and visualize this data. The application calculates key financial metrics such as monthly expenses and net income, helping users assess return on investment on a monthly basis.
2. Overall Description

2.1 Product Perspective
This application accepts property data including property name, price, monthly EMI, taxes, other expenses, and rental income. It uses this data to calculate expenses and income.
2.2 User Classes and Characteristics
•	Upload CSV data.
•	View total monthly expense per property.
•	View net monthly income per property.
•	View aggregate financials for all properties.
•	Visualize income and expense via charts (bar and pie).
•	Compare individual property performance.
3. Functional Requirements

3.1 CSV Upload and Validation
The system shall allow users to upload a CSV file in a specified format. It will validate the file structure and contents.
3.2 Calculations
•	Monthly Expenses = EMI + Taxes + Other Expenses
•	Net Income = Monthly Rent - Monthly Expenses
•	Aggregates across all properties
3.3 Aggregated Reporting
Users can view the total values for property price, rent, EMI, taxes, other expenses, monthly expense, and monthly income.
3.4 Data Visualization
•	Bar Chart: Net Monthly Income per property
•	Bar Chart: Total Monthly Expense per property
•	Stacked/Grouped Bar Chart: Expense breakdown per property
•	Pie Chart: Income distribution across properties
4. Technical Requirements

4.1 Frontend
•	Technologies: HTML5, Tailwind CSS, Chart.js
•	Features: Form for file upload, dynamic charts, responsive layout
4.2 Backend
•	Technologies: Django (Python), SQLite
•	Responsibilities: Handle file upload, data parsing, calculations, and render views
4.3 Business Logic
•	Implements core financial computations and data aggregation:
•	Expenses = EMI + Taxes + Other Expenses
•	Net Income = Rental Income - Expenses
•	ROI = (Net Income / Property Price) * 100
4.4 Visualizations
Chart.js will be used to render bar charts and pie charts as per calculated data.
4.5 Development & Deployment
•	Tools: VSCode, Git/GitHub, Docker (optional), Postman
•	Hosting: Localhost, Heroku, Railway, or any Python-compatible VPS
