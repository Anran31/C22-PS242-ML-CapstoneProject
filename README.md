# C22-PS242-ML-CapstoneProject

## Dataset Creation

The datasets that used in our project are consisted of 5 classes (Beach, Hotel, Temple, Museum, and Restaurant). The dataset of each class are based from user review on that place. The datasets of [Museum](https://www.kaggle.com/datasets/annecool37/museum-data), [Restaurant](https://www.kaggle.com/datasets/ahmedaliomar/restaurant-reviews), and [Hotel](https://www.kaggle.com/datasets/andrewmvd/trip-advisor-hotel-reviews) class are taken from kaggle. But, the datasets of Beach and Temple class are taken by scraping user review from Google Maps.

After collecting the data required, the datasets is created by taking 1000 records from each class. then, the dataset was split into training, test, and validation with 60%:20%:20% ratio.

Datasets used:

- Museum: https://www.kaggle.com/datasets/annecool37/museum-data
- Restaurant: https://www.kaggle.com/datasets/ahmedaliomar/restaurant-reviews
- Hotel: https://www.kaggle.com/datasets/andrewmvd/trip-advisor-hotel-reviews

## Creating and Training Model

Before training the model, we did preprocessing on the dataset by removing stopwords, leading spaces, punctuations, and numbers.

After doing the preprocessing, we build the ML model using a bidirectional LSTM layer for the training process.

## Model Results

After training, the best model we train has 99.17% accuracy and 90.21% validation accuracy.

## Saving the Model

Lastly, we save our model in `SavedModel` format and deploy it in Google Cloud Platform.
