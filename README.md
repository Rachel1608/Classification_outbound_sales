# Classification_outbound_sales

# Importing the Necessary Librabies
  * Pandas (Loading the dataset)
  * Numpy
  * nltk (preprocess)
  * spacy
  * Regex (Cleaning the dataset)

* Checking the Shape of the Data
* Checking the Data description to find the missing values
* Checking the Data info for the datatypes
* Checking the null value using .isnull()
* Using value_counts to count the labels

# Preprocessing the dataset
  * Cleaning the indepentdent feature using regular expression and assigned new column for the further process
  * Lowercasing the labeled data and used unique function to avoid the unnecessary classes for the training the model
  * We tokenize the reply feature and remove the stopwords and did lemmatize using WordNetLemmatizer for the better primary words.
  * Assigned new column as tokens for the preprocessed data.

# Label Encoder
  * Since it is Classification Problem and Multiclass we used Label Encoder to transform the label feature to numeric.

* We joined the preprocessed tokens column for the vectorization to train the data

# Model Training
  * We used TF-IDF vectorizer for vectorization for the training set
  * We did train_test_split with 75% training the data and 25% test size for training and testing the model
  * We used Logistic Regression for the Classifier and tested the raw input with the label encoded.
  * The model performed good with 100% Training Accuracy and 99% Testing Accuracy.

# Fine_tuning the transformer model (Distilbert-base-uncased)
* We imported necessary libraries for classification like DistilBertTokenizerFast, DistilBertForSequenceClassification, Trainer, TrainingArgument and whole process done pytorch
* Loading the tokenizer and model from the pretrained model and number labels for prediction.
*  We removed original label column for training
*  Renamed the label_encoded to label for the trainer.
*  We did training arguments with the parameters.
*  Compute metrics with accuracy for prediction.
*  We trained the transformer using trainer with setting up parameters from training arguments.
*  Model performed better with 99% Accuracy with 0.01 validation loss.

# Comparing the Model
* Both performed well
* Distilbert Base uncased is more effective for the production.

    
