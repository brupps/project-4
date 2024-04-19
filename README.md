# Reel Success: A Deep Dive into Film Performance

## Description/Overview
The topic we have chosen is movie success rate based on gross revenue. The goal of our project is to predict whether a movie will be successful based on profitability. We will be using several features in our predictive model such as rating, genre, director, etc.

## Tableau Dashboard
We created a beautiful Tableau dashboard showcasing our data; it gives a great overview in a clean and concise way!

<a href=”LINK”>Link to the dashboard</a>

![a screenshot of the tableau dashboard](https://github.com/cassidysimmons/project-4/blob/main/Resources/imagenamehere.PNG)


## Methodology
1. Finding the data
	- All of our data was found on <a href="https://www.kaggle.com">Kaggle.com</a>; we were able to directly export IMDB movie data as a single csv file

2. Cleaning the data
	- Our data ending up having several missing/ null values across many columns, we opted to remove all the missing values, leaving us with ~5,000 rows
	- After the initial data cleaning we opted to removed four extreme outliers that greatly skewed the data

3. Testing different models
	- Initially, we were unsure what model would be the best fit for our data/ goal so we tested out four different models: linear regression, gradient boost, random forest and neural network
	- The random forest model seemed to yield the highest accuracy score therefore we went with that one as the best choice

4. Optimizing the chosen model
	- After determining which model to use (random forest) we then set out to optimize said model to achieve the highest accuracy score possible. We carefully selected only the necessary features, appropriate target array and encoded any categorical values as needed.


## Files
- **data_cleaning.ipynb**
	- Cleaned the raw csv using pandas (removed unnecessary columns and extreme outliers) and exported the cleaned data as a csv into the resources folder


### Resources Folder
- **movies.csv**
	- Our raw, uncleaned data exported from Kaggle; movie data, includes columns such as name, director, budget, revenue, etc.

- **movies_cleaned.csv**
	- Cleaned movie data; excludes missing/ null values and extreme outliers


## Model Iterations
- **movie_neural_network.ipynb**
	- Tried building a neural network model; after several iterations changing features, target arrays, activations functions, etc. we ended with an optimal accuracy of ~58% (did not include as final model)

- **angie_predictions.ipynb**
	- Tried linear regression and random forest; linear regression return an R-squared of 0.34 (did not reach >0.80), random forest model returned promising results so we continued more in depth work in a new notebook

- **random_forest_trials.ipynb**
	- Continued iterations on the random forest model
	- Also tried gradient boost model, returned an R-squared of 0.46 (did not reach >0.80)

- **final_rf_model.ipynb**
	- Final round of random forest iterations; nailed down column transformations, ideal features and target arrays, etc. ***(ended with an accuracy of 65%)***


## Presentation Slides
Our final presentation displaying the entire project in a neat, aesthetically pleasing slide deck!

<a href="https://www.canva.com/design/DAGCKADuW0c/rGow_eKabuBoLh1OqogbPA/edit?utm_content=DAGCKADuW0c&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton">Link to the Canva slide deck</a>


## Acknowledgements
- <a href="https://github.com/brupps">Barb Rupps</a>
- <a href="https://github.com/angiecfoust">Angie Foust </a>
- <a href="https://github.com/cassidysimmons">Cassidy Simmons </a>
- <a href="https://github.com/ASPigman">Amanda Pigman </a>


## Resources
- <a href="https://www.kaggle.com/datasets/danielgrijalvas/movies">IMDB movie data</a>
- <a href="https://medium.com/analytics-vidhya/how-to-use-machine-learning-approach-to-predict-movie-box-office-revenue-success-e2e688669972">Movie project example 1</a>
- <a href="https://ryan-anderson-ds.medium.com/what-makes-a-successful-film-predicting-a-films-revenue-and-user-rating-with-machine-learning-e2d1b42365e7">Movie project example 2</a>
- <a href="https://screenrant.com/the-creator-budget-box-office-prediction/#:~:text=It%20is%20usually%20estimated%20that,would%20be%20twice%20the%20cost">Profit definition</a>
- <a href="https://scikit-learn.org/stable/auto_examples/ensemble/index.html">Ensemble Documentation</a>
