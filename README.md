# AirBnb Lisbon Data Analysis

The purpose of this repository is to analyze public data from the listings of the company AirBnb, in the city of Lisbon. 
The data was obtained from this page: http://insideairbnb.com/get-the-data.html.

The analysis attempts to answer the following questions:

## Which neighbourhoods have the most listings, which are more expensive and which have the most positive reviews?

The data from the listings.csv file is grouped by the "neighbourhood" column with the "count" aggregation function
in order to obtain this result.

**Review Score** 

The data from the listings.csv file is grouped by the "review_scores_rating" column with the "mean" aggregation function
in order to obtain this result.

**Price**

The "price" column is encoded into the "float_price" column by removing the currency symbol and parsing the values into floats.
Moreover, the data is grouped by the new encoded column with the "mean" aggregation function.

## Do super hosts have more positive reviews than regular hosts?

The "host_is_superhost" column is encoded into the "host_is_superhost_encoded" column by parsing the 't' and 'f' strings into boolean values.
Moreover, the data is grouped by the new encoded column with the "mean" aggregation function.

## What are the factors that contribute the most to more positive reviews?

In order to answer this question, a random forest regression is applied to the data in order to extract the feature importances from each of the paramters.
In order to wrangle the data, the following steps are followed:
	* NaN value analysis.
	* Encoding
	* Scaling
	
Furthermore, to extract the desired information from the random forest regression, the following steps are taken:
	* Grid search with cross validation
	* Learning Curve
	* Feature Importance Graph
	

## Package Dependencies

The following python libraries are used in other to aid in the data cleaning and analysis:

* numpy
* pandas
* matplotlib
* scikit-learn

To run this notebook locally, make sure you have Python 3 with the previously mentioned libraries installed, as well as Jupyter.
Navigate to the directory where the notebook file is, open a command prompt and type "jupyter notebook".

## Files in the repository

* **listings.csv** - public AirBnb data taken from the following source: http://insideairbnb.com/get-the-data.html.
* **Airbnb-Lisbon-Data-Analysis.ipynb** - a jupyter notebook which analyses the data in listings.csv.
* **License** - the license file.

## License

This repository is licensed under the MIT License. This license is short, simple and permissive with conditions only requiring preservation of copyright and license notices. Licensed works, modifications, and larger works may be distributed under different terms and without source code. To learn more, please the read the corresponding license file.






