# Twitter-Sentiment-Analysis
<img src="./images/banner.jpeg" width="350" height="200">

## About
Twitter Sentiment Analysis is a project that describes an analysis of the public sentiment toward presidential candidates (**Barack Obama** and **Mitt Romney**) in the 2012 U.S. election as expressed on Twitter.

'*training-Obama-Romney-tweets*' is the dataset based on which the project has been built. The csv file can be found in the 'dataset' directory of this repository.

- **Objective**: The analysis is performed for determining whether data is neutral, positive, or negative. It is used to detect a particular emotion based on a list of words and their corresponding emotions.

The dataset contains the tweets from 2012 presidential election for Barack Obama and Mitt Romney. The training data consists of three sentiments - '*positive*'(+1), '*negative*'(-1), '*neutral*'(0).

## How to run this project?
_Note: This project is run on Anaconda distribution._
1. Clone the repositiory into your workspace using the code link.
2. Install the required libraries shown in the 1st block of ipynb file.
3. Open IPython Notebook: Data_Mining_Project.ipynb with Jupyter Notebook.
4. Run the Notebook to view the results.

- **Data Cleaning and Pre-Processing**: 
1. Data cleaning was an integral part for sentiment analysis to remove unwanted data. This included converting the text to lower case, removing certain stop words which were repeated regularly in many tweets, removing non alpha numeric characters including hashtags.
2. The text after hashtag was retained to capture the emotion in the tweet for determining the sentiment better. Hyperlinks like ‘www. ’, ‘http://’ and ‘https://’ were removed, stemming of the text for instance, words ‘likes’, ‘liked’, ‘likely’ and ‘liking’ were stemmed to like and deleted the single length and double length characters which were not part of the stop word library like a, an, the, in, at, etc.

- **Data Analysis**:
The data retrieved from Kaggle contained 14000 tweets of training data and 2000 tweets of test data. My objective was to predict a sentiment behind a given tweet in the test data accurately using various classification models like '*Naive Bayes'*, '*Logistic Regression'*, '*Random Forest'*, and '*Support Vector Machine'* to find the model with the best accuracy using the Python.

- **Results**:
The top two models were Logistic Regression and Naïve Bayes, and '**Logistics Regression**' gave the best output with and accuracy of 70% and F1 score of 66%. Here 70% was a good enough accuracy as the data was minimized to 14,000 records. With a larger dataset we would get a higher accuracy.      



