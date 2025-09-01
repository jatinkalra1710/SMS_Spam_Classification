# 📱 SMS Spam Classification

This project builds and evaluates multiple machine learning models to classify SMS messages as spam or ham (non-spam). It uses a diverse dataset sourced from Kaggle and applies standard NLP preprocessing and classification techniques.

## 📂 Dataset

- **Source**: [SMS Spam Collection - A More Diverse Dataset](https://www.kaggle.com/datasets/thedevastator/sms-spam-collection-a-more-diverse-dataset)
- **Format**: CSV
- **Columns**:
  - `sms`: The message content
  - `label`: Binary label (0 = ham, 1 = spam)

## 🧪 Preprocessing

- Removed English stopwords using NLTK
- Transformed text data using `TfidfVectorizer`
- Split into training and test sets (80/20)

## 🧠 Models Used

| Model                         | Description                          |
|-------------------------------|--------------------------------------|
| Naive Bayes                   | Fast and effective for text data     |
| Logistic Regression           | Linear model with regularization     |
| Support Vector Machine (SVM)  | Kernel-based classification          |

## 📊 Evaluation Metrics
<img width="606" height="124" alt="image" src="https://github.com/user-attachments/assets/3ed3c75e-8ccf-439b-8263-40c4b4a6650e" />

Each model is evaluated using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**

All metrics are computed with `pos_label=1` to focus on spam detection performance.
