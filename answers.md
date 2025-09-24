# Part C – Short Answer (Reasoning)

### If you only had 200 labeled replies, how would you improve the model without collecting thousands more?
* Its also based on the preprocessing techniques can be done from nltk as well as spacy, if we text preprocess the data using spacy, it preprocess from the pretrained model which helps for effective training the model
* we'll also use the Word embeddings like Word2Vec, Glove other than TF-IDF vectorizer for the accurate meaningful words.
* For the model training other than ML Algs, Ensemble techniques like Random Forest and Decision Trees helpful in training the model better.
* For the Transformer adjusting the Training Arguments make the model perform effectively with limited independent features.

### How would you ensure your reply classifier doesn’t produce biased or unsafe outputs in production?
* We can ensure by using different preprocessing methods like for the tokenisation word_tokenize, sentence_tokenize. For the Stopwords removel we can customize the stopwords and prevent from unsafe outputs.
* For Lemmatization we use WordNet Lemmatizer for good primary word.
* For the Vectorization we adjust the parameters like min_df, max_df, max_features to avoid the the biased or unsafe output.

### Suppose you want to generate personalized cold email openers using an LLM. What prompt design strategies would you use to keep outputs relevant and non-generic?
* Make like notice something specific about the person, their roles, their projects.
* Make for to recognize and highlight their works and their success in their project
* Just make sure they understand by the strategies we are curious about them.
