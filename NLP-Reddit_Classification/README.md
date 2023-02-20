## Post Classifier using Web APIs & NLP

### Description:

- This project seeks to construct a classification model that can be used to predict the underlying subject of posts between two similar topics, perfume and pake up. 
- The classification model will be constructed based on a data set of over 10,000 previous reddit posts.
- Final model accuracy is approximately 97% and may be further refined in the future.

### Process:

- Data scraped from subreddits 'Perfume' and 'Makeup'
- Data cleaned in a manner deemed appropriate. 
- Variations of root word removed to avoid bias.
    - eg. 'perfume', 'perfumes', 'makeup', 'make', 'up', 'makeups', 'ups'
- Posts lemmatised before vectorising. 
- Utilised three vectorisation methods.
    1. Count Vectorisation
    2. N-grams
    3. TF-IDF
- Tested three variations of Naive Bayes on the three vectorisation methods to determine most suitable dataset.
    1. Bernoulli
    2. Multinomial
    3. Gaussian
- Naive Bayes models and other models optimised on TF-IDF dataset after determining it's most suitable. Other models include:
    1. Logistic Regression
    2. K-Nearest Neighbour
- Multinomial Naive Bayes model deemed to be most appropriate.
 

### Files used:

- data_makeup.csv -- Raw scraped data from subreddit 'Makeup'.
- data_perfume.csv -- Raw scraped data from subreddit 'Perfume'.
- data_raw.csv -- Merged raw scraped data from both subreddits 'Perfume' and 'Makeup'.

### Codebook / Data Dictionary:

- subreddit - the name of the subreddit where post was scraped from.
- title - the title/topic when a post is created.
- selftext - the body or paragraph of the post below the title/topic.


### Credits:
#### Advisors:
- Kishan
- Joshua Soh

### Project Status:
- Plans to refine the model further are subjected to availability.