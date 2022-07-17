# Google Play Review Sentiment Analysis

### Overview
This project works to uncover factors that influence Google Play application installs, which serves as a proxy for app success. Two datasets are merged and analyzed to address two hypotheses: 

- review sentiment impacts the number of app installs
- app category impacts the number of app installs

![google phone](https://images.unsplash.com/photo-1612442443556-09b5b309e637?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2070&q=80)

### Problem
Google play store apps are typically accompanied by user reviews sorted from most to least helpful. Prospective users make the decision to install apps for a variety of reasons, and in this study we seek to uncover the relationship between review sentiment and installation rate. The following questions is addressed: <b><i>“How much influence does review sentiment have on overall installs?”</b></i>

### Approach
Two datasets were obtained from [Kaggle](https://www.kaggle.com/datasets/yassershrief/goggle-play-data) and [Datacamp](https://projects.datacamp.com/projects/1197).

- apps.csv: contains all the details of the apps on Google Play. These are the features that describe an app.
- user_reviews.csv: contains 100 reviews for each app, most helpful first. The text in each review has been pre-processed, passed through a sentiment analyzer engine and tagged with its sentiment score

Exploratory, ANOVA, and Regression analyses are conducted to adress the project question.

### Results
- Games , Productivity and News and Magazine apps have significantly higher Install rates 
- 0.1 increase in sentiment score leads to 5.75M decrease in installs (p=0.002)
- Increase of sentiment score controlling for app size, price, and category is not significant

### Conclusions
- App sentiment is not a reliable metric of its success - further analyses using in-app data use may be a better metric
- Negative reviews should be used to support product improvement rather than be used as a metric for it's success.
- Higher utility apps will have high installation rates (including as news & productivity apps)
