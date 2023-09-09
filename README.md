TODO: implement pipeline as an airflow DAG
# machine-learning-pipeline
I made this machine learning pipeline to show recruiters an example of my skills in data engineering and my style of writing and documenting code. 

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
