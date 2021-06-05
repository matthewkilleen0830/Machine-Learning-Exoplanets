# Machine Learning Homework - Exoplanet Exploration

![exoplanets.jpg](Images/exoplanets.jpg)

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, you will create machine learning models capable of classifying candidate exoplanets from the raw dataset.

In this homework assignment, you will need to:

1. [Preprocess the raw data](#Preprocessing)
2. [Tune the models](#Tune-Model-Parameters)
3. [Compare two or more models](#Evaluate-Model-Performance)

- - -

## Instructions

### Preprocess the Data

* Preprocess the dataset prior to fitting the model.
* Perform feature selection and remove unnecessary features.
* Use `MinMaxScaler` to scale the numerical data.
* Separate the data into training and testing data.

### Tune Model Parameters

* Use `GridSearch` to tune model parameters.
* Tune and compare at least two different classifiers.

- - -

## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

* [Scikit-Learn Tutorial Part 1](https://www.youtube.com/watch?v=4PXAztQtoTg)

* [Scikit-Learn Tutorial Part 2](https://www.youtube.com/watch?v=gK43gtGh49o&t=5858s)

* [Grid Search](https://scikit-learn.org/stable/modules/grid_search.html)

- - -

## Hints and Considerations

* Start by cleaning the data, removing unnecessary columns, and scaling the data.

* Not all variables are significant be sure to remove any insignificant variables.

* Try a simple model first, and then tune the model using `GridSearch`.

* When hyper-parameter tuning, some models have parameters that depend on each other, and certain combinations will not create a valid model. Be sure to read through any warning messages and check the documentation

- - -

## Reporting: &nbsp;Model Performance

- Logistic Regression: &nbsp;GridSearch trained/tuned model was 87.93% accurate.

- Random Forests: &nbsp;GridSearch trained/tuned model was 89.16% accurate.

- k Nearest Neighbors: &nbsp;GridSearch trained/tuned model was 81.94% accurate.

- Neural Network/Deep Learning: &nbsp;trained model was 90.16% accurate.

In this example, we chose machine learning types Logistic Regression, Random Forests, k Nearest Neighbors, and
Neural Network/Deep Learning. &nbsp;Out of these four types, the Deep Learning model was most accurate. &nbsp;That being said, we feel that additional parameter tuning
would improve the results of this machine learning model. &nbsp;Since deep learning models are typically reserved for much
larger datasets, potentially more data from the Kepler deep space telescope could increase its accuracy even further. &nbsp;
Because this model is over 90% accurate, we feel it is good enough to correctly classify exoplanets.

Additionally, the k Nearest Neighbors model was more accurate (roughly 83% accurate) prior to applying GridSearch tuning. &nbsp;
Possibly specifying more parameters within the GridSearch would increase the accuracy of this trained/tuned model.

In sum, we feel that specififying more parameters within the GridSearch tuning has the potential to increase the accuracy of several types
of models whenever applicable.