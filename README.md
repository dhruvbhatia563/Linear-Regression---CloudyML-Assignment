# Linear-Regression: CloudyML-Assignment

Linear Regression is a statistical technique which is used to find the linear relationship between dependent and one or more independent variables. This technique is applicable for Supervised learning Regression problems where we try to predict a continuous variable.

### Simple Linear Regression (SLR)

Simple Linear Regression (or SLR) is the simplest model in machine learning. It models the linear relationship between the independent and dependent variables.

This assignment is based on the TV and Sales data . There is one independent or input variable which represents the TV data and is denoted by X. Similarly, there is one dependent or output variable which represents the Sales and is denoted by y. We want to build a linear relationship between these variables. This linear relationship can be modelled by mathematical equation of the form:-

             Y = β0   + β1*X    -------------   (1)
In this equation, X and Y are called independent and dependent variables respectively,

β1 is the coefficient for independent variable and

β0 is the constant term.

β0 and β1 are called parameters of the model.

For simplicity, we can compare the above equation with the basic line equation of the form:-

               y = ax + b       ----------------- (2)
We can see that

slope of the line is given by, a = β1, and

intercept of the line by b = β0.

In this Simple Linear Regression model, we want to fit a line which estimates the linear relationship between X and Y. So, the question of fitting reduces to estimating the parameters of the model β0 and β1.

### Ordinary Least Square Method

The TV and Sales data are given by X and y respectively. We can draw a scatter plot between X and y which shows the relationship between them.

Now, our task is to find a line which best fits this scatter plot. This line will help us to predict the value of any Target variable for any given Feature variable. This line is called Regression line.

We can define an error function for any line. Then, the regression line is the one which minimizes the error function. Such an error function is also called a Cost function.

## Problem Statement Build a model which predicts sales based on the money spent on different platforms for marketing.

#### Data Dict:

There are 3 Input Variables and 1 Output Variable (Sales).
The data type of all the input variables is float64. The data type of out variable (Sales) is float64.

![image](https://user-images.githubusercontent.com/68370376/183360947-5ec167b1-0758-40d4-99d4-1bbc0d42e5bc.png)

> No Strong Linear Relationship between Radio with Sales and Newspapaer with Sales

> TV and Sales shows strong positive linear relationship

![image](https://user-images.githubusercontent.com/68370376/183361095-cf0816c4-6598-443e-b502-8d47bdbe1d2b.png)

> Hey buddy! did you notice ? the above graph shows some sort of relationship between sales and TV. Don't you think this shows positive linear relation? i.e when As TV's value increases sales increases ans same is vise-versa.

![image](https://user-images.githubusercontent.com/68370376/183361178-9304349e-b608-4193-b0f8-40e8caaee63c.png)

> The above graph also shows positive linear relation between both TV and Sales.

#### Performing Simple Linear Regression

Equation of linear regression
𝑦=𝑐+𝑚1𝑥1+𝑚2𝑥2+...+𝑚𝑛𝑥𝑛
𝑦 is the response
𝑐 is the intercept
𝑚1 is the coefficient for the first feature
𝑚𝑛 is the coefficient for the nth feature

#### In our case:

𝑦=𝑐+𝑚1×𝑇𝑉
The 𝑚 values are called the model coefficients or model parameters.

#### Mechanics of the model

> Split the dataset into two sets – the training set and the test set. Then, instantiate the regressor lm and fit it on the training set with the fit method.

> In this step, the model learned the relationships between the training data (X_train, y_train).

> Oh Yeah! Now the model is ready to make predictions on the test data (X_test). Hence, predict on the test data using the predict method.

The steps are as follow:

#### Train test split

> Split the dataset into two sets namely - train set and test set.

> The model learn the relationships from the training data and predict on test data.

![image](https://user-images.githubusercontent.com/68370376/183361839-059d1e5c-4c1a-4d81-9c22-f3081ef67830.png)

![image](https://user-images.githubusercontent.com/68370376/183361904-a53a4c60-eb22-4654-9243-dd29494b9b75.png)

# Predicting Sales values on first five 5 TV  datasets only
array([19.49966095,  9.3759692 ,  7.88687015, 15.21236477, 16.81055533])

> Train - RMSE value:  2.3984162246129914

> Train - R2 Score value:  0.8157933136480389

> Test - RMSE value:  2.019296008966233

> Test - R2 Score value:  0.7921031601245658

#### Checking for Overfitting or Underfitting the data by calculation score using score function.

> Training set score:  0.816

> Test set score:  0.792

#### Residual analysis

![image](https://user-images.githubusercontent.com/68370376/183362451-bf76ed09-c703-4d88-af37-d1a4d179c228.png)


***** The END *****


