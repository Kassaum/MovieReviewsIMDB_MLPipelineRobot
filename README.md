# MovieReviewsIMDB_MLPipelineRobot
POC of a ML pipeline created with UiPath AI Center, Movie Reviews from IMDB dataset

## AI Center entities

Project: IMDBReviews // Datasets: test and train // ML Package: IMDBReviews: ML Packages -> Out of the box Packages -> Language Analysis -> EnglishTextClassification // ML Skills: IMDBReviews

### Package

This model is a deep learning architecture for language classification. It is based on RoBERTa, a self-supervised method for pretraining natural language processing systems. The original paper can be found here https://arxiv.org/abs/1907.11692 by Yinhan Liu, Myle Ott et al. The model was open-sourced by Facebook AI Research.

## Robot / Pipeline

1. The robot get the reviews from the file: MovieReviews.xlsx
2. Classify the review
3. Add the result to the train data in AI Center
4. If the classification of the review have a less then 0.7 confidence a task is created in Orchestrator for manual classification
