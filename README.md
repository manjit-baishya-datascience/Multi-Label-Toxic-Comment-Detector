# **Toxic Comment Detection**
![Asset 3](https://github.com/user-attachments/assets/5ae1cf01-f6d5-4d9e-93ca-dc001633cebc)

## **Overview**
The Multi-Label Toxic Comment Detection project aims to identify and categorize various types of toxic comments in online forums or social media platforms. This project leverages Natural Language Processing (NLP) and machine learning techniques to classify comments into multiple categories such as toxic, severe toxic, obscene, threat, insult, and identity hate, based on their content.

## **Project Structure**
This project is organized into several key components:

- **Data**: A dataset of comments with multiple labels indicating the types of toxicity present.
- **Preprocessing**: Steps to clean and prepare the comment data for modeling.
- **Modeling**: Machine learning algorithms used to classify the comments into their respective categories.
- **Evaluation**: Assessing the performance of the models using various metrics.
- **Pipeline**: A complete pipeline from data preprocessing to prediction.
- **Testing**: Examples of how the model performs on new, unseen comments.

## **Data**
The dataset contains several columns, with the primary columns being:
- `Comment`: The actual text of the comment.
- `Labels`: Multiple binary columns indicating the presence or absence of each toxicity category (e.g., toxic, obscene, threat).

The data is loaded from a CSV file and initially explored to understand its structure and content.

## **Data Preprocessing**
Effective preprocessing is crucial for building a reliable toxic comment detection model. The preprocessing steps include:

1. **Lowercasing**: Converting all text to lowercase to ensure uniformity, making the model less sensitive to case variations.
2. **Removing Punctuation**: Punctuation marks are removed to simplify the text.
3. **Removing Stop Words**: Common words that do not contribute significantly to the classification are removed.
4. **Tokenization**: Breaking down each comment into individual words (tokens) for better analysis.
5. **Lemmatization**: Reducing words to their root form to treat different forms of a word as the same.
6. **Vectorization**: Transforming the text data into numerical format using techniques like TF-IDF (Term Frequency-Inverse Document Frequency).

## **Modeling**
The processed data is used to train various machine learning models capable of multi-label classification. This project employs classifiers such as **Logistic Regression**, **Random Forest**, and **Support Vector Machine (SVM)**, tailored to handle the multi-label nature of the problem.

## **Evaluation**
The model's performance is evaluated using metrics such as accuracy, precision, recall, F1-score, and Hamming loss. A confusion matrix is also plotted for each label to visualize how well the model distinguishes between the different toxicity categories.

## **Pipeline**
A complete pipeline is created to automate the entire process, from data preprocessing to making predictions on new comments. This pipeline can be integrated into systems for moderating online content and preventing the spread of toxic language.

## **Testing the Model**
The model is tested with various sample comments to demonstrate its effectiveness. For each comment, the model predicts the presence or absence of each toxicity category, with results that align well with expectations.

## **Conclusion**
This project successfully implements a multi-label classification system to detect toxic comments using NLP and machine learning. The system is effective and can be used to enhance content moderation on online platforms.

## **Requirements**
To run this project, you'll need to install the following Python libraries:
- pandas
- numpy
- scikit-learn
- nltk
- matplotlib
- seaborn
