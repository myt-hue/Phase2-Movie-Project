
- ![image](https://thumbs.dreamstime.com/b/movie-symbols-14119963.jpg)

# Movie Studios: What type of movies are doing best in the box office?
**Authors**: Mytreyi Abburu, Wes Smolen
## Business Problem
Our movie studio wants to make low budget movies and wants and is deciding what types of movies to make based on what   genre,   director, and month of release.
movies.

## Data Understanding
We analyzed movie databases, such as IMDB, the moviedb, and boxofficemojo. We filtered our dataset based on the genres and directors taken from imdb, profits caluclated based on movie budget and worldwidegross, and calendar release timeframe.
## Data Analysis
Through exploration of data from the tables in the IMDB database, we wrote a SQL query to combine the contents of the movie basics and movie ratings tables to the movie_budgets database to create a master database. 
First, we added a profits column which is the worldwidegross - production_budget. 
Next, we added separate columns for the  6 genres (action, horror, romance, adventure, fantasy, comedy)  to deal with movies with multiple genres.  
We made separate dataframes for each of the 6 genres 

### Combined Linear Regression Plot for 6 Genres (Production_Budget vs. Profit)
![image](https://github.com/myt-hue/Phase2-Movie-Project/assets/73657823/01705774-b502-4958-b7cf-8fe61d4887db)

Adventure performs the best with unlimited budget

### Combined Linear Regression Plot for low budget films for 6 genres
![image](https://github.com/myt-hue/Phase2-Movie-Project/assets/73657823/1f898e78-b705-45b0-9006-2724d1691ee4)

Profit is highest in Horror Genre Films with a budget of less than 10 million dollars
### Bar plot showing Top 10 directors with the highest average Profit for Low Budget Horror Movies
![image](https://github.com/myt-hue/Phase2-Movie-Project/assets/73657823/77cf1311-7797-4304-8312-068d9ef6a010)

### Highest Average Profit for Horror Movies by Month Released
![image](https://github.com/myt-hue/Phase2-Movie-Project/assets/73657823/92016c10-97ff-46c6-9e35-1145e4d2d33e)


October is the best month for Average Profit for Horror Movies Released


## Conclusion
Horror movies perform best in the box office given the budget is less than 10 million dollars.  October is the best month to release horror movies in order to generate the most profit.
## Further Investigation 
We plan to furthur analyze profit generation by country, identify up and coming directors while they’re still affordable, and reassess strategy once established and working with a higher budget.
## Additional Resources
• https://stephenfollows.com/what-the-data-says-about-producing-low-budg
et-horror-films/

• https://www.freecodecamp.org/news/whose-reviews-should-you-trust-imd
b-rotten-tomatoes-metacritic-or-fandango-7d1010c6cf19/

• https://www.themoviedb.org/talk/5daf6eb0ae36680011d7e6ee

## For more information
Please visit our full analysis in our Jupyter notebook ![website](https://github.com/myt-hue/Phase2-Movie-Project/blob/main/Exploration_Notebook.ipynb) or presentation ![presentation](https://github.com/myt-hue/Phase2-Movie-Project/blob/main/presentation.pdf)
Data taken from ![data](https://developer.imdb.com/non-commercial-datasets/), ![data](https://www.the-numbers.com/movie/budgets/all),![data](https://www.boxofficemojo.com/charts/)


For more questions, please feel free to reach us:   Mytreyi Abburu | abburumk@gmail.com, Wes Smolen | wjsmolen@gmail.com. 

## Repository Structure

You are currently in the README.md file. The 'index.ipynb' file contains the jupyter notebook of the explaratory analysis of the given data that provides step-by-step guide to how we came to our conclusion. 'Images' file contains the images used in this file. The images were taken from the internet.

```
├── Data                             <- Data file used in this project
├── Image                            <- Images and Graphs used in this project obtained from external and internal source
├── .gitignore                       <- Contains list of files to be ignored from GitHub
├── presentation.pdf   <- Slide Presentation of the project
├── README.md                        <- Contains README file to be reviewed    
└── index.ipynb                      <- Jupyter notebook of the project containing codes and analysis
