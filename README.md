## Sentiment Analysis of 2020 US Election ##
These are the preliminary project files for my UCSD MLE Capstone Project. I used the [2020 Twitter Election Dataset](https://www.kaggle.com/datasets/manchunhui/us-election-2020-tweets/data) available on Kaggle.

The [docs](https://github.com/iamquantumis/capstone_project/tree/main/docs) folder includes the write-ups for the various project phases.

Here is a description of the Jupyter Notebooks:

- [election2020-priorwork.ipnyb](https://github.com/iamquantumis/capstone_project/blob/main/election2020-priorwork.ipynb) - This tries to replicate prior work performed on the dataset using [TextBlob](https://textblob.readthedocs.io/en/dev/) for basic sentiment analysis.
- [election2020-prediction.ipynb](https://github.com/iamquantumis/capstone_project/blob/main/election2020-prediction.ipynb) - First pass using [roBERTa](https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment-latest)
- [election2020-prediction-roBERTa.ipynb](https://github.com/iamquantumis/capstone_project/blob/main/election2020-prediction-roBERTa.ipynb) - Additional statistic analysis of the sentiment results, including results for just US users as well as with international users combined.
- [election2020-prediction-analysis.ipynb
](https://github.com/iamquantumis/capstone_project/blob/main/election2020-prediction-analysis.ipynb) - Added DistlBERT and sieBERT models (separately run due to resource constraints) to create an ensemble voting model from saved results. Best 2 of 3 model sentiment agreement decides final sentiment.
- [election2020-prediction-ensemble.ipynb](https://github.com/iamquantumis/capstone_project/blob/main/election2020-prediction-ensemble.ipynb) - Final notebook including all three modeels prior to deployment on Streamlit. See repo below for WebApp deployment.

See final project in my [election sentiment repo](https://github.com/iamquantumis/election_sentiment).
