# Sentiment-Analysis-for-Financial-Markets
This project builds an advanced sentiment analysis tool using deep learning techniques. The model classifies financial texts into Positive, Neutral, or Negative sentiments, aiding in financial market decision-making.

**Dataset**
Dataset Source:
Financial PhraseBank dataset containing phrases labelled as Positive, Neutral, or Negative.
Dataset Preparation:
Cleaning:
Removed special characters, punctuation, and stopwords.
Lowercased all text.
Label Encoding:
Mapped sentiments to integers: Positive=2, Neutral=1, Negative=0.
**Workflow**
Data Preprocessing
Tokenised words into sequences using Keras Tokenizer.
Padded sequences to ensure uniform length (100 tokens).
**Model Architectures**
BiLSTM: Captures bidirectional sequential context.
BiLSTM + Attention: Adds attention for interpretability.
CNN + BiLSTM: Combines CNN for local patterns with BiLSTM for context (final model).
Training and Evaluation
Models were trained for 5 epochs with validation splits.
The CNN + BiLSTM model achieved the best test accuracy of 74.41%.
**Final Model**
The CNN + BiLSTM was selected as the best model based on accuracy and performance.
Results
Best Model: CNN + BiLSTM
**Test Accuracy: 74.41%**
Strengths: Combines local pattern recognition (CNN) with contextual understanding (BiLSTM).

**Future Work**
Explore transformer models (e.g., BERT) for potentially higher accuracy.
Add more training data for improved generalisation.
Deploy the model in a web application for real-world use.
