
# Study Guide For Midterm

- The exam covers material from homeworks 1 (SQL) and 2 (Algorithms).  It does not cover material from the unit on machine learning.  
- Review the homeworks.  For homework 2, in particular, you might notice that in several of the questions I ask you about some algorithms but not others.  Thus, one study hint would be to revisit those questions and apply the question to other algorithms that you've learned about.  For example, what is the best and worst case runtime of SentinelLinearSearch?
- Review the lecture notes.  The relevant lectures are Lectures 4-13.
- Revisit the readings, especially the Boat book, *Algorithms Unlocked*, and any other technical readings from the relevant lectures.


## Additional SQL queries

You can try out these queries on the MovieRatings database available on [JackDB](https://www.jackdb.com).  The schema for the database is:


	Movie(mID, title, year, director)
	Reviewer(rID, name)
	Rating(rID, mID, stars, ratingDate)

Here are some queries.  Feel free to use Piazza to discuss how solve these queries.  I will not be posting solutions because in my experience students gain misplaced confidence by reviewing the *solutions* rather than working through each of the problems.

1. Find the titles of all movies directed by Steven Spielberg.   
2. Find all years that have a movie that received a rating of 4 or 5, and sort them in increasing order.   A given year should not appear more than once. 
3. Write a query to return the ratings data in a more readable format: reviewer name, movie title, stars, and ratingDate. Also, sort the data, first by reviewer name, then by movie title, and lastly by number of stars, all in ascending order. 
4. Find names of reviewers who have reviewed movies from before 1960 or whose titles start with the letter A. 
5. For each movie that has at least one rating, find the highest number of stars that movie received. Return the movie title and number of stars. Sort by movie title.  
6. For each movie that received at least one rating, find the title along with the number of ratings it has received.   
7. For each movie that received at least one rating, find the title along with the number of reviewers that have reviewed it.   
8. For each movie that has at least one rating, return the title and the rating spread, that is, the difference between highest and lowest ratings given to that movie. Sort by rating spread from highest to lowest, then by movie title alphabetically.    
9. For each movie that has at least one rating, the title, the director and its highest rating.  The highest rating should be an attribute called maxStars. 
10. For each movie that has at least one rating, the title, the director and its highest rating only for those movies whose highest rating is at most 4. 
11. Find the number of moives that Steven Spielberg has directed whose highest rating is at least 3.  Hint: use an earlier query as a subquery in the FROM clause. 
12. Find the average rating of movies released after 1980. (Keep in mind that some movies have been reviewed more than once.  So make sure to calculate the average rating for each movie, and THEN the average of those averages.)   
