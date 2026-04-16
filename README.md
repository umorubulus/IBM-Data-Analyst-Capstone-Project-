# IBM-Data-Analyst-Capstone-Project-
IBM Data Analyst Capstone Project contains the step by step process of Data Collection, Wrangling, Manipulation and visualisation. Thereby bringing out key insights  from the Data. 


<p align="center">
    <img src="https://howtolearnmachinelearning.com/wp-content/uploads/2021/04/coursera_machine_learning_ibm.png?raw=true" alt="IBM and Coursera Logos" width="926" height="133"/>
</p>

# Project Overview

For this project, I will assume the role of an Associate Data Analyst at a technology consulting organization. My primary task is to analyze the data and obtain valuable insights into current and future technological trends using the latest Stack Overflow Developer Survey dataset. 

In this project, I will analyze data to answer key questions about the use of technology. I will analyze trends in programming languages, databases, platforms, and frameworks, focusing on those technologies professionals currently use and those they aim to learn in the future. Through careful analysis, I will extract insights highlighting emerging patterns and shifts in the tech landscape. These findings will then be presented to various stakeholders in my organization for informed decision-making.

### Task 1

Our first task is to collect data for the technology skills that are most in demand from various sources including job postings, blog posts, and surveys. We will begin by scraping internet websites and accessing APIs to collect data in various formats like .csv files, excel sheets, and databases.

### Task 2

Once we've collected enough data we will take the collected data and prepare it for analysis by using data wrangling techniques like finding duplicates, removing duplicates, finding missing values, and inputting missing values.

### Task 3

Now that the data is ready we will apply statistical techniques to analyze the data and identify insights and trends like: What are the top programming languages that are in demand? What are the top database skills that are in demand? What are the most popular IDEs? And Demographic data like gender and age distribution of developers.

### Task 4

In the fourth task, we'll focus on choosing appropriate visualizations based on the data we want to present using charts, plots, and histograms to help reveal our findings and trends. We are going to access the Data from an SQL database and pull only the data we need into DataFrames.

### Task 5

For task 5, we will employ Cognos/Google Looker Studio to create interactive dashboards to help analyze and present the data dynamically.

### Task 6

For the final task, we will use our storytelling skills to provide a narrative and present the findings of our analysis.
Full presentation link: https://www.canva.com/design/DAGCO32O1hs/i6ag-UXsZqQ8_E5A-mI9bA/edit?utm_content=DAGCO32O1hs&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

## Table of Contents

- [Data Description](#data-description)
- [Tools](#tools)
- [Deliverables](#deliverables)
  - [Task 1: Data Collection](#task-1-data-collection)
  - [Task 2: Data Wrangling](#task-2-data-wrangling)
  - [Task 3: Exploratory Data Analysis](#task-3-exploratory-data-analysis)
  - [Task 4: Data Visualization](#task-4-data-visualization)
  - [Task 5: Dashboard Creation](#task-5-dashboard-creation)
  - [Task 6: Presentation of Findings](#task-6-presentation-of-findings)
- [Stretch Goals](#stretch-goals)

## Data Description

The dataset used for this analysis is the 2019 Stack Overflow Developer Survey, covering everything from developers’ favorite technologies to their job preferences.

[Click here to download the dataset](https://stackoverflow.blog/2024/08/06/2024-developer-survey/) under a ODbL: Open Database License.   

Note: This randomised subset contains around 1/10th of the original data set. Any conclusions we draw after analyzing this subset may not reflect the real world scenario.

The dataset is available as a .csv file.
## Tools

- [`python`](https://www.python.org/downloads/) v3.12.2
- [`pandas`](https://pandas.pydata.org/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for managing the data.
- [`numpy`](https://numpy.org/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for mathematical operations.
- [`seaborn`](https://seaborn.pydata.org/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for visualizing the data.
- [`matplotlib`](https://matplotlib.org/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkCoursesIBMML0187ENSkillsNetwork31430127-2021-01-01) for additional plotting tools.
- [`folium`](https://python-visualization.github.io/folium/latest/) for geospatial data visualization such as choropleth maps.
- [`plotly`](https://plotly.com/python/) for interactive plotting tools.
- [`Google Looker Studio`](https://lookerstudio.google.com/overview) for dashboards.
- [`IBM Cognos Analytics`](https://www.ibm.com/products/cognos-analytics) for dashboards.

## Deliverables

### Task 1: Data Collection

- [x] Collecting Data Using APIs
- [x] Collecting Data Using Web Scraping
- [x] Exploring Data

### Task 2: Data Wrangling

- [x] Finding Missing Values
- [x] Determine Missing Values
- [x] Finding Duplicates
- [x] Removing Duplicates
- [x] Normalizing Data

### Task 3: Exploratory Data Analysis

- [x] Distribution
- [x] Outliers
- [x] Correlation

### Task 4: Data Visualization

- [x] Visualizing Distribution of Data
- [x] Relationship
- [x] Composition
- [x] Comparison

### Task 5: Dashboard Creation

- [x] Dashboards

### Task 6: Presentation of Findings

- [x] Final Presentation

## Stretch Goals

- [ ] Create Dashboard in Google Looker or Tableau

### [Data Visualization](https://github.com/LinoyOkev/IBM_Data_Analyst_Capstone_Project/blob/main/6.Data%20Visualization.ipynb)

In this step, we focus on data visualization using data extracted from an RDBMS via SQL queries. The key objectives include:
- Understanding data distribution to identify patterns and outliers.
- Exploring relationships between features through visual analysis.
- Comparing and composing data using charts and graphs for better insights.

### Findings
- PostgreSQL is becoming the most popular database, while SQLite is growing for smaller applications.
- C# and SQL are in high demand, while JavaScript is still popular but slightly less preferred.
- Cloud services are expanding beyond AWS, with Google Cloud and Digital Ocean gaining users.
- React, Spring Boot, and FastAPI are the top web frameworks, with FastAPI becoming more popular for Python-based APIs.

#### Current Technology Usage
![6][Tab 1 _current Technology in use.png](https://github.com/umorubulus/IBM-Data-Analyst-Capstone-Project-/blob/main/Tab%201%20_current%20Technology%20in%20use.png)
#### Future Technology Trend
![7](https://github.com/user-attachments/assets/98868617-b1d0-4f1b-b816-a7dac4951ac7)

#### Demographics
![8](https://github.com/user-attachments/assets/4c461948-3190-4d24-95a9-5f8c0d356e72)

### Key Takeaways
- SQL and PostgreSQL are must-have skills for database professionals.
- C# is a valuable skill for developers, especially in enterprise and gaming.
- Diversify beyond JavaScript and explore backend frameworks like FastAPI.
- Multi-cloud expertise is crucial, not just AWS.
- FastAPI is the future of Python APIs, making it an essential skill for backend engineers.

