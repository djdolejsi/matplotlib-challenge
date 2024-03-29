# matplotlib-challenge

# Background
You've just  joined Pymaceuticals Inc., a new pharmaceutical company that specializes in anti-cancer pharmaceuticals. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice identified with SCC tumor growth were treated with a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the study. They have also asked for a top-level summary of the study results.

# Prepare the Data


Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.


Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining step.


Display the updated number of unique mice IDs.



Generate Summary Statistics
Create two summary statistics DataFrames:

* For the first table, use the `groupby` method to generate the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen. This should result in five unique series objects. Combine these objects into a single summary statistics DataFrames.

* For the second table, use the `agg` method to produce the same summary statistics table by using a single line of code.



# Create Bar Charts and a Pie Charts


Generate two bar plots. Both plots should be identical and show the total number of timepoints for all mice tested for each drug regimen throughout the course of the study.


Create the first bar plot by using Pandas's DataFrame.plot() method.

![image](https://user-images.githubusercontent.com/105513598/226959104-1f62bdc3-46aa-409c-8f11-7128b664a013.png)

Create the second bar plot by using Matplotlib's pyplot methods.

![image](https://user-images.githubusercontent.com/105513598/226959212-54d8c548-ba9b-4ff4-84ac-affe36672f9c.png)


Generate two pie plots. Both plots should be identical and show the distribution of female or male mice in the study.


Create the first pie plot by using both Pandas's DataFrame.plot().

![image](https://user-images.githubusercontent.com/105513598/226959312-26983bfb-5fec-4e9e-98f9-60a82041a854.png)

Create the second pie plot by using Matplotlib's pyplot methods.

![image](https://user-images.githubusercontent.com/105513598/226959403-c665ae5d-59bc-4a34-894d-bc141c77fd2c.png)



#Calculate Quartiles, Find Outliers, and Create a Box Plot


Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR and determine if there are any potential outliers across all four treatment regimens. Follow these substeps:


Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.


Create a list that holds the treatment names, as well as a second, empty list to hold the tumor volume data.


Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.


Determine outliers by using the upper and lower bounds, and then print the results.




Using Matplotlib, generate a box plot of the final tumor volume for all four treatment regimens. Highlight any potential outliers in the plot by changing their color and style.



# Create a Line Plot and a Scatter Plot


Select a mouse that was treated with Capomulin and generate a line plot of tumor volume vs. time point for that mouse.


Generate a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen.



# Calculate Correlation and Regression


Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment.


Plot the linear regression model on top of the previous scatter plot.

![image](https://user-images.githubusercontent.com/105513598/226959689-5c1fbd59-7e5a-4094-9a24-6b5b02067741.png)

# Submit Your Final Analysis
Review all the figures and tables that you generated in this assignment. Write at least three observations or inferences that can be made from the data. Include these observations at the top of your notebook.
