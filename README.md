# matplotlib_challenge
Module 5 assignment was completed to assess understanding of Matplotlib and data visualization.

## Background
You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.
As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

## Instructions
This assignment is broken down into the following tasks:

* Prepare the data.
* Generate summary statistics.
* Create bar charts and pie charts.
* Calculate quartiles, find outliers, and create a box plot.
* Create a line plot and a scatter plot.
* Calculate correlation and regression.
* Submit your final analysis.

**Prepare the Data**

1.	Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

2.	Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

3.	Display the updated number of unique mice IDs.

**Generate Summary Statistics**

Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.
Your summary statistics should include:

* A row for each drug regimen. These regimen names should be contained in the index column.
* A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

**Create Bar Charts and Pie Charts**
1.	Generate two bar charts. Both charts should be identical and show the total total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

* Create the first bar chart with the Pandas DataFrame.plot() method.
* Create the second bar chart with Matplotlib's pyplot methods.

![BarChart](https://github.com/MpatiM/matplotlib_challenge/assets/159741444/3977677b-5563-497c-b827-cf208effe96e)


2. Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

* Create the first pie chart with the Pandas DataFrame.plot() method.
* Create the second pie chart with Matplotlib's pyplot methods.

![PieChart](https://github.com/MpatiM/matplotlib_challenge/assets/159741444/deeb9e1b-684e-462a-9a18-777d2f97dfb0)


**Calculate Quartiles, Find Outliers, and Create a Box Plot**

1.	Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

* Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.
* Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
* Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
* Determine outliers by using the upper and lower bounds, and then print the results.

2.	Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.

_**hint**: All four box plots should be within the same figure. Use this Matplotlib documentation pageLinks to an external site. for help with changing the style of the outliers._

![BoxPlot](https://github.com/MpatiM/matplotlib_challenge/assets/159741444/7fae95c1-50ad-4e25-91a5-6ec86dadf84a)


**Create a Line Plot and a Scatter Plot**

1.	Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.
2.	Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

![IDedLinePlot](https://github.com/MpatiM/matplotlib_challenge/assets/159741444/cb34c36a-12a7-4d17-8a31-c4010fd74d31)
![ScatterPlot](https://github.com/MpatiM/matplotlib_challenge/assets/159741444/da6b2de2-1b82-4958-b26e-d0d90b5b9a88)


**Calculate Correlation and Regression**
1.	Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.
2.	Plot the linear regression model on top of the previous scatter plot.

![LinRegressionModel](https://github.com/MpatiM/matplotlib_challenge/assets/159741444/16502dcf-3869-4dbc-a999-120989086e88)


## Analysis
Write three observations or inferences based on observations made. Analysis should be written at the beginning of jupyter notebook.
