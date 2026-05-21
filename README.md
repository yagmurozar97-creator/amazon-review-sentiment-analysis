# Amazon Product Review Sentiment Analysis with NLP and Machine Learning

This project analyzes Amazon product reviews using exploratory data analysis (EDA), natural language processing (NLP), sentiment analysis, and machine learning techniques to uncover customer sentiment patterns and predictive review language.

The project focuses on understanding customer behavior, product satisfaction, review sentiment, and language patterns within Amazon customer reviews.

---

## Project Objectives

- Analyze product ratings and customer review behavior
- Evaluate category-level product performance
- Explore customer sentiment patterns in review text
- Apply NLP preprocessing techniques to textual data
- Build a machine learning model for sentiment classification
- Interpret predictive language patterns used in customer reviews

---

## Dataset

The dataset contains Amazon product information including:

- Product names and categories
- Discounted and actual prices
- Customer ratings and review counts
- Review titles and review content
- Product and image links

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- NLTK
- WordCloud
- TextBlob
- Scikit-learn

---

## Project Workflow

### 1. Data Cleaning and Preprocessing

#### Steps Performed

- Removed currency symbols and percentage signs
- Converted numerical columns into proper numeric formats
- Cleaned comma-separated review counts
- Handled invalid values and missing observations

---

### 2. Exploratory Data Analysis (EDA)

#### Analyses Performed

- Product rating distribution analysis
- Category-level performance evaluation
- Discount and pricing analysis
- Custom product scoring analysis
- Value score comparison across products and categories

#### Key Insights

- Most products received high customer ratings
- Ratings were heavily concentrated between 4.0 and 4.5
- Electronics products had the highest review engagement
- Low-cost products often achieved strong value scores

---

### 3. NLP and Text Processing

#### Text Preprocessing

- Lowercasing
- URL removal
- Stopword removal

#### Word Frequency Analysis

- Most common review words
- Filtered keyword analysis
- Word cloud visualization

#### Sentiment Analysis

Sentiment scores were generated using TextBlob and categorized into:

- Positive
- Negative
- Neutral

#### Sentiment Insights

- Customer reviews were overwhelmingly positive
- Positive sentiment dominated across most product categories
- Electronics and Home & Kitchen products showed relatively lower sentiment despite maintaining high ratings

---

### 4. Machine Learning Model

#### TF-IDF Feature Extraction

Customer reviews were transformed into numerical vectors using TF-IDF vectorization, allowing machine learning algorithms to analyze textual patterns efficiently.

#### Logistic Regression Classification

A Logistic Regression model was trained to classify customer reviews as Positive or Negative.

To address severe class imbalance in the dataset, balanced class weighting was applied to improve negative sentiment detection.

#### Model Evaluation

The model was evaluated using:

- Accuracy Score
- Classification Report
- Confusion Matrix

#### Model Performance

- Accuracy: approximately 98%
- Strong performance on positive review classification
- Balanced class weighting improved negative sentiment detection
- Model evaluation revealed the importance of handling class imbalance in sentiment classification tasks

---

### 5. Model Interpretability

The coefficients of the Logistic Regression model were analyzed to identify the words that most strongly contributed to Positive and Negative sentiment predictions.

#### Positive Predictive Words

Examples:

- good
- quality
- easy
- works
- best

#### Negative Predictive Words

Examples:

- poor
- waste
- bad
- slow
- difficult

This analysis improved model interpretability by revealing the language patterns driving sentiment predictions.

---

## Business Applications

This project demonstrates how NLP and machine learning can support:

- Customer satisfaction monitoring
- Product quality evaluation
- Review-based product analytics
- Automated sentiment classification
- Business decision-making using customer feedback

---

## Conclusion

This project combined exploratory data analysis, natural language processing, sentiment analysis, and machine learning techniques to analyze Amazon product reviews.

The analysis revealed overwhelmingly positive customer sentiment overall, while also identifying specific language patterns associated with dissatisfaction and product-related issues.

Although the initial classification model achieved very high accuracy, class imbalance limited its ability to detect minority negative reviews effectively. Applying balanced class weighting improved the model’s performance on negative sentiment classification.

The project demonstrates the effectiveness of NLP and machine learning approaches for extracting actionable business insights from customer review data while also highlighting the importance of model interpretability and class imbalance handling in real-world machine learning applications.

---
