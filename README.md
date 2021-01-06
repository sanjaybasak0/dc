# Document classification using 1D convolution.
In this project I have done classification of the documents.Each document is consists of an email.In the dataset we have 18828 documents and there are 20 classes.Our task is to classify a document into one of the 20 classes.
Basically there are two major parts in the project.In the first part data preparation is done and in the second part building a model,training the model and validation of the model are done.
# Data Preparation
In this part very complex data preprocessing is done and please go to this [file](https://github.com/sanjaybasak0/dc/blob/main/Text%20Classification%20Assignment.ipynb) to check what type of data preprocessing is done.After preprocessing all the documents we build a dataframe containing three columns namely preprocessed_subject, preprocessed_email and preprocessed_text. preocessed_subject contains all the subjects of the documents, i.e. as here each document is an email therefore preprocessed_subject contains all the subjects of the emails. preprocess_email contains all the email ids in the documents, i.e. we collect all the email ids from the body of the email(document). preprocessed_text contains the preprocessed texts in the documents(texts in the body of the email).

# Architecture of the model_1
![alt text](https://github.com/sanjaybasak0/images/blob/main/document_model_1.png)

In the model_1, we have used word embedding.To measure the model's performance we have used F1 score.After training we got training F1 score = 0.8849 and test F1 score = 0.7034.

# Architecture of the model_2
![alt text](https://github.com/sanjaybasak0/images/blob/main/document_model_2.png)

In the model_2, we have used character level embedding.To measure the model's performance we have F1 score.After training we got training F1 score = 0.3538 and test F1 score = 0.1189.
