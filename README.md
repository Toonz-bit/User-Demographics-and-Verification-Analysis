# User-Demographics-and-Verification-Analysis

### Table Of Content

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning / Preparation](#datacleaning/preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results / Findings](#results/findings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)

### Project Overview

![Screenshot 2024-10-13 163122](https://github.com/user-attachments/assets/d269527c-8e6e-4c14-8910-7fc689093ab7)

Designed to provide insights into user profiles and their verification status. It focuses on analyzing key user attributes such as gender, age, occupation, KYC verification, deactivation status, and residency across different countries.

### Data Sources

The data source used is an Excel CSV file containing key metrics and attributes for analysis, with MySQL database hosted on an SQL server at localhost:3306, designed to provide dynamic data for analysis and reporting, potentially integrated with Power BI or other BI tools.

### Tools

Excel - Data Cleaning
SQL Server - Data Analysis
Power Bi - Data Visualization

### Data Cleaning/Preparation

In the initial data preparation phase, we performed the following task

- Handling Missing Values
- Standardizing Formats
- Removing Duplicates
- Validating Age Data
- KYC Verification Consistency
- Categorizing Occupations and Countries

  ### Exploratory Data Analysis

  - Calculate the total users, total verified users, total non verified userS and Active users

    ![Screenshot 2024-10-30 110811](https://github.com/user-attachments/assets/6f0b719e-4233-42ed-8d9f-a0da362c02e4)

  - Users by KYC Status

  ![Screenshot 2024-10-30 110942](https://github.com/user-attachments/assets/ba436026-3ce9-42e6-9269-adab1caf03b8)
    
- User By Resident Country

  ![Screenshot 2024-10-30 110949](https://github.com/user-attachments/assets/b968ef00-0bdf-4ad6-ac3f-4f93937623d1)

  - Users by Gender
 
    ![Screenshot 2024-10-30 110822](https://github.com/user-attachments/assets/d623fd8c-416d-4225-b82e-909fe2c32788)

 
### Data Analysis

Include some interesting code/ features worked with
Measure: 
- Total Users = COUNT(Users[UserID])
- Verified Users = CALCULATE(COUNT(Users[UserID]), Users[VerificationStatus] = "Verified")
- Non-Verified Users = CALCULATE(COUNT(Users[UserID]), Users[VerificationStatus] = "Non-Verified")
- Active Users = CALCULATE(COUNT(Users[UserID]), Users[DeactivationStatus] = "Active")

### Results/Findings

Total Users shows the overall user count in the system.
Verified Users indicates the number of users who have completed verification.
Non-Verified Users reveals how many users are unverified.
Active Users shows the number of users currently active and not deactivated.
The metrics helps understand user engagement, verification progress, and overall platform activity.

### Recommendation

Base on the analysis, we recommend the following actions:

- Increase Verification Rates: Consider targeted outreach or incentives to encourage non-verified users to complete verification, which may improve trust and compliance.

- Enhance User Engagement: Use insights from active and inactive user counts to develop re-engagement strategies for inactive users, such as personalized notifications or feature highlights.

- Monitor User Growth: Track the trend of total users over time to assess growth, and consider marketing efforts or referral programs if user acquisition needs a boost.

### Limitations

 The measure for Active Users only identifies if users are deactivated but doesn’t track recent activity or engagement frequency. Further analysis is needed to gauge true activity levels.

 Verified Users only counts those marked as verified but doesn’t ensure that the verification is thorough or up-to-date, which may lead to gaps in security or compliance.

 ### References

 User Engagement and Retention Metrics: Resources like Mixpanel and Amplitude offer insights into user engagement, verification processes, and best practices for onboarding and retention analysis. Mixpanel User Engagement Guide and Amplitude Blog.

 🙂
 💰

 |Heading1|Heading2|
 |--------|--------|
 |Content|Content2|
 |SQL|PowerBi|

 
