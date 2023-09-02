# Netflix_Movies_TV_Show_Clustering
![netflix-netflix-startup](https://github.com/akeelrashid/Netflix_Movies_TV_Show_Clustering/assets/121357205/e29d85f6-e98e-4bf3-b088-bc5de19c2f06)

This repository contains the code and resources for analyzing the Netflix dataset of movies and TV shows until 2019. The dataset was sourced from the third-party search engine Flixable and includes information about various attributes of the content available on Netflix. The goal of this project is to uncover insights, trends, and patterns within the dataset and develop a content-based recommender system using natural language processing (NLP) techniques.

## Problem Statement
The problem at hand involves exploring the Netflix dataset to gain insights into the content available on the platform. The dataset provides information about movies and TV shows, their attributes, and their availability in different countries. By integrating this dataset with external sources such as IMDB ratings and Rotten Tomatoes, we can extract further valuable information.

The specific tasks to be performed in this project include:
* Exploratory Data Analysis (EDA): Cleaned the data, unnested the Netflix content and tackled the null/missing values and conduct a thorough analysis of the dataset to uncover trends, patterns, and correlations among different attributes.
* Understanding Content Availability: Determine the types of content available in different countries and identify any variations or preferences.
* Analyzing Netflix's Focus: Investigate whether Netflix has been increasingly focusing on TV shows rather than movies in recent years.
* Clustering Similar Content: Utilize text-based features to cluster similar content, enabling the development of a content-based recommender system.

## Project Summary

# Netflix Content Analysis Project Summary

## Problem Statement:

This project revolves around a dataset containing TV shows and movies available on Netflix as of 2019, collected from Flixable, a third-party Netflix search engine. In recent years, Netflix has experienced a significant shift, with the number of TV shows nearly tripling while the number of movies has decreased. The objective is to uncover valuable insights from this dataset and explore its potential integration with external datasets, such as IMDB ratings and Rotten Tomatoes.

## Project Summary:
I aim of this project is to analyze a dataset containing TV shows and movies available on Netflix as of 2019, obtained from Flixable, a third-party Netflix search engine. The dataset comprises 7,787 rows and 12 columns, with no duplicate values. However, several features had missing values. The dataset provides valuable information about content type (TV show or movie), title, director, cast, country of production, date added to Netflix, release date, duration, rating, and description

The project follows a step-by-step process, as outlined below:

###  Handling Missing Values:
Address any null or missing values present in the dataset.
### Dealing with Nested Columns: 
Process nested columns such as director, cast, listed_in, and country to facilitate clear visualization and analysis.
### Rating Binning: 
Categorize ratings into appropriate categories, including adult, children's, family-friendly, and not rated content.
### Exploratory Data Analysis (EDA): 
Perform in-depth EDA on various attributes, uncovering valuable findings to aid in churn prevention.
### Cluster Creation:
Create clusters using attributes such as director, cast, country, genre, rating, and description. Tokenize, preprocess, and vectorize the attribute values using TF-IDF vectorizer.
### Dimensionality Reduction:
Reduce the dimensionality of the dataset using Principal Component Analysis (PCA) to improve performance.
### Clustering Algorithms: 
Employ K-Means Clustering and Agglomerative Hierarchical Clustering algorithms to construct two distinct types of clusters. Determine the optimal number of clusters using methods like the Elbow method, Silhouette score, and Dendrogram.
### Content-Based Recommender System:
Develop a content-based recommender system using the cosine similarity matrix. This system analyzes the user's watched shows and generates personalized recommendations to enhance their experience.

# EDA Conclusion
- Movies account for approximately 69.1% of the content, while TV shows make up about 30.9%.
- Content is primarily suitable for adults and teenagers, with no content rated for general audiences in TV shows.
- Most movies have a duration of 90 to 120 minutes, and TV shows predominantly have a single season.
- Content additions to Netflix increased significantly after 2015, with peaks in November 2019 for both TV shows and movies.
- Content is frequently added on the 1st and 15th of each month.
- There has been a consistent increase in content releases, particularly after 2008, with notable drops in 2018 and 2020.
- International movies and TV shows are the most popular genres, followed by dramas and comedies.
- The USA leads in content production, followed by India and the United Kingdom.
- Notable directors include Jan Suter, Raul Campos, Jay Karas, Alastair Fothergill, and Ken Burns.
- Famous cast members include Anupam Kher, Shah Rukh Khan, Naseeruddin Shah, Takahiro Sakurai, Yuki Kaji, and Daisuke Ono.
- Most top countries produce adult-related content, except India, which produces more content suitable for teenagers.
- Frequent words in descriptions include family, friend, life, find, two, take, world, woman, live, and love.

# ML Conclusion:
- I implemented K-Means and Hierarchical Agglomerative clustering to cluster the dataset.
- K-Means with 5 clusters was selected as the final model due to well-defined clusters and a high Silhouette score.
- The Silhouette score served as the evaluation metric, indicating cluster quality.
- Additionally, I developed a recommendation system for personalized content recommendations based on similarity scores.












