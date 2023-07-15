# IMDBMovieAnalysis

The Final Project involves working with a dataset containing various columns of different movies from IMDb. The first step is to frame the problem by asking questions such as "What do you see happening?" and "What is the impact of the problem not being solved?" These questions will help define the problem and guide the analysis.

The data cleaning process is crucial and involves tasks like dropping columns, removing null values, and preparing the data for analysis. Once the data is cleaned, several tasks are to be performed:

Movies with highest profit: A new column called "profit" is created by calculating the difference between the "gross" and "budget" columns. The movies are sorted based on the profit and a chart is plotted to observe outliers.

Top 250 movies: A new column called "IMDb_Top_250" is created to store the top 250 movies with the highest IMDb ratings. The movies should have a minimum number of voted users of 25,000. A "Rank" column is also added to indicate the ranks of the corresponding films.

Top Foreign Language Films: Movies in the IMDb_Top_250 column that are not in the English language are extracted and stored in a new column named "Top_Foreign_Lang_Film."

Best Directors: The data is grouped by the "director_name" column, and the top 10 directors with the highest mean IMDb scores are identified and stored in a new column called "top10director." In case of a tie in IMDb score, the directors are sorted alphabetically.

Popular Genres: The popular genres are identified based on the knowledge gained from previous steps.

Actor Analysis: Three new columns are created for lead actors: "Meryl_Streep," "Leo_Caprio," and "Brad_Pitt," which contain the movies in which these actors are the lead. The rows of these columns are appended to create a new column named "Combined." The combined column is then grouped by the "actor_1_name" column, and the mean of "num_critic_for_reviews" and "num_users_for_review" is calculated to identify actors with the highest mean.

Decade Analysis: A column called "decade" is created to represent the decade to which each movie belongs. The data is sorted based on the decade, grouped by decade, and the sum of users voted in each decade is calculated and stored in a new data frame called "df_by_decade."

The final task is to find the critic-favorite and audience-favorite actors based on the analysis performed.
