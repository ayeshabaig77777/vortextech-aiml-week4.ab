Vortex Tech AI/ML Internship - Week 4: Sentiment Analysis Model

What I built
This project is a sentiment analysis model that classifies movie reviews 
as positive or negative, using the IMDB Dataset of 50K Movie Reviews. 
It covers the full NLP pipeline: text cleaning, TF-IDF feature extraction, 
model training, evaluation, and testing on custom example sentences.

What was done
- Loaded the IMDB movie reviews dataset and checked class balance
- Cleaned the text: lowercased, removed HTML tags, punctuation, and extra whitespace
- Converted cleaned text into numeric features using TF-IDF (top 5,000 words)
- Split data into 80% training / 20% testing sets
- Trained a Logistic Regression model and evaluated it using accuracy, F1-score, 
  and a confusion matrix
- Trained a Multinomial Naive Bayes model for comparison
- Tested the model on 3 original example sentences
- Summarized the full pipeline, results, and model limitations

Results
- Logistic Regression Accuracy: [your actual number]
- Logistic Regression F1-score: [your actual number]

Limitations
The model relies on word frequency (TF-IDF) and has no real understanding 
of context, word order, negation, or sarcasm — e.g. it can misread phrases 
like "not bad at all" due to the presence of the word "bad".

How to run it
1. Clone this repository
2. Install requirements: `pip install pandas scikit-learn`
3. Download the "IMDB Dataset of 50K Movie Reviews" from Kaggle and place 
   `IMDB Dataset.csv` in this folder
4. Open `week4_sentiment.ipynb` in Jupyter Notebook or VS Code
5. Run all cells
