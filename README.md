# Analyzing the impact of vaccination on humna lifespans in developed and developing nations
## Technologies and resource
- Python 3.6 
- Analysis libraries: numpy, pandas
- Visualization libraries: matplotlib, seaborn, plotly (interactive visualization), [pycountry](https://github.com/jefftune/pycountry-convert) (get continent name from country)
- Author: Wendy Ha (Swinburne University of Technology)
- The Life Expectancy (WHO) dataset: https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who
- Notebook with details coding: https://colab.research.google.com/drive/1_y5MCmAptpWYK-XxzziXwRSCJXfWTyX3?usp=sharing
## Introduction
Despite the fact that many research have been conducted in the past on factors impacting life expectancy, including demographic characteristics, income composition, and mortality rates, Max Roser emphasized on Our World In Data that the influence of vaccines has been overlooked (Max et al 2013).
<br/>
<br/>
Share the same concern with Max, two researchers from World Health Organization (WHO) Department of Data and Analytics, Deeksha Russell and Duan Wang, have compiled a collection of statistics on the key drivers of life expectancy, with a focus on immunization variables including Hepatitis B, Measles, Polio, and Diphtheria (Deeksha and Duan 2015). Furthermore, mortality, economy, social issues, and other health- related aspects are all taken into consideration (Deeksha and Duan 2015). As a result, numerous analyses of the impact of vaccination on human lifespans in developed and developing nations have been undertaken using this data set, with the goal of assisting residents in those countries in improving their quality of life.
### Objective
The analysis tries to answer the following essential questions:
- Among four main categories: vaccination-related factors, mortality-related factors, economic factors, and social factors, what are the actual factors
influencing life expectancy?
- What effect does immunisation coverage have on life expectancy?
- What effect do schooling and alcohol have on life expectancy?
- What effect does GDP have on life expectancy?
## Data Cleaning Process
### Detecting and Handling missing values
- Detecting missing values

![image](https://user-images.githubusercontent.com/90888090/175796973-03e2ef4c-cbb8-433c-bc02-83fe02c7d79d.png)

## Table of Contents
**1.0 Import Libraries** <br/>
**2.0 Data Cleaning and EDA** <br/>
**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.1 Preview Granularity/Variables description <br/>**
**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.2 Check duplicated rows and columns <br/>**
**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.3 Handling missing values <br/>**
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.3.1 Missing values detection <br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.3.2 Dealing with Missing values <br/>
**&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4 Handling outliers<br/>**
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4.1 Outlier detection<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4.2 Checking Data Distribution with Histogram and Box Plots<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4.3 Retrieving outliers’ data with IQR score<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4.4 Dealing with outliers<br/>
**3.0 Data Visualization<br/>**
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Question 1: What are the actual factors influencing life expectancy?<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Question 2: What effect does immunisation coverage have on life expectancy in two groups developing and developed countries?<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Question 3: What effect does Schooling and Alcohol have on Life Expectancy?<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Question 4: What effect does GDP have on life expectancy?<br/>
**4.0 Conclusion**
