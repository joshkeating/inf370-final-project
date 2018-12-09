# Airbnb Seattle Pricing Predictions

## Framing the Problem

The purpose of this project is to identify the aspects of Airbnb host listings that have a correlation to the price of bookings. This information will allow Airbnb hosts to find and improve certain variables of their listing that are the highest indicators when it comes to setting price. Our predictive model can provide rough estimates as to how much your Airbnb in Seattle should be listed at based on your listing criteria.

The dataset used was the Seattle Airbnb Open Dataset found on Kaggle [here](https://www.kaggle.com/airbnb/seattle#calendar.csv). The two CSV files we are using from this set are `calendar.csv` and `listings.csv`. The calendar file displays the `listing_id`, the dates, whether it is available on that date, and the price of booking for that day. The listings file includes a wide variety of metadata scraped from the listing url.

On top of the given columns in the dataset, we used the Microsoft Azure Text Sentiment Analysis API to calculate the sentiment value (on a scale of 1 - 100) of the listing summary. Positive and negative sentiment can be identified and perhaps has a correlation to number of bookings. This was done using post requests on Postman and is located in a file as scores.csv.

As an additional insight, we also included exploratory analysis through a predictive model on the ratings of listings at the bottom of the notebook.

## Project Structure

The data cleaning and preparation is performed primarily in the `clean-data.ipynb` notebook [link](https://github.com/joshkeating/inf370-final-project/blob/master/clean-data.ipynb). All of the data exploration, model training, parameter selection, and analysis is performed in the main `analysis.ipynb` notebook [link](https://github.com/joshkeating/inf370-final-project/blob/master/analysis.ipynb).

The origianl dataset is included in this repository with the addition of the calculated sentiment value from the listing summary. These files are located in the `/data` directory. 

## Paper

The full academic paper can be viewed [here](https://github.com/joshkeating/inf370-final-project/blob/master/INFO%20370%20Final%20Paper.pdf)