Flipkart Product Reviews Sentiment Analysis Project

Project Overview
Customer feedback is highly valuable for e-commerce platforms to understand product performance and user satisfaction. This project focuses on building a Machine Learning model to automatically analyze and classify Flipkart product reviews as either Positive or Negative based entirely on the textual content of the review.
Dataset Details
The dataset contains user reviews and numerical ratings from Flipkart. To train the model, the ratings were converted into binary sentiment labels. Ratings of 4 and 5 are mapped to Positive, while ratings of 1, 2, and 3 are mapped to Negative.
Technology Stack and Tools
The project is written in Python and developed within a Jupyter Notebook. It utilizes several key libraries: Pandas for data manipulation, NLTK and regular expressions for text cleaning and stopword removal, Scikit-learn for TF-IDF vectorization, model building, and evaluation, and finally Matplotlib, Seaborn, and WordCloud for exploratory data analysis and visualization.
Project Workflow
The workflow is divided into several clear steps. First, during data preprocessing, missing values and duplicates are handled. The raw review text is cleaned by converting it to lowercase, stripping out punctuation and numbers, and removing common English stopwords that do not contribute to sentiment.
Next, during Exploratory Data Analysis, the class distribution is visualized to understand the balance of the data. Word clouds are generated to identify the most frequent terms used in positive and negative contexts, and a correlation analysis proves that the length of a review does not correlate with its sentiment.
The cleaned text is then mathematically represented using Term Frequency-Inverse Document Frequency (TF-IDF), capped at 5000 features. Finally, four different classification algorithms are trained on this data: Logistic Regression, Naive Bayes, Random Forest Classifier, and Support Vector Machine.
Results and Conclusion
The Support Vector Machine outperformed the other models, making it the final choice for the prediction pipeline. It achieved an accuracy of 87.54 percent and an F1-Score of 92.51 percent. The model successfully identifies subtle complaints in negative reviews and reliable praise in positive reviews.

<img width="823" height="456" alt="Screenshot 2026-06-20 210421" src="https://github.com/user-attachments/assets/75d593ea-96cb-4384-9ba8-c0f3e2aa5fe1" />
