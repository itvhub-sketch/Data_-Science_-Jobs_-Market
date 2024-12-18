# Data_Science_Jobs_Market
Data Analysis of 700 hundred Postings from Indeed.com with the search term "Data Science"

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

### Results






