## Spam Message Classifier

A machine learning–based spam message classifier built using Python and scikit-learn.  
The model classifies SMS messages as **Spam** or **Not Spam** using a real-world dataset.

## Overview

This project demonstrates an end-to-end machine learning pipeline for text classification.
It uses a real SMS dataset and applies Natural Language Processing (NLP) techniques
to detect spam messages with high accuracy.

The project is designed to be simple, interpretable, and suitable for beginners
while still reflecting real-world machine learning practices.

## Approach & Methodology

1. **Dataset**
   - Used the SMS Spam Collection dataset containing 5,574 labeled messages.
   - Labels include `spam` and `ham` (non-spam).

2. **Text Processing**
   - Messages are converted into numerical features using the Bag-of-Words model.
   - English stopwords are removed during vectorization.

3. **Model**
   - Multinomial Naive Bayes classifier is used.
   - This model is well-suited for text classification problems.

4. **Evaluation**
   - The dataset is split into training and testing sets (80% / 20%).
   - The model achieves approximately **98–99% accuracy** on test data.

5. **Prediction**
   - Users can enter custom messages via the command line.
   - The model predicts whether the message is Spam or Not Spam.


## Technologies Used
- Python 3
- pandas
- scikit-learn
- Multinomial Naive Bayes

## Project Structure

```
spam-classifier/
│
├── spam_classifier.py        # Main program
├── SMSSpamCollection         # Dataset file
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
```

## How to Run
1. Clone the repository
```bash
git clone https://github.com/diyaj02/Spam-message-classifier.git
cd Spam-message-classifier  
```

2. Install dependencies 

pip install -r requirements.txt

3. Run the program

python spam_classifier.py

4. Enter an SMS message when prompted to classify it as Spam or Not Spam. 


## Results

- The model achieves an accuracy of approximately **98.8%** on the test dataset.
- It successfully classifies unseen SMS messages as **Spam** or **Not Spam**.

## Example Output

```
Enter a message (or type exit): WINNER! You have won a free recharge. Call now
Spam

Enter a message (or type exit): Hey, I will reach college in 10 minutes
Not Spam
```
