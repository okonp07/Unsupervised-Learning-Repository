# 2201ACDS_NM2 Unsupervised Learning  - Movie Predition

## Project Overview

A recommendation system is a subclass of Information filtering Systems that seeks to predict the rating or the preference a user might give to an item. In simple words, it is a system that uses a machine learning algorithms that suggests relevant items to users. There are two main types of recommender systems – personalized and non-personalized. Non-personalized recommendation systems like popularity based recommenders recommend the most popular items to the users, for instance top-10 movies, top selling books, the most frequently purchased products etc.

In today’s technology driven world, recommender systems are socially and economically critical to ensure that individuals can make optimised choices surrounding the content they engage with on a daily basis. This is made possible by personalized recommendation systems. One application where this is especially true is movie recommendations; where intelligent algorithms can help viewers find great titles from tens of thousands of options that is suited to their individual preference.

In this unsupervised learning challenge, our team is to develop a recommendation algorithm based on content or collaborative filtering, capable of accurately predicting how a user will rate a movie they have not yet viewed yet, based on their historical preferences. Providing an accurate and robust solution to this challenge has immense economic potential. Users of this system will be providede with personalised recommendations - generating platform affinity for the streaming services which best facilitates their audience's viewing.

## Team Members and Supervisor

Below is the list of all the members of this team who are to participate in this project. At the time of generating this repository, they are all students at EXPLORE Data Science Academy.

- Prince Okon
- Adewale Daniel Odukoya
- Huzaifa Abu 
- Izunna Eneude
- Jerry Iriri

**Supervisor: Nomfundo Manyisa**

## Project Aim

To build a Machine Learning model that uses the historical data of a movies viewed by an individual to predict the rating that they will assign to movies that they haven't seen yet.

## Data Details

The dataset consists of several million 5-star ratings obtained from users of the online MovieLens movie recommendation service. The MovieLens dataset has long been used by industry and academic researchers to improve the performance of explicitly-based recommender systems. The data used for this project is a pre- enriched version of the MovieLens dataset which has been cleaned, and resampled for fair evaluation purposes.

### Data Source

The data for the MovieLens dataset is maintained by the GroupLens research group in the Department of Computer Science and Engineering at the University of Minnesota. Additional movie content data was legally scraped from IMDB.

### Supplied Data Files
genome_scores.csv - a score mapping the strength between movies and tag-related properties. Read more here
genome_tags.csv - user assigned tags for genome-related scores
imdb_data.csv - Additional movie metadata scraped from IMDB using the links.csv file.
links.csv - File providing a mapping between a MovieLens ID and associated IMDB and TMDB IDs.
sample_submission.csv - Sample of the submission format for the hackathon.
tags.csv - User assigned for the movies within the dataset.
test.csv - The test split of the dataset. Contains user and movie IDs with no rating data.
train.csv - The training split of the dataset. Contains user and movie IDs with associated rating data.

### Ratings Data File Structure (train.csv)

All ratings are contained in the file train.csv. Each line of this file after the header row represents one rating of one movie by one user, and has the following format:

**userId,movieId,rating,timestamp**
The lines within this file are ordered first by userId, then, within user, by movieId.

Ratings are made on a 5-star scale, with half-star increments (0.5 stars - 5.0 stars), giving 10 rating categories in all.

Timestamps represent seconds since midnight Coordinated Universal Time (UTC) of January 1, 1970.

### Tags Data File Structure (tags.csv)
All tags are contained in the file tags.csv. Each line of this file after the header row represents one tag applied to one movie by one user, and has the following format:

userId,movieId,tag,timestamp
The lines within this file are ordered first by userId, then, within user, by movieId.

Tags are user-generated metadata about movies. Each tag is typically a single word or short phrase. The meaning, value, and purpose of a particular tag is determined by each user.

Timestamps represent seconds since midnight Coordinated Universal Time (UTC) of January 1, 1970

