# Predicting Amazon Kindle Product Ratings Based on Review Text
The project aims to Predict the overall rating of Amazon Kindle products based on the textual content of the reviews.

Documentation for Amazon Kindle Reviews Analysis

Business Understanding

1.1 Objective: To predict the overall rating of Amazon Kindle products based on user review text.

1.2 Goals: Develop a machine learning model to classify review ratings. Provide insights into model performance using appropriate metrics and visualizations.

Data Understanding

2.1 Dataset: Sample of 982,619 reviews from the Amazon Kindle store. Key columns: reviewerID, asin, reviewerName, helpful, reviewText, overall, summary, unixReviewTime, reviewTime.

Data Preparation

3.1 Data Filtering: Review texts and ratings are extracted into separate lists. The length of each review text is calculated, and only valid data is kept. A subset of 200,000 samples is used for training due to computational constraints.

3.2 Text Length Analysis: The average length of review texts is calculated. Reviews longer than the average are identified.

Pre-trained Word Embeddings

4.1 GloVe Embeddings: GloVe embeddings are used for word representation. The file glove.6B.zip is downloaded and extracted if not already present. The embeddings are loaded into memory for further processing.

Model Training

5.1 Model Architecture: A deep learning model is constructed using PyTorch, specifically an LSTM for text classification.

5.2 Training: The model is trained using a training dataset for a specified number of epochs.

Model Evaluation

6.1 Evaluation Metrics: The model is evaluated using metrics such as precision, recall, F1-score, and accuracy.

6.2 Results: The model achieved the accuracy is below 50%, indicating potential for improvement with more training data, longer texts, and more training epochs.

Conclusion： 

The project successfully implemented a text classification model to predict overall ratings from review texts. Future improvements could include utilizing more computational resources and advanced models for better performance.
