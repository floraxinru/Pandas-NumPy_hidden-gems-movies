# hidden-gems-movies

A mini-project exploring movies of the MovieLens dataset that have high ratings but low popularity. Completed as part of the Python for Data Science MOOC on edx.

Main tools used: 
##### Python, Pandas, NumPy, Matplotlib, JupyterNotebook

## Motivation
As a movie lover, I am always on the lookout for high-quality independent movies. For this project, my goal is to find the “hidden gems” in the MovieLens dataset. 
These are defined as movies with a low number of user ratings (which implies they are not well-known, likely because they weren’t released at large cinema chains and only reached a limited audience), but a high average rating. 
Furthermore, I would also like to find out the proportion of each genre in these titles (using a pie chart) - my hypothesis is Romance movies will take up the largest proportion, but I would like to test that.

Insights from this study would be valuable for movie industry professionals for finding good movie directors and small-scale productions to invest in, for film festival organizers and independent cinemas to expand their line-ups by-genre, and also for independent movie fans like me!

## Dataset
The movielens dataset was provided by the MOOC instructors. The dataset has six files, with a total size of 18.6 MB. It is publicly available for download at <http://grouplens.org/datasets/>.

From the README file of the movielens dataset:

> This dataset (ml-20m) describes 5-star rating and free-text tagging activity from [MovieLens](http://movielens.org), a movie recommendation service. It contains 20000263 ratings and 465564 tag applications across 27278 movies. These data were created by 138493 users between January 09, 1995 and March 31, 2015. This dataset was generated on March 31, 2015, and updated on October 17, 2016 to update links.csv and add genome-* files.

> Users were selected at random for inclusion. All selected users had rated at least 20 movies. No demographic information is included. Each user is represented by an id, and no other information is provided.

> The data are contained in six files, `genome-scores.csv`, `genome-tags.csv`, `links.csv`, `movies.csv`, `ratings.csv` and `tags.csv`. More details about the contents and use of all these files follows.

 
## Research Questions
* What are the highly-rated but unpopular “hidden gems” titles from this movie dataset?
* Among these movies, what proportion does each genre take up?
  * Is Romance indeed the most numerous category of these movies?

## Findings

The research questions I set out to explore where answered, since I found the 313 titles that are highly rated (mean rating less than 4.0) and are unpopular (number of ratings fewer than the mean number of ratings, 747). 
I also found the proportion taken up by each genre, and the pie chart shows Drama and Comedy are the two genres with the most titles, with Romance coming third instead of first (see moviepie2.png).

A possible improvement would be to adjust the filter requirements so that more titles are included, as well as looking at tags in addition to genres of movies. 
I am also interested in doing a more thorough analysis on a larger dataset, with more internaitonal titles.
 
## Installation and Usage
Download the .csv data files from the Movielens movie dataset, as well as requirements.txt.
Install the requirements for this project using `pip install -r requirements.txt.` This will install the exact version of the libraries that I had when doing this project.
