# Financial subReddits, Data Analysis
 _Joao P. Maia_

In Reddit, a lot of groups are formed to discuss the stock market. Some of them are pretty known in the media (_r/wallstreetbets_ and _r/gme_) other despite their number of members, you barely hear about it. However, no one can deny the importance of this medium.

I used a Keagle Dataset to gather data from the most famous subreddits to analyze/study the posts and get insights about the correlation between them and the stock market itself.

## Dataset
All data used comes from [this dataset](https://www.kaggle.com/leukipp/reddit-finance-data). Apart from the data cleaning, the only major modification was the selection of subreddits with 20.000 or more posts.

Data used:
- r/wallstreetbets: #638158 (2021-01-01 00:02:06 - 2021-07-05 19:05:13)
- r/gme: #224149 (2021-01-01 04:08:51 - 2021-07-05 19:01:50)
- r/personalfinance: #64798 (2021-01-24 19:30:31 - 2021-07-05 19:03:36)
- r/stocks: #50729 (2021-01-01 00:05:17 - 2021-07-05 19:03:41)
- r/pennystocks: #42571 (2021-01-01 00:13:41 - 2021-07-05 19:04:28)
- r/stockmarket: #27710 (2021-01-01 02:42:42 - 2021-07-05 18:59:07)
- r/investing: #25486 (2021-01-01 00:18:40 - 2021-07-05 19:03:27)
- r/robinhoodpennystocks: #21200 (2021-01-01 00:27:36 - 2021-07-05 14:34:27)
- r/robinhoodpennystocks: #21200 (2021-01-01 00:27:36 - 2021-07-05 14:34:27)
- r/options: #18378 (2021-01-01 01:39:43 - 2021-07-05 19:00:27)

## Cleaning
In the _Main.py_ file, I used a series of scripts to clean/classify all data and then save it in an SQLite database (which is not included in this repo).

There is also support for adding more content over time without repeating the cleaning processes to the database provided it follows the same partner given in the Keagle dataset.

In the cleaning process, only full-text posts were considered. And the AFINN library was used for sentiment analysis.


## Terms/files
| File | Info |
| ------ | ------ |
| Main.ipynb |Introduction to the dataset, cleaning the data, and analyzing the sentiments using the AFINN library. |
| SILVER.ipynb | The precious metal. |
| GME.ipynb| GameStop, a game/console selling store. |
| NVDA.ipynb | Nvidia corporation.|
