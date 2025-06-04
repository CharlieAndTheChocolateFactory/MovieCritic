# Movie Data Analysis with R

This project uses R to analyze and visualize movie data, including IMDb ratings, Rotten Tomatoes scores, release years, and awards/nominations. Data is scraped from IMDb and OMDb API, with additional random sampling from a Kaggle dataset.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Data Sources](#data-sources)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Notes](#notes)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

This R script gathers, cleans, and analyzes movie data from various sources. It compares "hero" movies to random and top IMDb movies, examining relationships between ratings, awards, release years, and more with informative plots and linear regressions.

## Features

- Scrape IMDb lists and extract movie IDs
- Query OMDb API for detailed movie data (title, director, ratings, awards, etc.)
- Analyze and visualize:
  - IMDb rating vs. total nominations/awards
  - Rating trends over release years
  - Rotten Tomatoes score relationships
- Easily extendable for other datasets or types of movies

## Data Sources

- **IMDb**: Movie IDs and lists ([IMDb Top 250](https://www.imdb.com/chart/top/))
- **OMDb API**: Movie details ([OMDb API](http://www.omdbapi.com/))
- **Kaggle**: Random sampling from a dataset of movies with >20,000 votes
- **Rotten Tomatoes**: Scores via OMDb API

## Installation

1. **Clone this repository**  
   ```sh
   git clone https://github.com/yourusername/movie-data-analysis.git
   cd movie-data-analysis
2. **Install Required R Packages**
   Open R or RStudio and run:
   install.packages(c("rvest", "stringr", "dplyr", "lubridate", "gutenbergr",
                   "tidytext", "textdata", "ggplot2", "httr", "tidyr"))
3. **Obtain OMDb API Key**
   Register for a free key at OMDb API and add it to the script:
    api_key <- "YOUR_OMDB_API_KEY"
4. **Prepare Data Files**
   - Download and place movieID.csv (from Kaggle) in your working directory.

## Usage 
1. Run the script
- You can run the R script in chunks or all at once (recommended in RStudio).

2. What the script does

- Scrapes IMDb for hero and top movies.
- Fetches movie details from OMDb API.
- Cleans and merges data.
- Performs analysis and creates plots, such as:
- IMDb Rating vs. Awards
- Rating/score vs. Year
- Rotten Tomatoes vs. Nominations

.
├── README.md
├── movie_analysis.R         # Main R script (your file)
├── movieID.csv              # Movie IDs from Kaggle
└── (other files...)

##  Notes
- API Limits: OMDb API has a daily request limit for free users.
- This is a school project of COMP2501

