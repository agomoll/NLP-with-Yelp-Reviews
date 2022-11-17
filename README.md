# NLP-with-Yelp-Reviews
Using Natural Language Processing to parse Yelp review data and testing a Machine Learning Model's ability to predict positive or negative reviews

## Resources
  * Python
  * Pyspark
  * Google CoLab



## Method

The Yelp review data was composed of 1000 yelp reviews for a restaurant csv format. Each review included the text of the review as well as a classification of 'positive' or 'negative'. 


#### Initial Data 

<img src="Resources/initial_data.png" width=25%>

#### Adding a 'length' as a feature for later prediction modeling

<img src="Resources/length_feature.png" width=25%>

#### Transformation code

<img src="Resources/transform_features.png" width=65%>

#### Labels and resulting features DataFrame

<img src="Resources/label_and_resulting_features.png" width=25%>

#### Transformed Model DataFrame
The data was split into 70% training data and 30% testing data.  Then a Naive Bayes Machine Learning classifier model was fit to the training data. The fit model was then used to produce predicted classification on the testing Yelp reviews. Predicted values are seen in the last column of the DataFrame.

<img src="Resources/transformed_model.png" width=85%>

#### Model Accuracy

<img src="Resources/model_accuracy.png" width=65%>

## Analysis
At 70% accuracy there is room for improvement. However, if the goal is simply to get a high level assessment of general sentiment then this model may be helpful with further sets of yelp reviews on this particular restaurant.
