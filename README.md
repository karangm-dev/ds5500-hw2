# ds5500-hw2

## Problem 1¶

**Confirm your group for the second project component. Check in with me if the group is different from the first project component. Post a public note on Piazza in the project folder with the title “[group] all group members’ last names”. Include in the body of the note all of the group members’ full names.**

Group - Samdariya, Kasoju, Muralidhar, Kanuparti

Aanchal Anil Samdariya<br/>
Apoorva Kasoju<br/>
Karan Gulur Muralidhar<br/>
Krishna Sai Rohith Kanuparti<br/>

## Problem 2

**Choose and critique one of the visualization by one of your fellow classmates for HW 1 Problem 2 (distribution of income across countries and continents over time). Include a link to the original. Describe the visualization and how it is similar and/or different from yours. Is it easy to interpret? Does it effectively visualize what is being asked? Why or why not?**

VISUALIZATION LINK - https://colab.research.google.com/github/prathwishshetty/DS5500-Homework-1/blob/master/ds5500_hw1.ipynb<br/>
GITHUB - https://github.com/prathwishshetty/DS5500-Homework-1

To compare across continents, a static plot has been incorporated which is similar to what i have done. However for the distribtuion of income across countries, a dynamic plot has been used compared to static plot of mine.

The dynamic plot with a world map incorporated is a visual treat to observe and it represents so much information effieciently. The timeline scale shows how the income changes over time. The only disadvantage of the dynamic plot is that if you want to check out the changes for a particular country over time and see if there was any dip or increase, a static might be a better choice.

## Problem 3

**Choose and critique one of the visualization by one of your fellow classmates for HW 1 Problem 3 (relationship between income, life expectancy, and child mortality over time). Include a link to the original. Describe the visualization and how it is similar and/or different from yours. Is it easy to interpret? Does it effectively visualize what is being asked? Why or why not?**

VISUALIZATION LINK - https://colab.research.google.com/github/prathwishshetty/DS5500-Homework-1/blob/master/ds5500_hw1.ipynb<br/>
GITHUB - https://github.com/prathwishshetty/DS5500-Homework-1

The static plot to depict relationship between income, life expectancy and child mortality is similar to what i have. The plot is substantiated with explanation of dips and outliers and potential reasons for it which is worth noting. However the solution is devoid of the explicit representation of relationship across all continents. 

## Problem 4

**Choose and fit one or more models to quantify the relationship betweem income (GDP per capita) and life expectancy over time. Justify your choice of model and comment on its appropriateness. (You are not required to handle the autocorrelation of time series, but should comment on how this impacts your analysis.) Visualize the model(s) and comment on what they tell you about the relationship between income and life expectancy over time.**


From the figure, we can clearly observe that the relationshsip between income and life_expectancy. Since there was lot of variance for a given a life expectancy value, i aggregated the value across all countries and continent by time and get the average income and average life expectancies.

![alt text][logo_4]

[logo_4]: https://github.com/karangm-dev/ds5500-hw2/blob/master/output/4.png "Fig: Income vs Life Expectancy"

Also, i applied log transformation to get more linear curve. After applying log transformation, I tried fitting various models as follows:<br/>
Model 1 - log(y) ~ x <br/>
Model 2 - log(y) ~ x + x^2 <br/>
Model 3 - log(y) ~ x + x^2 + x^3 <br/>
Model 4 - log(y) ~ x + x^2 + x^3 + x^4 <br/>

Overall, the model4 performed well with an adjusted r^2 value of 0.98

![alt text][logo_4_4]

[logo_4_4]: https://github.com/karangm-dev/ds5500-hw2/blob/master/output/4_4.png "Fig: Income vs Life Expectancy Model Output"

We can see a positive relation between life expectancy and GDP as expected i.e. with increase in GDP over time, the life expectancy will increase.

## Problem 5

**Choose and fit one or more models to quantify the relationship betweem income (GDP per capita) and child mortality over time. Justify your choice of model and comment on its appropriateness. (You are not required to handle the autocorrelation of time series, but should comment on how this impacts your analysis.) Visualize the model(s) and comment on what they tell you about the relationship between income and child mortality over time.** 

From the figure, we can clearly observe that the relationshsip between income and child_mortality. Since there was lot of variance for a given a life child_mortality, i aggregated the value across all countries and continent by time and get the average income and average child_mortality.

![alt text][logo_5]

[logo_5]: https://github.com/karangm-dev/ds5500-hw2/blob/master/output/5.png "Fig: Income vs Child Mortality"

Also, i applied log transformation to get more linear curve. After applying log transformation, I tried fitting various models as follows:<br/>
Model 1 - log(y) ~ x <br/>
Model 2 - log(y) ~ x + x^2 <br/>
Model 3 - log(y) ~ x + x^2 + x^3 <br/>
Model 4 - log(y) ~ x + x^2 + x^3 + x^4 <br/>

Overall, the model4 performed well with an adjusted r^2 value of 0.99.

We can see a negative relation between child mortality and GDP as expected i.e. with increase in GDP over time, the child mortality will decrease.

![alt text][logo_5_4]

[logo_5_4]: https://github.com/karangm-dev/ds5500-hw2/blob/master/output/5_4.png "Fig: Income vs Child Mortality"
