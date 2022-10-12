# WeRateDogs Twitter Analysis

Wrangling, analysis and visualization of the tweet archive of Twitter user [@dog_rates](https://twitter.com/dog_rates), also known as [WeRateDogs](https://en.wikipedia.org/wiki/WeRateDogs). 

## Gathering Data

Three datasets were gathered from three different sources. 

The first is the **WeRateDogs Twitter Archive** which can be found [here](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/59a4e958_twitter-archive-enhanced/twitter-archive-enhanced.csv). The CSV file was downloaded manually and read into a [`pandas`](https://pandas.pydata.org/) dataframe.

The second is the **Tweet Image Predictions**; a file containing the tweets’ image predictions according to a neural network. The TSV file was downloaded programmatically from [Udacity’s server](https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv) using the [`Requests`](https://pypi.org/project/requests/) library.

The third is **Additional data _(specifically, retweet count and favorite count)_** from Twitter API. Twitter API was queried for the JSON data of each tweet in the Twitter Archive using Python's [`Tweepy`](http://www.tweepy.org/) library.

## Assessing Data

The gathered data were assessed both visually and programmatically in order to detect and document any quality and tidiness issues that they might have.

## Cleaning Data

The issues detected were cleaned using the 'define-code-test' framework.

## Storing Data

After all the data had been cleaned, they were merged into a master dataframe and stored in a CSV file. 

## Analyzing and Visualizing Data

The cleaned data was analyzed to answer the following questions:
- What dog breed is the most popular?
- What dog breed has the highest number of likes from tweets?
- What dog stage is the most popular?
- What dog stage has the highest number of likes from tweets?

## Reporting

Two reports were created:
- The **wrangle_report** that briefly describes the wrangling efforts.
- The **act_report** that communicates all the insights and displays the visualizations produced. 