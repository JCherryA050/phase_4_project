# MyAnimeList Recommendation
![MALlogo](./imgs/myanimelist.png)

## Overview

My Anime List (MAL) is a fan-based website where users can track and rate the anime or manga that they watch. MAL contains a lot of details about anime and mange as well as reviews and ratings from almost half a million users. With all this information, MAL has a global ranking of anime/manga, a recommendation system based on users preferences, and directs users to where they can watch or read a given anime/manga.

## Business Problem

Since MAL is a fan-based website, we have been tasked to develope a more effective recommendation system using our expertise in machine learning. 

## Data

Our dataset is made available by Kaggle.

**Note**: the dataset is too large to be uploaded on github.  
Here are steps to acquire the dataset in order to make our codes work:
- Download the data from Kaggle. Click this [link](https://www.kaggle.com/hernan4444/anime-recommendation-database-2020). The files that we will be using are "anime.csv" and "animelist.csv".
- Create a folder called "data" and place the files in it.
- Make sure that the paths for the files look like this: "data/anime.csv" and "data/animelist.csv".

The dataset was scraped directly from My Anime List in March 2021. It contains over 109 million reviews from over 325000 users with approximately above 17000 anime titles. The rating reviews score between 1-5 stars (5 is the best) with is translated to 10 points scale. The metadata also contains key features such as Genre, Popularity, English name, and Score.

## EDA

The distribution of rating is quite normal (with mean ~ 7 and std ~ 0.9)

![rating_graph](./imgs/rating_dist.png)

## Methodology

We begin our methodology with filtering data down to more manageable size. We remove unrelated and unsavory genres such as 'Musical', 'Movie','OVA', 'Special', 'ONA', and 'Hentai.' We choose to build our recommendation system using collaborative filtering algorithm. There are two libraries that provide useful built-in machine learning models: ALS from PySpark; SVD from Surprise. These are two models that we rely on heavily.  


## Results

words

## Conclusions

words

## Next Steps

words
 
## For More Information

See full analysis in [Jupyter Notebook](./project_four_code.ipynb) or check out this [presentation](./project_four_presentation.pdf). 
For additional info, please contact:  
Ramil Chaimongkolbutr at [ramil.ming@flatironschool.com](mailto:ramil.ming@flatironschool.com)  
George Ferre at [georgeaferre@flatironschool.com](mailto:georgeaferre@flatironschool.com)  
Aaron Cherry at [cherrya050@flatironschool.com](mailto:cherrya050@flatironschool.com)


## Repository Structure

```
├── data
├── imgs
├── README.md
├── project_four_presentation.pdf
└── project_four_code.ipynb
```
