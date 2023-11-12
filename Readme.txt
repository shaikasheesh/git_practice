Back to NLP basics:

I had a good time working on Text classification project.
For a quick debrief here are the steps I have included in my pipeline
	1) Data Pre-processing:
		· Only allowed alphabets and numbers on the text data, rest is replaced with space  
		· Lowered the sentence case and Applied stemming 
	2) As part of EDA, 
		· Generated word cloud across different sentiment categories
		· Visualized the distribution of the labelled data
	3) Performed Topic modelling using sk-learn LDA to generate different topics hidden in the text 
	4) Feature Extraction:
		· Applied TfIdf vectorizer to extract the features from the text
	5) Using ensemble techniques, performed classification task
	6) Using LSTM RNN,
		· Prepared word embeddings using one hot encoding for  text data
		· Padding is done to ensure all the input sentences have same length
		· Built LSTM RNN network using tf & keras library
			§ Output activation as softmax
			§ Loss considered is sparse_categorical_cross_entropy
			§ Adam optimizer is used
	7) Using Transformers
		· Utilized hugging face pipeline library to download the pre-trained distilled BERT model for classifying the sentiments of the input text
		· Fine-tuned distilled BERT and trained on the input data for better results.
			§ Autotokenizer for the BERT model is called using hugging face API
			§ Tensorflow data set loader is used to transform the pandas data frame for efficient training
			
	

