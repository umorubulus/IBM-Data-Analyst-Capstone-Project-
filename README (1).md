<p align="center">
    <img src="https://howtolearnmachinelearning.com/wp-content/uploads/2021/04/coursera_machine_learning_ibm.png?raw=true" alt="IBM and Coursera Logos" width="926" height="133"/>
</p>

# Data Visualization with Python

This is the Capstone Project for Course 9, _IBM Data Analyst Capstone Project_. Part of IBM's Data Analyst Professional Certificate from Coursera. Available here: https://www.coursera.org/programs/jda20232t1-z1hse/professional-certificates/ibm-data-analyst?collectionId=Wxyxq

We will take on the role of a Data Analyst with a global IT and Business services firm. In this role, we will be analyzing several datasets to help identify trends for emerging technologies. We have recently been hired as a Data Analyst by a global IT and business consulting services firm that is known for its expertise in IT solutions and its team of highly experienced IT consultants. To keep pace with changing technologies and remain competitive, our organization regularly analyzes data to help identify future skill requirements.

As a Data Analyst, we will be assisting with this initiative and have been tasked with collecting data from various sources and identifying trends for this year's report on emerging skills.

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

Stack Overflow, a popular website for developers, conducted an online survey of software professionals across the world. The survey data was later open sourced by Stack Overflow. The actual data set has around 90,000 responses.

The dataset we are going to use comes from the following source: https://stackoverflow.blog/2019/04/09/the-2019-stack-overflow-developer-survey-results-are-in/ under a ODbL: Open Database License.

We will be given a subset of the original data set in this capstone project. We will explore, analyze, and visualize this dataset and present our analysis.

Note: This randomised subset contains around 1/10th of the original data set. Any conclusions we draw after analyzing this subset may not reflect the real world scenario.

The dataset is available as a .csv file here.

The below table lists the questions asked in the survey and the column under which the response was collected.

<details>
 <summary><strong>View Table</strong></summary>
