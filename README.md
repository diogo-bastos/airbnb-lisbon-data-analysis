# AirBnb Lisbon Data Analysis

The purpose of this repository is to analyze public data from the listings of the company AirBnb, in the city of Lisbon. 
The data was obtained from this page: http://insideairbnb.com/get-the-data.html.

The analysis attempts to answer the following questions:

## Which neighbourhoods have the most listings, which are more expensive and which have the most positive reviews?

**Number of Listings**
1. Alfama (1376)
2. Baixa (941)
3. São Jorge de Arroios (815)

**Review Score** 
1. Charneca (98.25)
2. São João de Deus (94.17)
3. Santa Maria dos Olivais (94.14)

**Price in American Dollars**
1. Bairro Alto (300.00)
2. Benfica (210.59)
3. São Domingos de Benfica (197.35)

## Do super hosts have more positive reviews than regular hosts?

The response is yes! Super hosts do have more positive reviews on average than regular hosts.

**Average Review Score**
1. Super Hosts - 96.862366
2. Regular Hosts - 90.778280

## What are the factors that contribute the most to more positive reviews?

It is safe to say that super hosts do have the highest review scores. Price, the number of amenities and availability seem to the following most important factors. It is interesting to notice that the cleaning fee and whether extra people are allowed or not seems to have an impact as well.

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






