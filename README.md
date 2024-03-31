# Spam Classification using Naïve Bayes

This project focuses on classifying SMS messages as either spam or non-spam using the Naïve Bayes classifier. The dataset used for this task is the Spam SMS dataset.

## Dataset Overview

- The dataset contains SMS messages labeled as spam or non-spam.
- Columns: 'class' for the message label and 'sms' for the SMS content.

### Data Preprocessing

The following preprocessing steps were performed on the dataset:

1. **Drop unnecessary columns:** Removed columns 'Unnamed: 2', 'Unnamed: 3', 'Unnamed: 4'.
2. **Rename columns:** Renamed columns 'v1' to 'class' and 'v2' to 'sms'.
3. **Remove duplicates:** Removed duplicate entries from the dataset.
4. **Visualize data:** Created histograms of message lengths for both spam and non-spam messages.

### Text Preprocessing

Text preprocessing steps include:

- **Lowercasing:** Convert all text to lowercase.
- **Tokenization:** Split text into individual words.
- **Removing Special Characters:** Removed special characters from the text.
- **Removing Stop Words and Punctuation:** Removed stopwords and punctuation marks from the text.
- **Stemming:** Reduced words to their base or root form using stemming.

### Feature Extraction

For feature extraction, TF-IDF vectorization was performed using the TfidfVectorizer from sklearn. The maximum number of features was set to 3000.

### Model Training

The dataset was split into training and testing sets using a test size of 20% and a random state of 2. A Multinomial Naïve Bayes classifier was trained using the training dataset, and the accuracy of the model was evaluated on the test dataset.

The model achieved an accuracy of 0.9709864603481625.

