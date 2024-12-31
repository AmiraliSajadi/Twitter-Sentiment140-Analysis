# Twitter-Sentiment140-Analysis

This project uses an LSTM-based neural network to perform binary classification of the **Sentiment140 dataset**. The model predicts whether a given tweet expresses **positive** or **negative sentiment**.

<p align="center">
  <img src="https://user-images.githubusercontent.com/48511939/127962271-673b57a8-8aaa-4907-86fb-8831d669d355.jpg" width="500"/> 
</p>

## Features
- **Data Preprocessing**: Includes tokenization, cleaning, and lemmatization of tweets to create structured input for the model.
- **Custom Embedding Layer**: Utilizes pre-trained **GloVe embeddings** for word representation, ensuring robust vectorization of textual data.
- **Model Design**: A two-layer bidirectional LSTM with dropout for regularization, trained using the Adam optimizer.
- **Performance**: Trained on a subset of the Sentiment140 dataset (~1.6M tweets), achieving effective sentiment classification.

## Example Predictions
<p align="center">
  <img src="https://user-images.githubusercontent.com/48511939/127893581-681b708b-ffc7-4da9-90f8-f51dd2dd363f.png" width="600"/>
</p>
- Sentences closer to **1.0** indicate positive sentiment.
- Sentences closer to **0.0** indicate negative sentiment.

## Project Highlights
1. **Data Preprocessing**:
   - Tokenization using NLTK.
   - Lemmatization with POS tagging.
   - Noise removal (URLs, mentions, punctuation, and stopwords).
2. **Visualization**: Generates word clouds of frequent words for exploratory data analysis.
3. **Model**:
   - Embedding layer built from GloVe.
   - Bidirectional LSTMs for context-aware text analysis.
   - Dropout for overfitting prevention.
4. **Custom Predictions**: Easily classify custom text strings using the trained model.

## Results
The model can predict custom sentences with confidence, such as:
```python
print(predict_custom_string("I love chocolate"))  # Output: ~0.93 (positive)
print(predict_custom_string("I hate chocolate"))  # Output: ~0.09 (negative)
```

## Dataset
The Sentiment140 dataset is used for training and testing. It contains 1.6 million tweets labeled as positive (4) or negative (0).

##
For more details, refer to the notebook.
