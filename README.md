# riiid_education_lgb_model

Kaggle Profile: https://www.kaggle.com/brendanartley

I posted the code files for this competition here just in case, but I strongly encourage you to check them out on Kaggle for increased readability and context.

## Files

[Early EDA](eda-riiid-answer-correctness-data-exploration.ipynb)

- This early exploratory data analysis notebook was completed well before the other notebooks. Just exploring and plotting the data is important to get a good sense of what you are working with. You can figure out whether the data set will require extensive cleaning, you can gain insight into potential feature opportunities, and you can explore the correlation between features provided and the predicted variable.


[Splitting Data](riiid-splitting-train-and-test-data.ipynb)

- This competition was interesting because all activity for this task was required to be completed in the Kaggle notebook environment. Due to limited computing resources in this environment, it was hard to find a balance between a satisfactory number of features and enough of the data. There were 100 million rows of interactions and the possibility for thousands of features. This file shows how and why I decided to split the data for training and feature creation. 

[Stats by Question](riiid-content-answers-df-preprocessing.ipynb)

- We were given content_id's in the dataset which provided us with a specific question that we knew the user was answering. I found using a groupby object and calculating the mean and avg_time spent on the question, I was given some powerful features. I would have done this in the actual notebook attempt, but when I kept this in the submission notebook I would exceed 16GB RAM limit and crash the notebook. In order to stay under this limit, I computed this in a separate notebook.

[Riiid Model + Prediction](riiid-attempt-lgb-model.ipynb)

- This is by far the most important notebook provided here. It contains much of the feature engineering and feature selection. Due to the train_test_split I made I was also able to loop over new information and update user and content statistics. These loops are provided in the notebook. There is also a decent amount of information and text I provided throughout the notebook to increase readability.
