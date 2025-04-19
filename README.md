# Retail Revenue Prediction Task (Predicting with Limited Data)
This project develops a revenue prediction model for ABC-Retail using limited transaction data to predict quarterly revenue indices. The project addresses several key challenges including small sample size, varying reporting periods, and the need to aggregate daily data to quarterly predictions.

![image](https://github.com/user-attachments/assets/4b3ed551-fc47-416d-8850-4822ed1e3d5b)
## Retail Revenue Prediction (Predicting with Limited Data)

In this project, I developed a revenue prediction model for a made up retailer using limited transactional data. This mini project was split into 3 steps including: Data Cleaning, Feature Engineering and Modeling. 

////////////////////////////////////////////////////////////////////

predicted if the Falcon 9 first stage would land successfully. SpaceX advertised Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings was because SpaceX could reuse the first stage. Therefore if it was determined if the first stage would land, the cost of a launch could be determined. This information could be used if an alternate company wanted to bid against SpaceX for a rocket launch.

### [SpaceX API Data Collection](https://github.com/CarlBrazier/SpaceX_Falcon9_First_Stage_Landing_Prediction/blob/main/jupyter-labs-spacex-data-collection-api.ipynb)
- Data Collection: Retrieved data via the SpaceX API, including launch details like dates, rocket type, and payload mass.
- Data Cleaning: Addressed missing values and transformed data for analysis.
- Data Analysis: Conducted exploratory analysis to identify trends in launch data.
- Data Exporting: Saved the cleaned data to a CSV file for further use.

### [Data Wrangling](https://github.com/CarlBrazier/SpaceX_Falcon9_First_Stage_Landing_Prediction/blob/main/labs-jupyter-spacex-Data-wrangling.ipynb)
- Exploring Launch Sites: Analyzed the number of launches from different SpaceX launch sites.
- Examining Orbit Types: Understood various orbit types targeted by these launches.
- Data Cleaning: Prepared the data by handling missing values and removing unneeded columns.
- Data Export: Saved the cleaned and processed data into a CSV file for further analysis.

### [Web Scraping Launch Records from Wikipedia](https://github.com/CarlBrazier/SpaceX_Falcon9_First_Stage_Landing_Prediction/blob/main/jupyter-labs-webscraping.ipynb) 
- Data Retrieval: Retrieved data from a static URL pointing to a specific revision of a Wikipedia page on Falcon 9 and Falcon Heavy launches.
- Data Parsing: Initial steps used requests.get() to fetch the webpage content for scraping.

### [EDA - SQL](https://github.com/CarlBrazier/SpaceX_Falcon9_First_Stage_Landing_Prediction/blob/main/jupyter-labs-eda-sql-coursera_sqllite.ipynb)
- Database Connection: Established a connection to a local SQLite database to store and retrieve the SpaceX dataset.
- Data Loading: Involved reading the downloaded CSV file containing the SpaceX launch data and loading this data into a SQL table within the SQLite database. This step was critical for performing SQL-based data manipulation.
- Data Analysis SQL Queries: Performed operations such as filtering, sorting, and aggregating data to extract insights related to the economics of SpaceX launches, focusing on the reusability of the Falcon 9 rocket's first stage, to determine the cost implications of landing the first stage of the Falcon 9.

### [EDA Through Data Visualisation](https://github.com/CarlBrazier/SpaceX_Falcon9_First_Stage_Landing_Prediction/blob/main/jupyter-labs-eda-dataviz.ipynb) 
- Data Loading: Utilized the Pandas library to load the CSV data directly into a DataFrame for immediate manipulation and analysis.
- Data Visualization: Employed Matplotlib and Seaborn for creating visualizations.
  - Categorical scatter plots to analyze the relationship between flight number and payload mass, categorized by mission outcome (success or failure).
  - Scatter plots to assess the correlation between launch sites, payload mass, and other relevant mission details, providing insights into factors influencing launch success.

### [Data Visualisation: Dashboard](https://github.com/CarlBrazier/SpaceX_Falcon9_First_Stage_Landing_Prediction/blob/main/jupyter-labs-build-a-dashboard-application-v10.ipynb)
- Library Installations: Installed Plotly, Pandas, and Dash.
- Dashboard Components: Set up a Plotly Dash application that included various interactive components such as dropdown lists and range sliders.
- Visualization Features:
  - Pie charts to analyze launch success rates based on selected criteria from dropdown menus.
  - Scatter plots to explore correlations between payload mass and other launch variables.
  - These visualizations were interactive, allowing users to select different parameters and instantly see updated results.
