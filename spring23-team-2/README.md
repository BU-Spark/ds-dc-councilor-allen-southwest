# Team 2 - Gun Violence in Southwest DC


## General Overview and Project Goal

The Southwest District has seen a lot of change in the last few years and certain areas have been completely overhauled (construction of wharf, stadiums, etc.). This has caused a clear distinction between the west and the east part of the district (specifically, Tracts 102 and 110 on the west, and Tract 64 and 105 on the east).
There also are 3 big public housing communities (Greenleaf Gardens, Syphax Gardens, and James Creek) in the east part of the Southwest District and this so called “neighborhood within a neighborhood” faces a lot of problems that are associated with generational poverty, such as high rates of unemployment, community violence, substance use, chronic disease, teen pregnancy, and food insecurity. 
The goal of this project is to provide a data dashboard which shows that these issues exist, so that these visualizations can be used as arguments to convince stakeholders in this district to aim for change. Furthermore, by analysing certain variables and inspecting correlations between them, we aim to detect underlying issues that perpetuate the issue of generational poverty so that decision-makers have an easier time approaching the task of improving the status-quo of this district.

## Team 2's Approach

While Team 1's focus is on Crime and Team 3's focus is on Education (primarily), Team 2 decided to tackle the other variables of interest to the clients. This means that we did not choose one specific topic and explored it in-depth, but rather that we focused on covering the bases. We picked broader variables and explored how they correlate with the issue of disparity and poverty.

## File Structure

The file structure is not yet finalized. We wanted to wait until deliverable 3 to finalize the organization. This part of the README will be updated accordingly.

Generally, however, we will have a /data folder that contains all the data that we worked with. We will also have a subfolder for every member that contains their specific notebooks and other work. Last but not least, we will have a /plots folder, in which all the variables will have their respective subfolder. These subfolders will contain all the relevant plots.

## Run Code

This will also be updated once deliverable 3 is submitted. We aim to have a specific how_to_run.md file in every members' subfolder, specifying how future users can run their notebooks.

For now, it will be put here:

#### Revathi
poverty_working_poor_analysis.py

Poverty vs Employment Analysis 

The code reads data from two CSV files ("poverty_2020_15.csv", "poverty_2015_10.csv", PATH= "../data/census/") containing poverty statistics for different years, creates bar charts showing the percentage of full-time and part-time employees living below the poverty level in different areas, and plots the charts using Matplotlib.

The first part of the code reads the data for the year 2020-2015, extracts the relevant rows and columns, and converts the data into a format suitable for plotting. The second part of the code does the same for the year 2015-2010.

Both sections of the code create a bar chart with two groups of bars side by side, representing the percentage of full-time and part-time employees below the poverty level in each area. The x-axis shows the different areas, and the y-axis shows the percentage below poverty level.  

The output of running the code will be two bar charts, one for each year, showing the poverty status of full-time and part-time employees in different areas. The charts will be displayed using Matplotlib.  

  

python poverty_working_poor_analysis.py

Poverty vs Sex and Race Analysis:  

The code requires several dataframes stored in a list poverty_dfs that contains data on poverty status for various locations and years. To run this code, you will need to first load the necessary dataframes into Python and store them in the poverty_dfs list.  

Once you have the dataframes, you can simply copy and paste the above code into a Python script or Jupyter Notebook and run it. The code will create a bar chart showing the year-wise distribution of poverty status among males for five different tracts (Tract 64, Tract 102.01, Tract 102.02, Tract 105, and Tract 110.01) in a grouped manner. The resulting plot will be displayed in the output of the cell or script. Similarly the following ipynb files produce visualizations for poverty status among females, whites, blacks, indians, asians, and hispanic or latino.  
  
mobility_gender.ipynb  
  
Mobility vs Gender:  

The code uses the data from a dataframe mobility_sex_df to create a bar chart that shows the mobility of males and females within and between counties and states for six different tracts.

The code first selects the relevant data from the dataframe and assigns it to variables mobility_male_within_county, mobility_female_within_county, mobility_male_within_state, and mobility_female_within_state. Then, it defines the x-axis labels as the names of the six tracts.

Next, the y-axis values for each gender and location are defined by converting the values from the selected dataframe columns to lists of integers. Two additional lists are created by adding the intra-county and inter-state mobility values for females.  

The code then uses the plt.bar() function to create the stacked bar chart, with each bar representing a tract and each color representing a different type of mobility (male/female, within/between county or state). The legend is added using the plt.legend() function, and the axis labels and chart title are added using plt.xlabel(), plt.ylabel(), and plt.title().  

Finally, the values for each bar are displayed on the chart using the plt.text() function. The chart is displayed using the plt.show() function.  
  
Mobility vs Race:

The code generates a bar chart using matplotlib to show the mobility of different racial groups within a county and state.

First, the script imports the necessary libraries, defines the x-axis labels, and extracts the mobility data for whites, blacks, Asians, Hawaiians, and Indians from separate data frames. Then, it calculates the total mobility of whites and blacks by adding the mobility within the county and state. Afterward, it calculates the total mobility of Asians, Hawaiians, and Indians by adding their mobility to the previously calculated total of whites and blacks.

The script then defines the colors and stacking order of the bars and plots the data using the plt.bar() function. It also adds x-axis labels, y-axis labels, a chart title, and a legend using plt.xticks(), plt.xlabel(), plt.ylabel(), plt.title(), and plt.legend(), respectively.Finally, the chart is displayed using plt.show().


#### Mingxin
  
1. To begin, access the .ipynb file by utilizing Google Colab.  
2. Then proceed to upload the necessary data files located within the spring23-team-2/data folder to your Google Drive base directory. 
3. Once uploaded, execute the sequence of steps as presented to generate the desired output.

#### Jonas

Simply choose the notebook of choice and run all the cells. Everything is ready to go and should produce the plots of that variable. 
The only thing that you might need to change is the path for the .csv files and the path to the directory in which you want the plots to be saved.
