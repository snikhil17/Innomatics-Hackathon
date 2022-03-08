# About Dataset:
- This dataset contains information about the top 1000 highest grossing hollywood films. It is up to date as of 10th January 2022.
- This data has been scraped from multiple sites and has been added together for performing various data operations. The data has been taken from imdb, rotten tomatoes and many other sites.

# Approach and Analysis performed:
## Impute missing values in Release Date:
- YEAR: Title of the movie contained Year, there were 1.7 % miss matching in year from title and year from Release date (rows where missing values weren't there). Hence i considered to replace year with year value.
- MONTH: I grouped the data using Distributors and then calculated used the median of months. Idea was that Distributors (say Warner Bros.) releases movies in specific months.
- Day: i just used 1 here.
##  Impute missing values in License:
- Grouped the data using Distributor then calculated the mode of License and replaced accordingly.

## Feature Engineering:
- Converted Sales from $ to million $
- Convert Movie Runtime from 2h 36m to 2.36
- Keep only 4 genres (in separate columns), if movie doesn't have 2 or more genre use 1st genre.

## Exploratory Data Analysis:
- Top 10 Worldwide Selling Movies
- Comparison of Sales w.r.t Genres
- Movies Released month-year Analysis
- Movies Released Month-Distributer Analysis
- Distributor and Duration relation
- License-Distributor Analysis
- Number of movies Released over years
- Word Clouds of Genre

## Tableau Dashboard [Link](https://public.tableau.com/views/MoviesDataAnalysisHackathon/MoviesDataAnalysis?:language=en-US&:display_count=n&:origin=viz_share_link)
- Top N Distributor w.r.t Worldwide Sales
- Worldwide Sales calendar for Nth Year
- Domestic and International Sales over Numerous Years
- Tags showing change in Domestic, Independent and Worldwide sales.
