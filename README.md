# Video Game Recommender

## Goal

To recommend games based on a game given by the user. Show rating, cover art, current stats etc. of the recommended game. 

## Tasks

### Cleaning data
  1. Acquire a dataset consisting of popular games to recommend from.
  2. Clean the data.
  3. Separate numerical/categorical and scale/transform.
  4. Find optimum K for KMeans.
  5. Train KMeans model on the dataset to predict their clusters.
  6. Save the dataset with the clusters to be used later for recommendation.
  7. Save the model and tranformers to predict cluster on the new data.

### Building recommender

  1. Take a game name as user input, search for the game on the site and scrape the top search results.
  2. Allow user to select their game from the search results; if game not found, search again. 
  3. Once the game is selected, go to the site and scrape the game data needed to predict cluster.
  4. Scale/ transform scraped game data using the saved transformers.
  5. Predict the cluster of the game using the trained model.
  6. Recommend another game from the predicted cluster. Try to recommend game with rating higher or equal to user game else recommend any game from the cluster.
  7. Ask for a new recommendation for the same user game.
  8. If 'no' then start again or quit.

  * website used fro scraping game data: https://www.backloggd.com/
    
