# Predicting IMDb rating

The goal of this project is to try and build a prediction model for the IMDb rating score for movies of this century.
This project is divided into 6 jupyter notebooks:
1. web_scraping_part1: Scraping informations about the movies from the search-result pages of the imdb website
2. cleaning_part1: Dealing with missing values in this first webscraped informations
3. web_scraping_part2: Scraping more information about the same movies from each movie webpage
4. cleaning_part2: Merging the scraped informations and more cleaning of the data
5. analysis_and_viz: Descriptive analysis of the data and some data visualisation
6. regression: Regression models

## Data

Here is the list of features scraped for each movie: 
_(features used in the regression model are **bold**)_

* movie: title of the movie
* **year**: release date (2000 to 2020)
* imdbID: format '/title/tt......./': extension of imbd.com url for each movie with unique 7 digits ID 
* certificate: rating certificate (R, PG-13, etc...)
* **genre**: list of genres corresponding to the movie
* **runtime**: in minutes
* **rating**: imdb rating (from 1 to 10): **target of the regression models**
* **metascore**: rating score from the website [Metacritic.com](https://www.metacritic.com/)
* **director**: director of the movie
* **votes**: number of votes on IMDb website
* gross: how much the movie made at the box office
* **stars**: list of 3 top actors staring in the movie
* **writer**: name of the writer
* popularity: indicates how much a movie’s page has been visited in the current week on IMDb in it’s area of interest
* **plot_keywords**: list of top 5 plot keywords by relevance
* **languages**: list of languages for the movie
* **country**: country for the movie
* budget: budget of the movie
* **cum_worldwide_gross**: cumulative worldwide gross: how much the movie made at the box office worldwide


## Regression Models

The models tested on the data are:
* Linear Regression
* k-Nearest-Neighbors
* Decision Tree
* Random Forest

## Tools

* Python
* Numpy
* Pandas
* requests
* BeautifulSoup
* Matplotlib
* Seaborn
* sklearn


