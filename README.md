# Profit Drivers and Trends in the US and UK Film Industry 2010-2023
## Project Description 
This project explores the relationships between key factors in the UK and US movie industries, uncovering trends, establishing the major factors driving profit and suggesting areas for improvement in the film industry, using data from The Movie Database (TMDB). The analysis focuses on the period between 2010 and 2023, covering various aspects of film production and performance.

## Key Objectives:

- Identify correlations between budget, runtime, average rating, and profit
- Analyze the performance of top production companies by profit, average budget, average user rating and profit trends over time
- Examine genre-level investment and return, highlighting profitable genres and areas for improvement
- Investigate release year trends by metrics provided by the dataset

## Data Sources
- Movies main data obtained from asaniczka, (2024). Full TMDB Movies Dataset 2024 (1M Movies) (Data obtained from The Movie Database [TMDB]). Retrieved from [Kaggle](https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies/data)

- Popularity metrics obtained from TMDB Popularity Guides, (2024): Retrieved from [TMDB docs](https://developer.themoviedb.org/docs/popularity-and-trending#tv-shows)

- Movie Parent Company data obtained and clarified from Wikipedia. (n.d.). List of film production companies. Retrieved from [Wikipedia](https://en.wikipedia.org/wiki/List_of_film_production_companies)

## Tools
- Python(Pandas) - Data Cleaning 
- Power Bi - Data Transformation, Exploration and Visualization

## Data Cleaning/Preparation
At the data cleaning phase, I performed the following tasks uisng Python
- Data loading and inspection
- Handling missing data
- Data formatting
- *ipynb file showcasing the steps taken in this process is provided in this repository*

## Data Transformation
At the Data transformation phase, I performed the follwing tasks using power Bi
- Creating New Columns off Main Table
- Creating Bridge Tables
- Aggregating data

## Data Exploration
At the Data Exploration phase, I asked the following questions:
  - What are the factors affecting profit?
  - What relationships exist between the different factors in the movie industry?
  - What are the top performing production companies on profit?
  - What trends are observable over the years in the movie industry?   
#### Correlation Analysis
  To better understand the relationships between factors and answer questions posed, I calculated correlation coefficients using Power BI. The scatter plots and figures 
  below illustrate the correlations:
  
  <img width="608" alt="2024-09-13 (10)" src="https://github.com/user-attachments/assets/204c374a-bd76-442a-a64a-68658b1c45bd">

  
  Using the Power BI correlation coefficient function, I calculated and displayed the Correlation Coefficient of key variables in the movie industry, all of which displayed some level of positive relationship. Scatter plots were also used to further visualize the relationships between these key variables. The gauge visuals above display the correlation coefficients between:
  - Net Profit and Average Rating: 0.29 (weak positive correlation)
  - Budget and Runtime: 0.42 (moderate positive correlation)
  - Runtime and Average Rating: 0.40 (moderate positive correlation)
  - Net Profit and Budget: 0.64 (strong positive correlation)
  - Net Profit and Popularity: 0.15 (very weak positive correlation)
  - Net Profit and Runtime: 0.30 (weak positive correlation)

From the Correlation Coefficients, it is observed that budget is the major player in determining a movie's financial success but, it's not the only factor at play. A great rating, engaging runtime, and very minimally, popularity can all contribute to a movie's financial success, but they are no definite guarantees of success. Surprisingly, popularity has little or no significant impact on Profit.




