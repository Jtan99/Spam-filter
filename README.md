# SMS Spam Filter

**Table of Contents**
- [Project Objective](#project-objective)
- [Data Source](#data-source)
- [Key Features](#key-features)
- [Project Details](#project-details)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Project Outcome](#project-outcome)
- [Future Directions](#future-directions)
## Project Objective

The SMS Spam Filter project aims to create a robust machine learning model capable of effectively filtering out spam text messages while minimizing false positives to ensure that legitimate messages are not classified as spam.

## Data Source

The project utilizes an open-source dataset with two columns: the first column contains labels "spam" or "ham" (where "spam" represents spam messages, and "ham" represents legitimate messages).

## Key Features

- Extensive preprocessing techniques, including label encoding ("ham" to 0 and "spam" to 1) and the use of regular expressions to identify and replace URLs, phone numbers, and currency symbols with unique identifiers.
- Removal of English stop words and punctuation from text data.
- Application of stemming to keep only word stems as features.

## Project Details

The heart of the project lies in feature engineering in the context of Natural Language Processing (NLP). In NLP, a "feature" refers to a characteristic or property extracted from text data. In this project, individual words, stemming from the text data, are used as tokens/features for model training.

## Technologies Used

- Jupyter Notebook for interactive data analysis and model development.
- NLTK (Natural Language Toolkit) for NLP operations.
- Scikit-learn (sklearn) for machine learning tasks.
- Pandas and NumPy for data manipulation.

## Getting Started

To set up and run this project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Jtan99/Spam-filter.git

2. **Navigate to the Project Directory**:
   ```bash
   cd Spam-filter

3. **Create and activate virtual Environment**:
   ```bash
   python -m venv venv
   venv\Scripts\activate

4. **Install Dependencies**:
   ```bash
   pip install nltk==3.7.0 scikit-learn==0.24.2 pandas==1.2.4 numpy==1.19.5

4. **Run the Jupyter Notebook**:
   ```bash
   jupyter notebook

## Project Outcome
The project successfully demonstrates advanced analysis skills and builds a highly accurate spam filter model. An ensemble model, comprising several machine learning algorithms, achieves an impressive accuracy rate of 98.99% with no false positives. The model effectively identifies spam messages containing phone numbers, URLs, and specific keywords such as "free" and "urgent." It's noted that KNN is not suitable for this task due to low correlation among tokens.

## Future Directions
For future improvements, it's recommended to acquire a more balanced dataset with a larger proportion of spam messages, as the current dataset is skewed towards legitimate messages. This can further enhance the model's ability to detect spam effectively.

This project showcases the successful use of NLP and machine learning techniques for text classification, resulting in a valuable SMS spam filter with high accuracy and minimal false positives.