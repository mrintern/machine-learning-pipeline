# machine-learning-pipeline
As a part of a final round interview for the position of "Senior Data Engineer", I was asked to create a machine learning pipeline from scratch. 
The pipeline does the following:
1. Sends a request to the NewsAPI's /sources endpoint (https://newsapi.org/)
2. Creates `sources.csv` from the API response
3. Sends a request to the NewsAPI's /everything endpoint
4. For every publisher in sources.csv grabs every article written in the past 3 days
5. Applies a sentiment analysis model to the article titles
6. Performs some data analysis
7. Generates a sql statement that can be used to upload this data to BigQuery for further analysis

Note: `pipeline.ipynb` is meant to be run in google colab.

Enjoy!
