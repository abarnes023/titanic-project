 # titanic-project

## Survival on the Titanic

This report investigates the data included in the dataset titanic_data.csv, downloaded from [Udacity](https://www.udacity.com/)  for the final project of the [Intro to Data Analysis](https://www.udacity.com/course/intro-to-data-analysis--ud170) free course.

The questions that this report tries to answer are: which factors were predictive of survival on the Titanic and can we build a model based on these factors to predict survival? The factors that were investigated include:
- Ticket class
- Sex
- Age
- Number of siblings/ spouses aboard
- Number of parents/ children aboard
- Passenger fare
- Port of embarkation


### Analysis

The report uses chi-square tests for independence, Welch's t-tests, and a Logistic Regression model to investigate the factors that best predict survival.

For the **Welch's t-tests**, the null hypothesis for the variables being investigated is that there is no difference in the population means for the survival group vs non-survival group. Under the null hypothesis, for example, the mean age for those that survived and those that did not survive would not be statistically different. My hypothesis is that the population means for the variables are different between the survival and non-survival groups (e.g. the mean age for those who survived is different than the mean for those who did not survive).

For the **chi-square tests for independence**, the null hypothesis is that knowing the value of the categorical variable (e.g. sex of the passenger) cannot help predict the survival outcome, and therefore survival and the variable are independent. My hypothesis is that these variables are not independent from survival outcome, and knowing their values can help predict survival or non-survival.


### References and More Info

For more detailed information on the dataset please visit [Kaggle](https://www.kaggle.com/c/titanic/data), which is where Udacity obtained the data.

The Logistic Regression model and analysis in this report were created with references to the guides written by Susan Li on [Medium](https://towardsdatascience.com/building-a-logistic-regression-in-python-step-by-step-becd4d56c9c8), Kevin Markham's example on [Data School](http://www.dataschool.io/logistic-regression-in-python-using-scikit-learn/), and the blog post on [Data-Mania](http://www.data-mania.com/blog/logistic-regression-example-in-python/).

The Python libraries used in this analysis include:
- Pandas
- NumPy
- scikit-learn
- Matplotlib
- Seaborn
- SciPy
