# Analysis on Promotion of Intangible Wood-Carving Culture Heritage
@Author: Fangze Sun

## Goal
- To analyze the promotion and dissemination of intangible wood carving culture heritage on Chinese social media platform.
- To investigate the growth trend of public's attention to intangible wood carving culture heritage.
- To explore the recommendation mechanism of the video platform for specific culture.

## Data Set
- **Data Source**: Developed a **reusable scraper** algorithm to crawl the data from Bilibili, a Chinese video platform.
- **Data Description**: 424 wood carving culture heritage videos posted by 269 video authors, including general video information (title, pulished date, and author, etc.) and audience interaction data (likes, coins, and shares etc.).

## Repo Structure
```
|-- README.md                                              <- You are here
|-- Data_Analysis_on_WoodCarving_Culture_Heritage.ipynb    <- Jupyter Notebook containing scraper, data cleaning, feature engineering, visualizations
|-- requirements.txt                                       <- Python package dependencies
```

## Data Cleaning & Feature Engineering
- Cleaned the raw data by filtering irrelevant contents, detecting abnormal values, dropping duplicates, standardizing units, and unifing data types.
- Generated new features based on existed variables, including "published year" and "publish month" for later analysis on peak periods of wood carving culture promotion.
- Calculate "recommend rate" based on metrics of audience interactions and the platform recommend algorithm.

## Exploratory Data Analysis
- Applied **Plotly interactive scatter plot** to visualize **"The Relationship Between Likes/Views/Coins and Video Duration"** for all wood carving culture videos.
- Detected the **"Top 10 Video Authors of Wood Carving Culture Heritage Vidoes"**, using **Plotly bar chart** to see who are promoting this niche culture, and identified the **influencial levels of these authors** by calculating average likes of their videos.
- Explored **Annual Growth Trend of Wood Carving Culture Heritage Videos** by counting the number of videos posted each year, and **investigated the seasonalnality of wood carving making**.
- **Evaluated the recommendation rate** of wood carving culture heritage videos based on Bilibili recommendation algorithm.
- Conducted **text analysis** on video titles using *jieba* package to **generate corpus**, and **created bi-grams to find the most frequent key words** in wood carving videos.
- **Explored the commercialization level** of intangible wood carving culture to see its possibility of entering the market.
