# IMDB Movie Review Sentiment Analysis

This project demonstrates sentiment analysis on the IMDB dataset of 50,000 movie reviews, using machine learning techniques to classify reviews as positive or negative.

## Dataset Overview

- 50,000 highly polar movie reviews from IMDB
- Balanced dataset: 25,000 positive and 25,000 negative reviews
- 40,000 reviews used for training and 10,000 for testing

## Project Features

- Text preprocessing (HTML tag removal, stopword filtering, lemmatization)
- Feature extraction using TF-IDF vectorization
- Multiple classification algorithms compared:
  - Logistic Regression (achieved best performance)
  - Naive Bayes
  - Random Forest
  - Linear SVM
- Model evaluation and error analysis
- Visualization of important words for classification

## Results

- **Best Model:** Logistic Regression with 88.51% accuracy
- Consistent performance across both positive and negative classes
- The model identified key sentiment indicators in reviews:
  - Positive reviews: "great", "excellent", "perfect", "wonderful"
  - Negative reviews: "worst", "waste", "bad", "awful", "boring"

## Implementation Details

The project includes:
1. Data exploration and preprocessing
2. Feature extraction with TF-IDF
3. Model training and evaluation
4. Hyperparameter optimization
5. Error analysis
6. Prediction function for new reviews

## Usage

The final model can be used to analyze new movie reviews:

```python
# Example usage
result = predict_sentiment("This movie was absolutely fantastic! I loved every moment of it.")
print(f"Prediction: {result['prediction']}")
print(f"Confidence: {result['confidence']:.4f}")
```

## Future Improvements

Potential enhancements could include:
- Implementing deep learning models (LSTM, Transformers)
- Adding a web interface for real-time sentiment analysis
- Exploring additional features beyond word frequency

## Requirements

- Python 3.x
- pandas
- scikit-learn
- numpy
- matplotlib
- NLTK
