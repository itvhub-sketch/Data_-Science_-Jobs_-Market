# Data_Science_Jobs_Market
Data Analysis of 700 hundred Postings from Indeed.com with the search term "Data Science"

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources(#data-sources)
- [Tools](#Tools)
- [Data Cleaning](#Data-Cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results Findings](#results-findings)
- [Recommendations](#Recommendations)
- [Limitations](#Limitations)
- [References](#References)
  



### Project Overview 

This dataset has beeen uploaded to kaggle by ShaShan Lu. There are nearley 7000 job postings from Indeed.com with the search term of "Data Science". Insights from analyzing the data will be beneficial to me, to identify trends, make data-driven recommendations and to gain a deeper understanding of the dataset.

## Data Sources

The dataset used for this analysis is the JobMarket_EDA.csv file, uploaded to kaggle by shashan Lu, containing information from job listings on Indeed.com with the search term "Data Science".

### Tools

- Phython Pandas in juypter Notebook - Data Cleaning
- Phython Pandas in juypter Notebook - for data Analysis
- Tableau - Creating a reports

### Data Cleaning and Preparation

In the data preparation phase I performed the following tasks.
1. Data loading and inspection.
2. handling missing values.
3. data claaning and formatting.

### Exploratory Data Analysis

EDA involves exploring the sales data to answer key questions, such as:

- What are the most common job titles?
- Which companies have posted the most job listings?
- How many job listings are there for each unique location?
- What is the distribution of reviews for the job listings?

### Data Analysis


```python
company_counts = data_df['company'].value_counts()

plt.figure(figsize=(10, 6))
sns.barplot(y=company_counts.index[:10], x=company_counts.values[:10], palette="magma")
plt.title('Top Companies by Number of Listings', fontsize=14)
plt.xlabel('Number of Listings')
plt.ylabel('Company')
plt.show()
```
This plot will display the companies that have posted the most job listings.

### Results/Findings

 The data analysis reveals that A few companies dominate the listings, reflecting either regional or organizational hiring trends. While most job postings lack reviews, those with reviews exhibit significant variability, with some standout roles receiving a disproportionately high number of reviews. The job descriptions emphasize skills in data analysis, teamwork, and technical expertise, aligning with the growing demand for data professionals. Overall, the dataset highlights a concentrated market for technical and analytical talent in a specific geographic area.

 ### Recommendations

 To improve the dynamics reflected in the dataset, companies should diversify job opportunities beyond Atlanta, encourage more candidate reviews for transparency, and promote lesser-known organizations to attract diverse talent. Offering training in data-related fields can address skill gaps, while standardizing job descriptions enhances clarity. Remote work opportunities can reduce geographic concentration, and fostering a balanced focus on roles beyond data-related jobs can create a more inclusive market. Addressing review disparities and improving company culture will further attract and retain talent effectively.

 ### Limitations

 The dataset was focused on key columns such as "position," "company," "description," "reviews," and "location." Incomplete or inconsistent entries, like job descriptions with newline characters or truncated sentences, were retained in their original form. Missing values, particularly in the "reviews" column, were preserved to allow for differentiation between listings with and without reviews. No new columns or external data were added, but the reconstructed dataset is limited compared to the potential scope of the original file.

 ### References

 1. Ecommerce Analytics by Judah Phillips (Author)

 

 

 






