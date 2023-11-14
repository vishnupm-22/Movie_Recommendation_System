## **MOVIE RECOMMENDATION SYSTEM**
**Problem Statement**:
* Develop a content-based recommendation system using cosine similarity that suggests similar movies based on input provided by the user.


**Steps** :
* Understanding the data
* EDA
* Text Preprocessing
* Text Vectorization
* Model Building

Used kaggle 'TMDB 5000 Movie Dataset'.Movie dataset contains 20 features such as budget,genre,keywords etc is merged with Credit dataset contains 4 features on the basis of 'title' and 'id'.

**Did exploratory data analysis to gain some insights on data**:
 * Extracted and visualized Top Movies based on popularity,Top Blockbuster Movies and flop movies based profit/loss,Top movies based on imdb rating,Distribution of Movies by IMDb Rating Category,Count Plot for Range of Votes,Count Plot for number of Profit and loss movies
 * Formatted the genre,keywords,cast & crew .Extracted the top movie genres ,Top 10 popular actors based on cast,Top 10 directors based on crew etc.

Created 'tags' using these features ('overview','genres','keywords','cast' & 'director').
These features helps in categorizing and represents the characteristics of each movie, making it easier for the recommendation system to analyze and suggest similar movies to users.

**Text preprocessing and Text Vectorization**:
 * lowercasing the data ensures that the same word in different cases is treated as a single token.
 * To make text analysis efficient different inflected forms of a word in data  mapped to a common root word.
 * Used Count Vectorizer method  for creating a Bag of Words (BoW) representation of text. data.
 
**Model Building**:
 * Applied cosine similarity to compute similarity as the normalized dot product of vectors.
 * sorted the similarity scores and extracted top 5 movie recommendations for the given input.



