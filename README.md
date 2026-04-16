# IBM-Data-Analyst-Capstone-Project-
IBM Data Analyst Capstone Project contains the step by step process of Data Collection, Wrangling, Manipulation and visualisation. Thereby bringing out key insights  from the Data. This wor was done by Bulus Umoru


<p align="center">
    <img src="https://howtolearnmachinelearning.com/wp-content/uploads/2021/04/coursera_machine_learning_ibm.png?raw=true" alt="IBM and Coursera Logos" width="926" height="133"/>
</p>

# Project Overview

For this project, I will assume the role of an Associate Data Analyst at a technology consulting organization. My primary task is to analyze the data and obtain valuable insights into current and future technological trends using the latest Stack Overflow Developer Survey dataset. 

In this project, I will analyze data to answer key questions about the use of technology. I will analyze trends in programming languages, databases, platforms, and frameworks, focusing on those technologies professionals currently use and those they aim to learn in the future. Through careful analysis, I will extract insights highlighting emerging patterns and shifts in the tech landscape. These findings will then be presented to various stakeholders in my organization for informed decision-making.

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

Our first task is to collect data for the technology skills that are most in demand from various sources including job postings, blog posts, and surveys. We will begin by scraping internet websites and accessing APIs to collect data in various formats like .csv files, excel sheets, and databases. it consist of the following;

- [x] Collecting Data Using APIs
- [x] Collecting Data Using Web Scraping
- [x] Exploring Data

### Task 2: Data Wrangling

Once we've collected enough data we will take the collected data and prepare it for analysis by using data wrangling techniques like finding duplicates, removing duplicates, finding missing values, and inputting missing values. It consist of the following;

- [x] Finding Missing Values
- [x] Determine Missing Values
- [x] Finding Duplicates
- [x] Removing Duplicates
- [x] Normalizing Data

### Task 3: Exploratory Data Analysis

Now that the data is ready we will apply statistical techniques to analyze the data and identify insights and trends like: What are the top programming languages that are in demand? What are the top database skills that are in demand? What are the most popular IDEs? And Demographic data like gender and age distribution of developers. the following was handled in Tas 3;

- [x] Distribution
- [x] Outliers
- [x] Correlation

### Task 4: Data Visualization

In the fourth task, we'll focus on choosing appropriate visualizations based on the data we want to present using charts, plots, and histograms to help reveal our findings and trends. We are going to access the Data from an SQL database and pull only the data we need into DataFrames. The following was achieved;

- [x] Visualizing Distribution of Data
- [x] Relationship
- [x] Composition
- [x] Comparison


## Stretch Goals

- [ ] Create Dashboard in Google Looker or Tableau

### Task 5: Dashboard Creation

For task 5, we will employ Cognos/Google Looker Studio to create interactive dashboards to help analyze and present the data dynamically.

- [x] Dashboards
   ![Click here to view the Insights and  Visualisation (IBM Cognos-Analytics)](https://github.com/umorubulus/IBM-Data-Analyst-Capstone-Project-/blob/f592fd13b660466be629b51d16b52d47b4bf6ff4/Capstone%20Project%20Dashboard-Bulus_Umoru.pdf)

![Python Data Visualization](https://github.com/umorubulus/IBM-Data-Analyst-Capstone-Project-/blob/69db49d4fa85da08632aae69913b5df776a24c01/5.%20Data%20Visualization.ipynb)


### Task 6: Presentation of Findings

For the final task, we will use our storytelling skills to provide a narrative and present the findings of our analysis.

- [x] Final Presentation
   
   ![Click here to view the Report](https://github.com/umorubulus/IBM-Data-Analyst-Capstone-Project-/blob/b4f5a110346c87dc3ec771bdab08b66ab4274750/Data%20Analyst%20Capstone%20Project%20Report-Bulus_Umoru.pdf)

In this step, we focus on data visualization using data extracted from an RDBMS via SQL queries. The key objectives include:
- Understanding data distribution to identify patterns and outliers.
- Exploring relationships between features through visual analysis.
- Comparing and composing data using charts and graphs for better insights.

### Findings
- PostgreSQL is becoming the most popular database, while SQLite is growing for smaller applications.
- C# and SQL are in high demand, while JavaScript is still popular but slightly less preferred.
- Cloud services are expanding beyond AWS, with Google Cloud and Digital Ocean gaining users.
- React, Spring Boot, and FastAPI are the top web frameworks, with FastAPI becoming more popular for Python-based APIs.

### Key Takeaways
- SQL and PostgreSQL are must-have skills for database professionals.
- C# is a valuable skill for developers, especially in enterprise and gaming.
- Diversify beyond JavaScript and explore backend frameworks like FastAPI.
- Multi-cloud expertise is crucial, not just AWS.
- FastAPI is the future of Python APIs, making it an essential skill for backend engineers.

