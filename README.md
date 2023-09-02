# Netflix_Movies_TV_Show_Clustering

![netflix-netflix-startup](https://github.com/akeelrashid/Netflix_Movies_TV_Show_Clustering/assets/121357205/df5d6b04-bf89-49e8-82a9-b0e6e7685c2a)


## Problem Statement
This dataset consists of tv shows and movies available on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine.In 2018, they released an interesting report which shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has nearly tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

Integrating this dataset with other external datasets such as IMDB ratings, rotten tomatoes can also provide many interesting findings.

In this project you require to do
1. Exploratory Data Analysis

2. Understanding what type content is available in different countries

3. Is Netflix has increasingly focusing on TV rather than movies in recent years.
4. Clustering similar content by matching text-based features

5. ## Project Summary
6. I have been given a dataset which consists of **Tv shows and Movies available on netflix** as of 2019 which was collected from Flixable which is a third party netflix search engine.My task is to **explore** the data in order to find some useful insights.Try to understand what type of **content** is available in **different countries** and has to develop a **Clustering model** based on matching text-based Feature.The dataset provides us information regarding type of content whether **Tv shows or Movies** that has been added on Netflix.It provides information like **Title,Director,cast** of the Tv show/Movie and **Country** where Movie/Tv show was produced.When was it added on Netflix,what is the **release date,duration,rating and Description** of Movie/Tv Show.

After importing the dataset in my colabnote book.it was find out that 
the dataset consists of **7787** rows and **12** and the dataset **doesn't** contain any **duplicated** values but there are many features in dataset which **contains null** values like  **director** feature has maximum null vlaue around **30.68%**,followed by **cast 9.22%** ,**country 6.51%**,**date_added 0.13%** and **rating 0.09%**.I treated all the null values present in my dataframe,then i created some new column from the existing columns.

Then i performed **EDA** in order to find useful insights from the data and after that i performed **Textual Data Preprocessing** where i created new feature **filtered** using some important columns.Then i performed different method like **Lower casing**,**removed punctuations**,and **URLs**,**stops words**,**Lemmatization**,**Text Vectorization** and then performed Dimension reduction using **PCA**.

After that i implemented **K-Means** and **Hierarchical Agglomerative** clustering to cluster the dataset based on similarity with **Sihouette score** as evaluation metrics.At the end i have Built a **Recommendation system** that can help in providing Netflix users personalized recommendations based on their similarity scores.

## EDA Conclusion

* There are more  **Movie** realted content i,e around **69.1** and **Tv show** content is less i,e **30.9**  in the dataset
* Most of the content in the Netflix is suitable for **Adults** and **Teenagers** and also in TV Show there is no content for **General Audience**
* Most of the movies has duration of around **90 to 120 minutes** and most of the TV shows has only **1 Season**.
* After **2015** large number of Tv Shows were added on the platform.In **Nov 2019** maximum Tv show content was added to the platform.
* Similarly after **2015** large number of Movie content was added to the platform and in  **Nov 2019** maximum content was added.
* On **1st** and **15th** of every month maximum content both TV shows and Movies was added to the platform
* TV Show and Movie content release has been increased over years and after **2008** more number of movies and TV shows were released and it can be also seen that after **2018** and **2020** there were large drop in release of Movies and TV shows respectively
* **Internation Movies and TV shows** are most popular genres in Tv show and 
 in Movies followed by **Dramas** and **Comedy**
* **USA** is the top content Producing Country followed by **India** and **United Kingdom** in overall and also in **Movies** related Content
* **USA** also produces more **TV series** followed by **United Kingdom**,**japan**
* **Japan**,**South Korea** produces more **TV Shows** than **Movies**
* **Jan Suter** followed by **Raul Campos,Jay Karas** has directed maximum Movies and **Alastair Fothergill** and **Ken Burns** has directed maximum TV Shows
* **Anupam Kher**,**Shah Rukh Khan**,**Naseeruddin Shah** etc are famous Movie Cast and **Takahiro Sakurai, Yuki Kaji,Daisuke Ono** etc are famous TV Show cast
*  Almost **all top countries** produced more **adult** related content except **india** produce more **Teenagers** content
* It was seen that word like **family,friend,life,find,two take,worldwoman,woman,live,love** etc are most frequent words used in the description

* ### ML Conclusion

* I have implemented **K-Means** and **Hierarchical Agglomerative** clustering to cluster the dataset
* I have consider **K-means** 5 optimal number of cluster as my final Model.K-means give me better result with well separated clusters and high Sihouette score,so K-means algorithm was able to effectively capture the underlying structure and patterns in the data
* I have consider **Sihouette score** as my evaluation metrics.
The Sihouette score gives us the measurement of how close each sample in one cluster and far from neighbouring cluster.It takes into account both the cohesion (similarity within a cluster) and the separation (dissimilarity between clusters) of the data points.Sihouette score ranges from (-1 to 1),a higher Silhouette score indicates better-defined and well-matched clusters, while a lower score suggests overlapping or poorly matched clusters
* At the end i have Built a **Recommendation system** that can help in providing Netflix users personalized recommendations based on their similarity scores.
