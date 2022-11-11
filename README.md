# Economic-Data-Analysis-Project

In this Project I will be utilizing Fred API to obtain Data from Fred(Federal Reserve Economic Data) as well as utilizing serveral libraries from python such as pandas, numpy, matplotlib and plotly.express in order to complete the project. 

Fred Website: https://fred.stlouisfed.org/docs/api/fred/

1. Utilizing Fred API to retrieve Data

  - Importing The API Key with enviromental variable build in os system to hide my personal key
  
2. Data Exploration

  - fred.search allows us to search any data within the fred database just like how we search on a website and return us the data in panda dataframe
  
  - fred.get_series('xyz) allows us to pull raw data from fred
  
  - Imported a lineplot to analyze the S&P500, and S&P reached all time high in 2022.
  
  - Plotting our unemployment rate data and assuming that covid might be the main reason behind the face that unemployment rate spikes up during 2019. 
  
 3. Retrieving Data Regarding Unemployment Rate among different states
 
  - Specifically look for unemployment rate data in different states
  
  - Utilized for loop function in order to combined all the raw data together in the list and using the pd.concat function to concatenate all the data into a dataframe
  
  - Removed unneccesary data from dataframe.
  
 4. Data Cleaning
 
  - Remove Null Values
  
  - Utilized to_dict() to rename all the column alias name to a formal state name.
  
 5. Data Visualization
 
  - Utilized plotly.express library to visualize our data for the unemployment rate in different states from 1980 to 2020 ( graph can be downloaded as pic in file)
  
  - Utilized Barplot to demonstrated the Unemployment Rate in 2020 May within different states.
  
  - Using Subplots to show the participation rate and unemployment rate with the same graph. We can assume that as unemployment rate goes up, labour force rate goes     down as more people being unemployed means fewer people will be participated in the labor force. Moreover, as unemployment rate starts going down, we can tell       that labour force rate starts going up as more individuals are getting employed again. 
  
  - In the last table, I compare the Participation Rate and Unemployment Rate in Different States in One figure with different mini tables.
      
      - Utilized plt.subplots(10,5 ,figsize=(20,20),sharex= True) where 10 and 5 indicates the row and column for the quantity of our mini table and sharex                 indicated that all the mini table share the same x axis in order to keep the table organized and cleaned.
      
      - Utilized for loops to allow us to remove 2 extra tables and allow us to plot several mino table with one giant graph.
      
      - plt.tight_layout() allow text not to overlay on each others.
  
  
