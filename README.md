# Spam Detection
##Overview
This model is able to analyse the contents of an email and indicate whether or not it is spam.

## Data Preprossing
This is normalising the contents of the email by converting it to lowercase, removing punctuations and stop words, and converting each word to their base form (lemmatization).
After which, the contents are vectorised using the TfidfVectorizer so that they can be understood by the model.

## Model Training and Selection
The contents in their vector form are then passed to the models for training. The models used were a Support Vector Classifier (SVC) model and MultinomialNB model, which were chosen because of they are known to perform well in natural language processing. The SVC had the better perfomance of the two reporting an accuracy of 97% and was selected to use in testing.

## Model Validation
The model was tested using a new dataset and the results were uploaded to a kaggle competition where it reported a 96.8% accuracy.
