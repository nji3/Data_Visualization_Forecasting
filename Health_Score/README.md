# Health Score Analysis
The health score data of the employees from one company is used here. I visualize the data and did some analysis without applying any statistical tools. Simply try to understand the data and check some trend. Here is how I start.

## Understand the data

<div align="center">
        <img src="https://github.com/nji3/Data_Visualization_Forecasting/blob/master/Health_Score/images/First10.png" width="400px"</img> 
</div>

The first 10 rows of the original dataset is plotted above. It contains the Quarter number (the time period record made), the Employee ID, the Gender, the Race, the Age of the employees, go to hospital or not, Salary and the Health Scores.

We would want to see the summary statistics of each column and check if there is any missing value:

<div align="center">
        <img src="https://github.com/nji3/Data_Visualization_Forecasting/blob/master/Health_Score/images/Summary.png" width="400px"</img> 
</div>

The whole dataset has the missing values. The 'Sex' coloumn has 71 missing values and the 'Race' column has 2123 missing values.

Not all the values in the dataset are reasonable. The most irreasonable value is in the 'Age' column. We could see that the maximum value in the 'Age' column is 172, which is not possible for a human being. We would need to check if this is just one employee or there are more employees with irreasonable ages.

<div align="center">
        <img src="https://github.com/nji3/Data_Visualization_Forecasting/blob/master/Health_Score/images/Age.png" width="200px"</img> 
</div>

There are 1962 unique employees in total. It is confirmed that only one employee has the irreasonable age as 172. The other ages are reasonable. As a result, we would want to drop this employee from the original dataset.

## Knowing the Characteristics of the employees

<div align="center">
        <img src="https://github.com/nji3/Data_Visualization_Forecasting/blob/master/Health_Score/images/1.png" width="800px"</img> 
</div>

These count plots above show the information of different columns.

The count plot of the Sex shows that the ratio of the male and female employees are close to 1:1 in the company.

The count plot of the Races shows the ratio of the three races close to 3.8:1.9:1.

The count plot of the Ages (Here are the ages of the last quarter for each employee) shows a right skewed distribution. Most of the employees have ages from 26 to 31. We could see that there are several very young employees and some very old employees.

The count plot of total quarters employees going to hospital shows that 632 employees never go to the hospital in all the quarters. 745 employees only went to hospital in one quarter. There are a few people went to hospital for more than 3 quarters.

The count plot of total quarters employees going to hospital respect to the Sex and Races shows that there isn't a big difference among different sex groups or different race groups.

<div align="center">
        <img src="https://github.com/nji3/Data_Visualization_Forecasting/blob/master/Health_Score/images/2.png" width="400px"</img> 
</div>

The box plots and the violin plots respect to female and male shows that the ages of employees have almost the same distribution in different Sex groups.

<div align="center">
        <img src="https://github.com/nji3/Data_Visualization_Forecasting/blob/master/Health_Score/images/3.png" width="400px"</img> 
</div>

The boxplot shows that employees' salary rise in general every quarter. And we could see that generally the male employees have higher salaries in average.

## Check the relations between the Characteristics and the Health Scores

<div align="center">
        <img src="https://github.com/nji3/Data_Visualization_Forecasting/blob/master/Health_Score/images/6.png" width="400px"</img> 
</div>

Not consider any of the other characteristics, the health scores have a increasing trend by the quarter. The standratd deviation does not change a lot during all the years. But all the other statistics increase, which implies the distribution increases respect to the quarters.

<div align="center">
        <img src="https://github.com/nji3/Data_Visualization_Forecasting/blob/master/Health_Score/images/4.png" width="600px"</img> 
</div>

The boxplot shows that there is a slight increase of the health scores by quarters in general.

The first violin plot shows that the averaged health scores in the male group is a little higher than the gemale group.

The second violin plot shows that the averaged health scores in the go-to-hospital group is relatively higher than the not-go-to-hospital group. This difference is clear.

<div align="center">
        <img src="https://github.com/nji3/Data_Visualization_Forecasting/blob/master/Health_Score/images/5.png" width="400px"</img> 
</div>

Combine all the health scores and doing the boxplot respect to the Race, the Sex and the Hospital Vist again, we could see that there is not any clear difference among the races. The male group does have a bit higher health scores in general. The go-to-hospital group has a higer score than the not-go-to-hospital group in average with a smaller variance.

<div align="center">
        <img src="https://github.com/nji3/Data_Visualization_Forecasting/blob/master/Health_Score/images/7.png" width="600px"</img> 
</div>

The scatter plot of the Health Score against the Age shows two trend. First is something I've already discussed above that the go-to-hospital group has a averged higher health score. The other trend is that as the age increases, the variance of the health score decreases and the mean of the health score increases.

The scatter plot of the Health Score against the salary does not show a clear relationship between the salary and the health score.
