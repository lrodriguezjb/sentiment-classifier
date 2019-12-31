# Natural Language Processing
# Sentiment Classification Modeling

**Author**: Stephen Koch
**Version**: 1.0.0

## Overview
In this notebook, we are looking reading in a csv data file of [hotel reviews](https://www.kaggle.com/datafiniti/hotel-reviews#7282_1.csv) with [TensorFlow](https://www.tensorflow.org/) using [TensorFlow.keras](https://www.tensorflow.org/guide/keras). TensorFlow and TF.keras are both running ontop of [NumPy](https://numpy.org/). [Matplotlib](https://matplotlib.org/) is also running ontop of [NumPy](https://numpy.org/) and both are used to create graphs and tables from the data.

Before we can create a natural language processing model from our data, we need to clean up the data for use and assign sentiments to the data. We have chosen to rate the reviews on a scale of 0 - negative, 1 - neutral, and 2 - positive sentiments. Because this dataset is a little skewed toward the upper end (5/5), the decision was made to distribute sentiments as scores of 3 and lower are negative, 4 is neutral and 5 is positive.

## Getting Started
The original data set can be accessed from: [Kaggle - Hotel Reviews](https://www.kaggle.com/datafiniti/hotel-reviews#7282_1.csv). From there you can click the link for New Notebook which allows you to work from their virtual environment with no installation required!

![Access Kaggle Notebook](data/kaggle_hotel_reviews.png)

You can of course make your own copy this repository as well:
First, make sure that you have python3 installed:
```
$ python3 --version
Python 3.7.5
```
If you do not:
```
$ brew install python
```
You need to have the files locally. Click on the green clone or download button and Download ZIP:

![Click_to_download](data/Click_to_download.png)

Navigate to your command line:
```
MacOS: Press command + space to open up the search feature
Search for terminal - This is your command line.
```

In your command line, navigate to this directory:
```
$ cd ~  ##this is your root directory
$ cd Downloads  ##by default: Downloads is a directory inside of your root; and where your file will be downloaded
$ cd sentiment-classifier ##and now you are in this directory
```
This is a collection of Jupyter Nodebook from TensorFlow. Opening the notebooks requires jupyter, matplotlib, tensorflow, and numpy.

First we need to create a virtual environment to install our package dependencies. To be safe we will install them individually.

We are using a pipenv virtual environment:
```
$ pipenv install jupyter numpy pandas Keras tensorflow
```
Your packages will be installed after a short while.
We need to be running in our virtual environment to use our packages:
```
$ pipenv shell
```
From our virtual environment, we can open our sentiment_classification.ipynb notebook and get started!

## Change Log
Mon Dec 30 2019 20:57:23<br>Collected data on hotel ratings. Added a sentiment rating based on the distribution of user ratings on hotels. 

