# NLP-Janata-Hackathon

## Hackathon Description:

Sentiment Analysis for Steam Reviews (conducted by Analytics Vidhya)
Steam is a video game digital distribution service with a vast community of gamers globally. A lot of gamers write reviews at the game page and have an option of choosing whether they would recommend this game to others or not. However, determining this sentiment automatically from text can help Steam to automatically tag such reviews extracted from other forums across the internet and can help them better judge the popularity of games.

Given the review text with user recommendation and other information related to each game for 64 game titles, the task is to predict whether the reviewer recommended the game titles available in the test set on the basis of review text and other information.

Game overview information for both train and test are available in single file game_overview.csv inside train.zip

## Data Dictionary:
### train.csv
1. **review_id** : Unique ID for each review
2. **title** : Title of the game
3. **year** : Year in which the review was posted
4. **user_review** : Full text of the review posted by the user
5. **user_suggestion** : User will Recommend or Not Recommend the game

### game_overview.csv
1. **title** : Title of the game
2. **developer** : Name of the developer of the game
3. **publisher** : Name of the publisher of the game
4. **tags** : Popular user defined tags for the game
5. **overview** : Overview of the game provided by the publisher

### test.csv
1. **review_id** : Unique ID for each review
2. **title** : Title of the game
3. **year** : Year in which the review was posted
4. **user_review** : Full text of the review posted by the user

### samplesubmission.csv
1. **review_id** : Unique ID for each review
2. **user_suggestion** : User will Recommend or Not Recommend the game


## Evaluation Metric
Submissions are evaluated on `binary F1` score between the predicted and observed user suggestion for the reviews in the test set.
