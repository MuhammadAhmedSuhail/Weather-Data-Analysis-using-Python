# Weather-Data-Analysis-using-Python

## Project Description
The aim of this project is to perform a comprehensive analysis of weather data using Python. Weather data provides us with information about temperature, humidity, wind speed, and other atmospheric conditions. This project also aims to address the common challenge of missing data in data analysis. The dataset used is "Weather Records.xlsx", which contains 13 columns, including a prediction column for precipitation (in).

## Data Preprocessing
To deal with missing data, I used various methods such as forward fill, backward fill, and interpolation. I only dropped rows if they could not be filled in by any of these methods. For the date column, I created new features such as month, year, and day of the week.

The following columns were dropped due to missing data:
- Snow Depth: Too many missing values
- Wind Gust (mph): No clear correlation with precipitation
- Sea Level Pressure (in): Not relevant to precipitation prediction

## Dimensionality Reduction
I used PCA for dimensionality reduction with 3 components. I encoded categorical features such as the month and day of the week into numerical representations. PCA helped to reduce the dimensionality of the dataset and identify the most important features for precipitation prediction.

## Data Visualization
I created a scatterplot for the precipitation column and the principle components to determine the relationship between them so I could identify which component will help in predicting the value of precipitation.
The three scatterplots generated are attached below:

![X1vsY](https://user-images.githubusercontent.com/72251313/233482591-7a187221-fe2f-42b4-a607-5f37e73ced96.png)

![X2vsY](https://user-images.githubusercontent.com/72251313/233482610-0aa89ded-d33a-4035-99ee-b0058360e8e3.png)

![X3vsY](https://user-images.githubusercontent.com/72251313/233482641-ecb43f0c-fcd7-485d-974a-5ba39bcb3091.png)

By Analyzing the ScatterPlots we can conclude the fact that the first principal component had a strong positive correlation with precipitation.

## Conclusion
In conclusion, I was able to address the challenge of missing data in weather data analysis by using various methods for filling in missing values and dropping columns with irrelevant or missing data. I gained insights into the data through visualization and dimensionality reduction techniques, and identified the most important features for precipitation prediction.

## Tools Used
- Numpy
- Pandas
- Matplotlib
- Sklearn
- Seaborn

## Author:
- Muhammad Ahmed Suhail

## Acknowledgments:
- This project was completed as an assignment for Data Analysis at FAST - NUCES Islamabad.


