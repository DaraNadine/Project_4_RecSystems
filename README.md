# Spotify’s Movie Division Algorithm(Reccomendation System)

# Business Problem
 Spotify is launching a new Movie Divison. We are contracted Data Scientist tasked with creating a reccomendation system  for their new movie stream service. We want to compete with other streaming platforms such as Netflix, Hulu, Amazon Prime. Since they are new to the market, they want to ensure that their Reccomendation System is accurate and reliable. So we are building a model that reccomends the top 5 movies to a user based on their ratings on other movies. It can be hard as a user trying to sort out what to watch when given so many options. Many people have experience something refered to as "Streaming fatigue". That feeling of burnout when faced with so many choices when looking for original content to watch. So with our algorithm. We will address that. 



# Data Preparartion
Our data comes form the MovieLens Data set.https://grouplens.org/datasets/movielens/. This dataset consist of 102,377 rattings. These ratings range from 0.5 stars to the highest being 5 stars. This data came in several CSV files which would have to be merged into one Pandas Dataframe. The MovieID(movies.csv) file contains the movie title, associated genre as well as the specific unqiue movie ID number. Ratings(ratings.csv) contained the userId of the reviewer as well as the associated movie movie ID as well as the user rating of the movie and the timestamp(seconds since midnight Coordinated Universal Time (UTC) of January 1, 1970). Tags(tags.csv) contained userID, movieID, timestamp and tag. The tag column is user-generated metadata related to the mvoie. A short word or phrase associated with each movie. Links(links.csv) contained movieID,  imbld, and tmbld. Imbld and tmbld are identifersfor each movie used by  http://www.imdb.com and https://www.themoviedb.org. When merging all the datasets together we decided to not merge in the links dataset due to it's non relevance to the business problem. In additon we opted not to utilize tags. As the most relevant tag was 'In Netflix queue" which did not add much in terms of value and applying to our business probelm. In addiiton we elimated any duplicates in our data as well as converted timestp to datetime format. 


# Modeling
![image](https://i.imgur.com/RkNXafC.png)
![image](https://i.imgur.com/7yLMe0b.png)
# Conclusion