### Movies Data File Structure (movies.csv)
Movie information is contained in the file movies.csv. Each line of this file after the header row represents one movie, and has the following format:

movieId,title,genres
Movie titles are entered manually or imported from https://www.themoviedb.org/, and include the year of release in parentheses. Errors and inconsistencies may exist in these titles.

Genres are a pipe-separated list, and are selected from the following:

-Action
-Adventure
-Animation
-Children's
-Comedy
-Crime
-Documentary
-Drama
-Fantasy
-Film-Noir
-Horror
-Musical
-Mystery
-Romance
-Sci-Fi
-Thriller
-War
-Western
-(no genres listed)

### Links Data File Structure (links.csv)
Identifiers that can be used to link to other sources of movie data are contained in the file links.csv. Each line of this file after the header row represents one movie, and has the following format:

movieId,imdbId,tmdbId
movieId is an identifier for movies used by https://movielens.org. E.g., the movie Toy Story has the link https://movielens.org/movies/1.

imdbId is an identifier for movies used by http://www.imdb.com. E.g., the movie Toy Story has the link http://www.imdb.com/title/tt0114709/.

tmdbId is an identifier for movies used by https://www.themoviedb.org. E.g., the movie Toy Story has the link https://www.themoviedb.org/movie/862.

Use of the resources listed above is subject to the terms of each provider.

### Tag Genome (genome-scores.csv and genome-tags.csv)
As described in this article, the tag genome encodes how strongly movies exhibit particular properties represented by tags (atmospheric, thought-provoking, realistic, etc.). The tag genome was computed using a machine learning algorithm on user-contributed content including tags, ratings, and textual reviews.

The genome is split into two files. The file genome-scores.csv contains movie-tag relevance data in the following format:

movieId,tagId,relevance
The second file, genome-tags.csv, provides the tag descriptions for the tag IDs in the genome file, in the following format:

tagId,tag

### Jupyter Note book File (Project Base file)

The jupyter notebook in this repository is a detailed documentation of the technical steps taken to complete the defined task in this project. The notebook in this repository is the Base jupyter notebook, on which we shall rely to generate and update submissions of our models performance on Kaggle.

This file will be worked on and improved upon by all team members with the aim of reaching the goals and accomplishing the tasks set out as the goals of the project outlined. By Taking into account the contributions of all team members, we shall hopefully generate a final model which will perform best at recomending movies for individual viewers based on their past preferences.

### How to work on the base file as a Collaborator

All teammates have been added as collaborators in the project on Kaggle. Due to the sheer size of the data to be processed it is highly reccommended that all the work on this project be done mainly on the kaggle kernel platform. This is because most personal computers will lack the computational resources required to carry out the processing of this data in a timely and efficient manner.

### Dependencies

Note that the dependencies required for the notebook to run must be installed in personal machines before the jupyter file runs as it should. Note that some of theses dependencies may not install with a simple pip command as you might expect and may have to be installed via anaconda prompt or other command line interfaces. You may use google, stack overflow and other online resources to install and update the dependencies whenever you need to. These dependencies usually are requisite for the execution of the jupyter notebook.

### Resources

It will be beneficial to rely on the materials provided by Explore Data Science Academy on their learning platform, but it is also recommended that collaborators conduct personal research to supplement the information provided on Athena. Please make use of these resources and keep this readme file updated with relevant links to materials that may be useful to our work.

### Others

Refer to our teams Trello board for details on tasks assigned to specific teammates, progress reports and other updates.

- [Trello Board](https://trello.com/b/Lq21ugZq/teamnm2-movie-rating-prediction)

Refer to the kaggle leader board to access details on the teams performance on the ongoing Kaggle challenge

- [Kaggle Challenge](https://www.kaggle.com/competitions/edsa-movie-recommendation-2022/overview))

Refer to the presentation slides, by clicking on

- [Presentation Slides](https://docs.google.com/presentation/d/1oje2X49-cpqEB-631jv8q_7wyJrGES3cDbGoR1G2MAs/edit)
