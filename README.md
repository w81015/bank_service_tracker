[中文版 Chinese version](README_zh.md)

# Bank Service Topic Analysis Project

This project extracts, cleans, and analyzes data from the PTT Bank Forum (Bank Service). It uses LDA (Latent Dirichlet Allocation) to analyze popular topics within the forum and further interprets the results. The project is divided into three parts: data collection, data analysis, and result interpretation.

## Part One: Data Collection (`text_collection.ipynb`)

- **Objective**: Extract data from the PTT Bank Forum, capturing article titles, posts, comments, and other related information. This project utilizes over 4,000 pieces of data.
- **Tools Used**: Refer to the `Requirements` section at the end of the document.
- **Output**: Two datasets: one containing all data (over 100 articles, including titles, authors, likes, etc.), and another containing comments (over 3,900 comments).

## Part Two: Data Analysis (`lda_analysis.ipynb`)

- **Objective**: Apply cleaning techniques and LDA analysis to the collected data to identify dominant themes within the PTT Bank Forum.
- **Tools Used**: Python and its NLP libraries, such as `ckiptagger` for Chinese text segmentation and `gensim` for LDA modeling.
- **Output**: A set of topics representing the main discussion themes within the PTT Bank Forum, along with their respective word distributions and relevancy scores.

## How to Use

1. **Data Collection**: Run the `text_collection.ipynb` notebook to collect and preprocess data from PTT Bank.
2. **Data Analysis**: With the collected data, further clean it (segmentation, removing stop words) and then perform LDA analysis using the `lda_analysis.ipynb` notebook to reveal underlying topics.

## Result Interpretation

1. **LDA Analysis Webpage**: A topic model visualization webpage, observing three different topics' keywords, distribution, and similarity.
    1. Keywords like "credit card", "interest rate", "loan", "deposit" may reflect the discussion and attention of users on bank credit products and savings services.
    2. Terms such as "ATM", "online banking", "fees" may relate to the convenience and cost of banking services.
    3. Words related to file formats or URLs, like "jpg" or "picture", might refer to bank product promotional materials or screenshots shared by users.
2. **Datasets**: Over 100 articles and 3,900 comments from the PTT Bank Forum (Bank Service).

## Further Research

1. **Trend Analysis**: Track these keywords over time to help identify changes in user interests and market trends.
2. **Sentiment Analysis**: Incorporate sentiment analysis tools to assess the emotional tone during discussions, e.g., analyzing the positive and negative sentiments when discussing "fees" and "charges", providing insights for improving banking services.
3. **User Segmentation**: Segment users based on the topics and keywords discussed to understand the focus of different user groups.

## Requirements

- Python 3.6+
- `pandas`, `jieba`, `requests`, `beautifulsoup4`, `ckiptagger`, `gensim`, `pyLDAvis`.