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
- **Detecting missing values**

![image](https://user-images.githubusercontent.com/90888090/175796973-03e2ef4c-cbb8-433c-bc02-83fe02c7d79d.png)
- **Dealing with Missing values**

Using the mean (average) value of the year to replace missing values.

![image](https://user-images.githubusercontent.com/90888090/175797061-65c548c4-9a6b-459e-89b2-7cd8c2ab9652.png)
![image](https://user-images.githubusercontent.com/90888090/175797074-74f9ce38-7acb-4945-970b-272480fd7367.png)
### Detecting and Handling outliers
- **Checking Data Distribution with Histogram and Box Plots**

![image](https://user-images.githubusercontent.com/90888090/175797258-33152c11-b621-4f7e-b1b9-cc16637bdd8d.png)
![image](https://user-images.githubusercontent.com/90888090/175797275-b96aacd2-1abf-40a2-a3fc-2d0a75a91398.png)

- **Retrieving outliers’ data with IQR score**

![image](https://user-images.githubusercontent.com/90888090/175797330-51d565b3-f277-45f4-8ef0-c499e9b34593.png)
- **Dealing with outliers**

The Winsorizing approach proposed by Tukey & McLaughlin (1963) is suggested in this project to handle the outliers. An ideal approach is setting all outliers to a specific percentage of the data, for example, all data above the 95th percentile are recoded to the 95th percentile value, and all observations below the 5th percentile are recoded to 25th percentile value (Tukey & McLaughlin 1963).

![image](https://user-images.githubusercontent.com/90888090/175797428-eba82a3d-626f-4d0d-ac08-ffaf1cccf4d8.png)
![image](https://user-images.githubusercontent.com/90888090/175797351-3546d5f3-5285-404d-94ac-418115748b0b.png)
## Data Visualization
### Question 1: What are the actual factors influencing life expectancy?
![image](https://user-images.githubusercontent.com/90888090/175797460-0e8407ca-4d9a-4d30-8177-d999e486d05e.png)
### Question 2: What effect does immunisation coverage have on life expectancy in two groups developing and developed countries?
![image](https://user-images.githubusercontent.com/90888090/175797563-b2b89120-7c88-4365-81e1-90d9b6cb1a09.png)
### Question 3: What effect does Schooling and Alcohol have on Life Expectancy?
![image](https://user-images.githubusercontent.com/90888090/175797738-0f953d00-cf29-42a2-946a-91f84ff7df4f.png)
### Question 4: What effect does GDP have on life expectancy?
![image](https://user-images.githubusercontent.com/90888090/175797764-f94d7be7-2007-4938-938b-7f39bed4e1b3.png)
## Conclusion
1. The World Health Organization's data set on variables impacting life expectancy still has a lot of missing numbers. These missing data values are primarily seen in nations with small populations, where data sources are not abundant.
2. This dataset also contains numerous outliers that have been reprocessed using the Winsorization approach.
3. Many developing countries are doing a good job of promoting vaccination against hepatitis B, polio, and diphtheria among 1-year-old children in order to improve the life expectancy of their citizens. However, the availability of the measles vaccine still needs to improve because they is one of the most dangerous causes of the recent life expectancy declines.
4. One of the diseases that has a substantial influence on life expectancy in underdeveloped countries is HIV/AIDS. This directly highlights the important role of education in resolving this issue. If the number of people in developing countries who go to school increases, so does the number of HIV/AIDS infections and the mortality rate by HIV/AIDS will reduced. As a result, life expectancy possibly rises.
5. Furthermore, Alcohol intake is a severe problem in industrialised countries, with a detrimental influence on life expectancy. When the amount of alcohol consumed gets out of control (Centers for Disease Control and Prevention 2015), it has a negative impact on health, which in turn is a decrease in life expectancy.
