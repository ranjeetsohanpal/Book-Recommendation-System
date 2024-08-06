# Book Recommendation System

## About the project 

* This project gives recommendations based on the title of the book given as input.
* It shows 4 books which are most related to the input book title.
* You can also find the 50 most popular books which pass the condition of certain number of votes.

### Dataset
* The following dataset has been used to build this project :[Book Recommendation Dataset](https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset)
* The dataset consists of 3 .csv files :
  1. Books.csv : This contains all the infomation about the books(ISBN, Title, Author, Year, Image of cover
  2. Ratings.csv : This contains the ratings given by user for a book. The ratings lie between **0-10**.
  3. Users.csv : This contains the user IDs, location and age.

### Methods used

1. Recommendation System :
      * This project employs the use of **Collaborative Filtering** which uses the ratings given by other users to recommend titles. 
      * It calculates the similarity of any two books based on cosine similarity(which is basically the norm of two vectors in space).
      * Hence for every book, we will show 4 books which have the highest cosine similarity except itself. These books will be recommended to the user.

  

2. Top 50 popular books :
   * For showing the top 50 books, we will sort the books firstly on the basis of ratings.
   * The books to be shown must have voting count above the certain threshold given in the *notebook*. In this project, the threshold is 250 votes.
   * In the end, the filtered books are sorted by ratings in desceding order.


## Further Plans
* Since the user can only enter the books which are present in the dataset as it is, this leads to difficulty in usage. This problem could be solved by improving the search engine.
* Show the book searched too before the recommendations.
* Include more books which are available on Amazon by webscraping.
* Try content based filtering too!!
