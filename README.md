# TikTok Video Claim Prediction Project

## Overview

The goal of this project was to create a logistic regression, a random forest, and a XGBoost model to predict whether a video contains a claim or offers an opinion. This project utilized a dataset where each row represents a different published TikTok video in which a claim/opinion has been made. The final random forest model performed with 99.7% accuracy, 99.7% precision, and 99.7% recall in determining if a video is a claim. The final XGBoost model performed with 99.3% accuracy, 99.8% precision, and 98.9% recall in determining if a video is a claim. Based on the metric results, the random forest model is the champion model. According the feature importances plot of the random forest model, the video view count, video like count, and video share count were most influential in determining if a video contains a claim or an opinion. 

## Business Understanding

TikTok users have the ability to submit reports that identify videos and comments that contain user claims. These reports identify content that needs to be reviewed by moderators. The process generates a large number of user reports that are challenging to consider in a timely manner. By developing a predictive model that can determine whether a video contains a claim or offers an opinion, TikTok can reduce the backlog of user reports and prioritize them more efficiently.

## Data Understanding

The dataset used in this project contains synthetic data created for this project in partnership with TikTok. The data consisted of around 19k published TikTok videos in which a claim/opinion has been made. The features included information on a video, such as its id, the duration, the author's ban status, and so on. A new feature, called text_length, was engineered out of the length of a video's transcription text to be used as a potential feature in the model.

## Modeling and Evaluation

A random forest model comprising 200 decision trees was used to determine feature importance in whether a TikTok video contains a claim or an opinion. The below plot shows that a video's view count, like count, share count, and download count were the Top 4 most important factors in determining if a video contains a claim or an opinion. The overall model performed with 99.7% accuracy, 99.7% precision, and 99.7% recall.
![TikTok RF Feature Importance Plot](https://github.com/chungchenran2/TikTok_Video_Claim_Prediction_Project/blob/main/Images/TikTok_RF_Feature_Importance.png)

## Conclusion

This model can benefit TikTok moderators in determining whether a video contains a claim or offers an opinion, reducing the backlog of user reports and prioritize them more efficiently. In the future, adding more information on a video and a user report may also be beneficial in helping the stakeholder address their business problem.