<table>
  <thead>
    <tr>
      <th>Column Name</th>
      <th>Question Text</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Respondent</td>
      <td>
        Randomized respondent ID number (not in order of survey response time)
      </td>
    </tr>
    <tr>
      <td>MainBranch</td>
      <td>
        Which of the following options best describes you today? Here, by
        “developer” we mean “someone who writes code.”
      </td>
    </tr>
    <tr>
      <td>Hobbyist</td>
      <td>Do you code as a hobby?</td>
    </tr>
    <tr>
      <td>OpenSourcer</td>
      <td>How often do you contribute to open source?</td>
    </tr>
    <tr>
      <td>OpenSource</td>
      <td>How do you feel about the quality of open source software (OSS)?</td>
    </tr>
    <tr>
      <td>Employment</td>
      <td>
        Which of the following best describes your current employment status?
      </td>
    </tr>
    <tr>
      <td>Country</td>
      <td>In which country do you currently reside?</td>
    </tr>
    <tr>
      <td>Student</td>
      <td>
        Are you currently enrolled in a formal, degree-granting college or
        university program?
      </td>
    </tr>
    <tr>
      <td>EdLevel</td>
      <td>
        Which of the following best describes the highest level of formal
        education that you’ve completed?
      </td>
    </tr>
    <tr>
      <td>UndergradMajor</td>
      <td>What was your main or most important field of study?</td>
    </tr>
    <tr>
      <td>EduOther</td>
      <td>
        Which of the following types of non-degree education have you used or
        participated in? Please select all that apply.
      </td>
    </tr>
    <tr>
      <td>OrgSize</td>
      <td>
        Approximately how many people are employed by the company or
        organization you work for?
      </td>
    </tr>
    <tr>
      <td>DevType</td>
      <td>
        Which of the following describe you? Please select all that apply.
      </td>
    </tr>
    <tr>
      <td>YearsCode</td>
      <td>Including any education, how many years have you been coding?</td>
    </tr>
    <tr>
      <td>Age1stCode</td>
      <td>
        At what age did you write your first line of code or program? (E.g.,
        webpage, Hello World, Scratch project)
      </td>
    </tr>
    <tr>
      <td>YearsCodePro</td>
      <td>
        How many years have you coded professionally (as a part of your work)?
      </td>
    </tr>
    <tr>
      <td>CareerSat</td>
      <td>Overall, how satisfied are you with your career thus far?</td>
    </tr>
    <tr>
      <td>JobSat</td>
      <td>
        How satisfied are you with your current job? (If you work multiple jobs,
        answer for the one you spend the most hours on.)
      </td>
    </tr>
    <tr>
      <td>MgrIdiot</td>
      <td>How confident are you that your manager knows what they’re doing?</td>
    </tr>
    <tr>
      <td>MgrMoney</td>
      <td>Do you believe that you need to be a manager to make more money?</td>
    </tr>
    <tr>
      <td>MgrWant</td>
      <td>Do you want to become a manager yourself in the future?</td>
    </tr>
    <tr>
      <td>JobSeek</td>
      <td>
        Which of the following best describes your current job-seeking status?
      </td>
    </tr>
    <tr>
      <td>LastHireDate</td>
      <td>When was the last time that you took a job with a new employer?</td>
    </tr>
    <tr>
      <td>LastInt</td>
      <td>
        In your most recent successful job interview (resulting in a job offer),
        you were asked to… (check all that apply)
      </td>
    </tr>
    <tr>
      <td>FizzBuzz</td>
      <td>Have you ever been asked to solve FizzBuzz in an interview?</td>
    </tr>
    <tr>
      <td>JobFactors</td>
      <td>
        Imagine that you are deciding between two job offers with the same
        compensation, benefits, and location. Of the following factors, which 3
        are MOST important to you?
      </td>
    </tr>
    <tr>
      <td>ResumeUpdate</td>
      <td>
        Think back to the last time you updated your resumé CV, or an online
        profile on a job site. What is the PRIMARY reason that you did so?
      </td>
    </tr>
    <tr>
      <td>CurrencySymbol</td>
      <td>
        Which currency do you use day-to-day? If your answer is complicated,
        please pick the one you’re most comfortable estimating in.
      </td>
    </tr>
    <tr>
      <td>CurrencyDesc</td>
      <td>
        Which currency do you use day-to-day? If your answer is complicated,
        please pick the one you’re most comfortable estimating in.
      </td>
    </tr>
    <tr>
      <td>CompTotal</td>
      <td>
        What is your current total compensation (salary, bonuses, and perks,
        before taxes and deductions), in <code>CurrencySymbol</code>? Please
        enter a whole number in the box below, without any punctuation. If you
        are paid hourly, please estimate an equivalent weekly, monthly, or
        yearly salary. If you prefer not to answer, please leave the box empty.
      </td>
    </tr>
    <tr>
      <td>CompFreq</td>
      <td>Is that compensation weekly, monthly, or yearly?</td>
    </tr>
    <tr>
      <td>ConvertedComp</td>
      <td>
        Salary converted to annual USD salaries using the exchange rate on
        2019-02-01, assuming 12 working months and 50 working weeks.
      </td>
    </tr>
    <tr>
      <td>WorkWeekHrs</td>
      <td>On average, how many hours per week do you work?</td>
    </tr>
    <tr>
      <td>WorkPlan</td>
      <td>How structured or planned is your work?</td>
    </tr>
    <tr>
      <td>WorkChallenge</td>
      <td>
        Of these options, what are your greatest challenges to productivity as a
        developer? Select up to 3:
      </td>
    </tr>
    <tr>
      <td>WorkRemote</td>
      <td>How often do you work remotely?</td>
    </tr>
    <tr>
      <td>WorkLoc</td>
      <td>Where would you prefer to work?</td>
    </tr>
    <tr>
      <td>ImpSyn</td>
      <td>
        For the specific work you do, and the years of experience you have, how
        do you rate your own level of competence?
      </td>
    </tr>
    <tr>
      <td>CodeRev</td>
      <td>Do you review code as part of your work?</td>
    </tr>
    <tr>
      <td>CodeRevHrs</td>
      <td>On average, how many hours per week do you spend on code review?</td>
    </tr>
    <tr>
      <td>UnitTests</td>
      <td>
        Does your company regularly employ unit tests in the development of
        their products?
      </td>
    </tr>
    <tr>
      <td>PurchaseHow</td>
      <td>
        How does your company make decisions about purchasing new technology
        (cloud, AI, IoT, databases)?
      </td>
    </tr>
    <tr>
      <td>PurchaseWhat</td>
      <td>
        What level of influence do you, personally, have over new technology
        purchases at your organization?
      </td>
    </tr>
    <tr>
      <td>LanguageWorkedWith</td>
      <td>
        Which of the following programming, scripting, and markup languages have
        you done extensive development work in over the past year, and which do
        you want to work in over the next year? (If you both worked with the
        language and want to continue to do so, please check both boxes in that
        row.)
      </td>
    </tr>
    <tr>
      <td>LanguageDesireNextYear</td>
      <td>
        Which of the following programming, scripting, and markup languages have
        you done extensive development work in over the past year, and which do
        you want to work in over the next year? (If you both worked with the
        language and want to continue to do so, please check both boxes in that
        row.)
      </td>
    </tr>
    <tr>
      <td>DatabaseWorkedWith</td>
      <td>
        Which of the following database environments have you done extensive
        development work in over the past year, and which do you want to work in
        over the next year? (If you both worked with the database and want to
        continue to do so, please check both boxes in that row.)
      </td>
    </tr>
    <tr>
      <td>DatabaseDesireNextYear</td>
      <td>
        Which of the following database environments have you done extensive
        development work in over the past year, and which do you want to work in
        over the next year? (If you both worked with the database and want to
        continue to do so, please check both boxes in that row.)
      </td>
    </tr>
    <tr>
      <td>PlatformWorkedWith</td>
      <td>
        Which of the following platforms have you done extensive development
        work for over the past year? (If you both developed for the platform and
        want to continue to do so, please check both boxes in that row.)
      </td>
    </tr>
    <tr>
      <td>PlatformDesireNextYear</td>
      <td>
        Which of the following platforms have you done extensive development
        work for over the past year? (If you both developed for the platform and
        want to continue to do so, please check both boxes in that row.)
      </td>
    </tr>
    <tr>
      <td>WebFrameWorkedWith</td>
      <td>
        Which of the following web frameworks have you done extensive
        development work in over the past year, and which do you want to work in
        over the next year? (If you both worked with the framework and want to
        continue to do so, please check both boxes in that row.)
      </td>
    </tr>
    <tr>
      <td>WebFrameDesireNextYear</td>
      <td>
        Which of the following web frameworks have you done extensive
        development work in over the past year, and which do you want to work in
        over the next year? (If you both worked with the framework and want to
        continue to do so, please check both boxes in that row.)
      </td>
    </tr>
    <tr>
      <td>MiscTechWorkedWith</td>
      <td>
        Which of the following other frameworks, libraries, and tools have you
        done extensive development work in over the past year, and which do you
        want to work in over the next year? (If you both worked with the
        technology and want to continue to do so, please check both boxes in
        that row.)
      </td>
    </tr>
    <tr>
      <td>MiscTechDesireNextYear</td>
      <td>
        Which of the following other frameworks, libraries, and tools have you
        done extensive development work in over the past year, and which do you
        want to work in over the next year? (If you both worked with the
        technology and want to continue to do so, please check both boxes in
        that row.)
      </td>
    </tr>
    <tr>
      <td>DevEnviron</td>
      <td>
        Which development environment(s) do you use regularly? Please check all
        that apply.
      </td>
    </tr>
    <tr>
      <td>OpSys</td>
      <td>What is the primary operating system in which you work?</td>
    </tr>
    <tr>
      <td>Containers</td>
      <td>
        How do you use containers (Docker, Open Container Initiative (OCI),
        etc.)?
      </td>
    </tr>
    <tr>
      <td>BlockchainOrg</td>
      <td>
        How is your organization thinking about or implementing blockchain
        technology?
      </td>
    </tr>
    <tr>
      <td>BlockchainIs</td>
      <td>Blockchain / cryptocurrency technology is primarily:</td>
    </tr>
    <tr>
      <td>BetterLife</td>
      <td>
        Do you think people born today will have a better life than their
        parents?
      </td>
    </tr>
    <tr>
      <td>ITperson</td>
      <td>Are you the “IT support person” for your family?</td>
    </tr>
    <tr>
      <td>OffOn</td>
      <td>Have you tried turning it off and on again?</td>
    </tr>
    <tr>
      <td>SocialMedia</td>
      <td>What social media site do you use the most?</td>
    </tr>
    <tr>
      <td>Extraversion</td>
      <td>Do you prefer online chat or IRL conversations?</td>
    </tr>
    <tr>
      <td>ScreenName</td>
      <td>What do you call it?</td>
    </tr>
    <tr>
      <td>SOVisit1st</td>
      <td>
        To the best of your memory, when did you first visit Stack Overflow?
      </td>
    </tr>
    <tr>
      <td>SOVisitFreq</td>
      <td>How frequently would you say you visit Stack Overflow?</td>
    </tr>
    <tr>
      <td>SOVisitTo</td>
      <td>I visit Stack Overflow to… (check all that apply)</td>
    </tr>
    <tr>
      <td>SOFindAnswer</td>
      <td>
        On average, how many times a week do you find (and use) an answer on
        Stack Overflow?
      </td>
    </tr>
    <tr>
      <td>SOTimeSaved</td>
      <td>
        Think back to the last time you solved a coding problem using Stack
        Overflow, as well as the last time you solved a problem using a
        different resource. Which was faster?
      </td>
    </tr>
    <tr>
      <td>SOHowMuchTime</td>
      <td>
        About how much time did you save? If you’re not sure, please use your
        best estimate.
      </td>
    </tr>
    <tr>
      <td>SOAccount</td>
      <td>Do you have a Stack Overflow account?</td>
    </tr>
    <tr>
      <td>SOPartFreq</td>
      <td>
        How frequently would you say you participate in Q&amp;A on Stack
        Overflow? By participate we mean ask, answer, vote for, or comment on
        questions.
      </td>
    </tr>
    <tr>
      <td>SOJobs</td>
      <td>Have you ever used or visited Stack Overflow Jobs?</td>
    </tr>
    <tr>
      <td>EntTeams</td>
      <td>
        Have you ever used Stack Overflow for Enterprise or Stack Overflow for
        Teams?
      </td>
    </tr>
    <tr>
      <td>SOComm</td>
      <td>
        Do you consider yourself a member of the Stack Overflow community?
      </td>
    </tr>
    <tr>
      <td>WelcomeChange</td>
      <td>Compared to last year, how welcome do you feel on Stack Overflow?</td>
    </tr>
    <tr>
      <td>SONewContent</td>
      <td>
        Would you like to see any of the following on Stack Overflow? Check all
        that apply.
      </td>
    </tr>
    <tr>
      <td>Age</td>
      <td>
        What is your age (in years)? If you prefer not to answer, you may leave
        this question blank.
      </td>
    </tr>
    <tr>
      <td>Gender</td>
      <td>
        Which of the following do you currently identify as? Please select all
        that apply. If you prefer not to answer, you may leave this question
        blank.
      </td>
    </tr>
    <tr>
      <td>Trans</td>
      <td>Do you identify as transgender?</td>
    </tr>
    <tr>
      <td>Sexuality</td>
      <td>
        Which of the following do you currently identify as? Please select all
        that apply. If you prefer not to answer, you may leave this question
        blank.
      </td>
    </tr>
    <tr>
      <td>Ethnicity</td>
      <td>
        Which of the following do you identify as? Please check all that apply.
        If you prefer not to answer, you may leave this question blank.
      </td>
    </tr>
    <tr>
      <td>Dependents</td>
      <td>
        Do you have any dependents (e.g., children, elders, or others) that you
        care for?
      </td>
    </tr>
    <tr>
      <td>SurveyLength</td>
      <td>How do you feel about the length of the survey this year?</td>
    </tr>
    <tr>
      <td>SurveyEase</td>
      <td>How easy or difficult was this survey to complete?</td>
    </tr>
  </tbody>
</table>

</details>

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
