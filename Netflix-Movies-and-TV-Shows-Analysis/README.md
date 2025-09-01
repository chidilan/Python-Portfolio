# Netflix-Movies-and-TV-Shows-Analysis
## __Table of Contents__ ##
<ul>

[1. About the project](#about-the-project)

[2. About the dataset](#about-the-dataset)

[3. Tools and libraries](#tools-and-libraries)

[4. Phases of the project](#phases-of-the-project)

<ul>

  [4.1. Data Exploration](#1-data-exploration)

  [4.2. Data Cleaning](#2-data-cleaning)

  [4.3. Data Analysis and Visualization](#3-data-analysis-and-visualization)

</ul>

</ul>

<hr>

## __About the project__ ##
This project is a self-study project, its main objective is to help me practice on a real dataset and strength my analysis skills in Python.
<br>

It is about cleaning and analyzing Netflix movies and tv shows data, and getting insights about the countries where they were filmed, their ratings and release years.
<br>

The detailed notebook of the project is [here](Analyzing%20Netflix%20Data.ipynb).

<hr>

## __About the dataset__ ##
This project's dataset is an open-source data from __Kaggle__.
<br>

> You can find it [here.](https://www.kaggle.com/datasets/shivamb/netflix-shows)

<u>
The dataset contains one "csv" file which has 8807 entries with the following information:
</u>

* __Type__: Movie or TV Show
* __Title__: The name of the movie/tv show
* __Director__
* __Cast__: The names of the movie/tv show's cast
* __Country__: The country(s) which this movie/tv show was filmed
* __Date added__: The date when the movie/tv show was added on Netflix
* __Release year__
* __Rating__: Age-based media reviews
* __Duration__: The number of minutes for movies or number of seasons for tv shows
* __Listed in__: The category(s) which this movie/tv show is listed in
* __Description__: A sentence which describes this movie/tv show on Netflix

<hr>

## __Tools and libraries__ ##
This project was done in Python using Jupyter Notebooks.

The libraries used are:
* __Pandas and Numpy__: for exploration, cleaning and analysis
* __Matplotlib and Seaborn__: for visualizations

<hr>

## __Phases of the project__ ##
### 1. Data Exploration ###

<ul>

After reading the data, I have to explore it, its columns, and the info it contains. So, I've gained information about:

1. The dataset size
2. The datatypes of the columns
3. What each column represents
4. What are the information inside the categorized columns such as  __type__, __listed_in__, __rating__ and __country__.

</ul>

<hr>

### 2. Data Cleaning ###

<ul>

After exploring the data, I need to check it if there are any issues.

1. Search for duplicates
  
    * Fortunately, it has no duplicates.

2. Search for nulls

    2.1. Columns with few nulls

   * Solution 1: Get the missing information by searching for them
   * Solution 2: Drop them
    
    2.2. Columns with many nulls

    * Solution: I wasn't interested in those columns so we left them as they're

3. Change the incorrect datatypes into appropriate datatypes

</ul>

<hr>

### 3. Data Analysis and Visualization ###

<ul>

<u>
The questions we are interested to know are:
</u>

1. The percentage of movies and tv shows in this data

  <ul>
  
  <img src="visuals/MoviesVsTVShows.png" alt="Movies vs TV Shows" width="500"/>

  > The dataset has 71.35% of its entries movies and the rest are tv shows.
  
  </ul>


2. The growth of content creations over the years

  <ul>
  
<img src="visuals/ContentCreationGrowth.png" alt="Movies vs TV Shows" width="600"/>

  > The results shows that the year which has the highest number of content creations is 2018 which means that the data may be not complete.
  
  </ul>

3. Monitor content creations along the months
  <ul>
  
<img src="visuals/ContentCreatorsAlongMonths.png" alt="Movies vs TV Shows" width="600"/>

  > December is the month when the highest number of content occurs.
  
  </ul>

4. The oldest 10 tv series and movies
  <ul>
  
  4.1. The oldest 10 tv shows
  
<img src="visuals/oldest%20tv%20shows.png" alt="Movies vs TV Shows" width="500"/>

  4.2. The oldest 10 movies
  
<img src="visuals/oldest%20movies.png" alt="Movies vs TV Shows" width="500"/>

  </ul>

5. The highest 10 countries contributed in contect creation
  <ul>
  
<img src="visuals/CountriesContributed_in_MoviesCreationTop10.png" alt="Movies vs TV Shows" width="500"/>
  
  > United States is the top 1 country contributed in both movies and tv shows
  
  </ul>
  
6. The most frequenct categories
  <ul>
  
<img src="visuals/TopMovieCategoriesPieChart.png" alt="Movies vs TV Shows"/>

  </ul>

7. Number of movies and tv shows by MPA rating for top 10 MPA ratings
  <ul>
  
<img src="visuals/ContentCreations_ByTop10MPARatings.png" alt="Movies vs TV Shows"/>

  </ul>

</ul>

<hr>