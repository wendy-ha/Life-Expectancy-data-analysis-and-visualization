# Analyzing the impact of vaccination on humna lifespans in developed and developing nations
## Introduction
Despite the fact that many research have been conducted in the past on factors impacting life expectancy, including demographic characteristics, income composition, and mortality rates, Max Roser emphasized on Our World In Data that the influence of vaccines has been overlooked (Max et al 2013).
<br/>
<br/>
Share the same concern with Max, two researchers from World Health Organization (WHO) Department of Data and Analytics, Deeksha Russell and Duan Wang, have compiled a collection of statistics on the key drivers of life expectancy, with a focus on immunization variables including Hepatitis B, Measles, Polio, and Diphtheria (Deeksha and Duan 2015). Furthermore, mortality, economy, social issues, and other health- related aspects are all taken into consideration (Deeksha and Duan 2015). As a result, numerous analyses of the impact of vaccination on human lifespans in developed and developing nations have been undertaken using this data set, with the goal of assisting residents in those countries in improving their quality of life.
<br/>
<br/>
- This data collection is a component of the World Health Statistic Report 2015, which can be accessed at: [https://www.who.int/docs/default-source/gho-documents/world- health-statistic-reports/world-health-statistics-2015.pdf](https://www.who.int/docs/default-source/gho-documents/world-health-statistic-reports/world-health-statistics-2015.pdf)
- The Life Expectancy (WHO) dataset used for analysis in this report can be downloaded at: [https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who)
- Notebook with details coding for this report can be viewed at: https://colab.research.google.com/drive/1_y5MCmAptpWYK-XxzziXwRSCJXfWTyX3?usp=sharing
- Author: **Wendy Ha (Swinburne University of Technology)**
## Table of Contents
1.0 Import Libraries
2.0 Data Cleaning and EDA
  2.1 Preview Granularity/Variables description
  2.2 Check duplicated rows and columns
  2.3 Handling missing values
    2.3.1 Missing values detection
    2.3.2 Dealing with Missing values
  2.4 Handling outliers
    2.4.1 Outlier detection
    2.4.2 Checking Data Distribution with Histogram and Box Plots
    2.4.3 Retrieving outliers’ data with IQR score
    2.4.4 Dealing with outliers
3.0 Data Visualization
  Question 1: What are the actual factors influencing life expectancy?
  Question 2: What effect does immunisation coverage have on life expectancy in two groups developing and developed countries?
  Question 3: What effect does Schooling and Alcohol have on Life Expectancy?
  Question 4: What effect does GDP have on life expectancy?
4.0 Conclusion
