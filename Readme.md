# Data Wrangling: WeRateDogs Tweets

This project was developed to analyse tweets from the [WeRateDogs](https://twitter.com/dog_rates) page from Twitter. It aims to go through the role process of data wrangling: gather, access and clean data.

## Packages

The project requires the installation of the following packages: `Pandas`, `Numpy`, `Matplotlib`, `Seaborn`, `Requests`, `Tweepy`, `Json`, `Datetime` and the magic function `%Matplotlib inline`.

## Datasets

Data was extracted from Udacity's database and 2 datasets will be analyzed: the WeRateDogs Twitter archive ('twitter-archive-enhanced.csv' file) and the tweet image predictions ('image-predictions.tsv' file). Tweets data in json extension was downloaded using the `Tweepy` library and stored in a file called "tweet_json.txt".

## Structure

The structure was divided in six (6) main parts related to the Data Wrangling process + Conclusion and References:

* Brief Introduction
* Part I - Gather
* Part II - Assess
* Part III - Clean
* Part IV - Analysis and Visualization
* Part V - Conclusions
* Part VI - References

## Assess 

During the development of the project, eight (8) quality issues and two (2) tidiness issues were fixed (find them below). It was possible to observe incorrect data types, incorrect values in a column, irrelevant columns to analyze, variables from the same 'group' in different columns and data that could be merged in the same dataframe.

### Quality Issues

* Timestamp column has '+0000' after time;
* Timestamp column is a string, not a datetime object;
* doggo, puppo, floffer and pupper columns have missing values stored as 'None';
* doggo, puppo, floffer and pupper should be set as categorical values;
* Retweets should be excluded;
* Invalid dog names starting with 'a', 'an' and 'the' should be removed;
* tweet_id should be converted to a string - Issue fixed on Tidiness section, during merging process; 
* Rating numerator of '1776' should be excluded.

### Tidiness Issues

* Image prediction and tweets dataframes could be merged in the same df;
* Dog breeds can be unified in one column.

## Conclusions

The project analyzed some preferences from users subscribed in a popular account on Twitter: WeRateDogs.

It was possible to observe that datasets with a lot of information should pass through a clean process, otherwise insights or results could present erroneous information.

After an extensive cleaning process, it was possible to verify that the top 3 common dog breeds extracted from the dataset are golden_retriever, Labrador_retriever and Pembroke, the favorite dog development stage from Twitter's users is puppo and the least favorite is pupper.
