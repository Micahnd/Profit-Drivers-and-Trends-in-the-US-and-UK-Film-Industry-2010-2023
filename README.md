# Profit Drivers and Trends in the US and UK Film Industry 2010-2023
## Project Description 
This project explores the relationships between key factors in the UK and US movie industries, uncovering trends, establishing the major factors driving profit and suggesting areas for improvement in the film industry, using data from The Movie Database (TMDB). The analysis focuses on the period between 2010 and 2023, covering various aspects of film production and performance.

## Key Objectives:

- Identify correlations between budget, runtime, average rating, and profit
- Analyze the performance of top production companies by profit, average budget, average user rating and profit trends over time
- Examine genre-level investment and return, highlighting profitable genres and areas for improvement
- Investigate release year trends by metrics provided by the dataset

## Tools
- Python(Pandas) - Data Cleaning 
- Power Bi - Data Transformation, Exploration and Visualization

## Methodology

- **Data Collection**: I collected movie data from TMDB Movies Dataset 2024 on Kaggle.
- **Data Cleaning and Preprocessing**: I handled missing values using Python's Pandas library, dropping inconsistent and missing values, also some missing values were sourced from trusted and verified web sources and manually plugged in. Duplicate entries were removed and columns containing irrelevant information removed, data was also filtered to contain only information that fit within the scope of the analysis.
- **Data Transformation and Feature Engineering**: Using Power Bi, I created new bridge tables to establish relationship between different factors in the data, calculated Correlation Coefficients and created an average profit column using the Power BI measure
```Power BI
Average Net Profit = 
AVERAGE('Movies Main Table'[Revenue(USD)]) - AVERAGE('Movies Main Table'[Production Budget(USD)])
```
- **Data Visualization and Exploration:** - Created various charts and visualizations in Power BI to identify patterns and trends, also explored relationships between variables, including net profit and other factors.

## Key Findings
- Budget and Profit Correlation: A strong correlation exists between budget and profit, indicating that production companies with higher budgets tend to generate more profit from movies.
- Multivariate Correlations: Moderate correlations are observed between runtime, average rating, and budget, suggesting interconnected relationships between these factors.
- Genre Impact on Profit: Budget is not the sole determining factor for profit; movie genre also significantly impacts profitability.
- 2020 Profit Decline: Profit from movies declined in 2020, with many production companies recording substantial losses.
- Trends in Runtime and Budget: The runtime of movies and average budget have increased over the years, especially after 2020.

## Visualizations
  To better understand the relationships between factors and answer questions posed, I calculated correlation coefficients using Power BI. The scatter plots and figures below illustrate the correlations:

 <img width="608" alt="2024-09-13 (10)" src="https://github.com/user-attachments/assets/204c374a-bd76-442a-a64a-68658b1c45bd">
 
 *Fig 1: Correlation Analysis*
 
The gauges on fig 1 show the **positive** correlation between movie attributes and key factors, with colors indicating strength: Burgundy (**very strong**), Pink (**moderate**), Orange (**weak**), and Blue (**very weak**). These visualizations alongside the scatter plots provide a quick overview of the relationships between key attributes.

*Insights*
- Budget is the primary driver of a movie's financial success, but not the sole factor.
- High ratings and engaging runtime can contribute to success, but offer no guarantees.
- Runtime significantly impacts both expenses and viewer ratings, requiring a delicate balance.
- Surprisingly, popularity has little to no significant impact on Profit.

Building on the correlation insights from Fig. 1, I delved deeper into the relationship between budget and profit. Fig. 2 and 3 present detailed analysis of how budget impacts profit, highlighting trends and patterns in movie production by production companies.

<img width="608" alt="2024-09-13 (11)" src="https://github.com/user-attachments/assets/e85beec1-3c9d-4aa3-9b8c-0aea07b1d52d">

*Fig. 2: Budget and Profit Analysis By Production Company*

<img width="612" alt="2024-09-13 (12)" src="https://github.com/user-attachments/assets/5f4d0be5-7fa7-4af9-9e43-bf30a7a39465">

*Fig. 3: A better view on 2020 financial Performance*

The visualizations in fig 2 and 3 reveal the complex relationship between budget and profit in the movie industry, showing trends, outliers, and key insights.
- Walt Disney stands out as the top earner in the UK and USA movie industries on average accumulated profit from 2010-2023, as shown in the column chart. 
- The bar and column charts reveal a correlation between bigger budgets and higher profits, but with a twist. Some companies with smaller budgets outperformed those with larger ones, suggesting that other factors like genre, marketing, and audience reception may play a significant role in financial success.
- Performance Over Time reveal a striking dip in profits and substantial losses in 2020, with Walt Disney among the companies hit hard, despite having large budgets. Some companies also had no budgets and revenues at all.

<img width="610" alt="2024-09-13 (13)" src="https://github.com/user-attachments/assets/7746b291-df0b-4236-9a93-82c63bf29574">

*Fig. 4: Budgeting Trends and Analysis by Movie Genre*


Building on the budget-profit analysis in Fig. 2 and 3, Fig. 4 explores genre-specific budgeting patterns and their impact on profit. The following findings were made:
- Top Genres by Average profit tend to attract more investments: Walt Disney dominates profit by investing significantly in top performing genres.
- Budgeting strategies, not just total spend, influence profit.
- In 2020 companies significantly reduced movie productions, as seen in the drastic drop in total production budgets.
- However, average budget per movie remained relatively stable, indicating focused investments in fewer, higher-quality productions.
- Post-2020, companies increased average budget per movie substantially, suggesting a strategic shift towards quality over quantity, likely in a bid to recover from the previous losses.












## Insights and Visualizations



## Referrences
- Movies main data obtained from asaniczka, (2024). Full TMDB Movies Dataset 2024 (1M Movies) (Data obtained from The Movie Database [TMDB]). Retrieved from [Kaggle](https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies/data)

- Popularity metrics obtained from TMDB Popularity Guides, (2024): Retrieved from [TMDB docs](https://developer.themoviedb.org/docs/popularity-and-trending#tv-shows)

- Movie Parent Company data obtained and clarified from Wikipedia. (n.d.). List of film production companies. Retrieved from [Wikipedia](https://en.wikipedia.org/wiki/List_of_film_production_companies)
