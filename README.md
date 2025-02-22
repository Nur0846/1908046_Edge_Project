# 1908046_Edge_Project
### **Project Overview**  

This thesis addresses the challenges associated with freedom of speech on the internet and the misuse of social media platforms like Twitter. The increasing spread of harmful content on these platforms highlights the need for an effective solution. To tackle this issue, we conduct a thorough review of existing research, identify gaps, and propose an improved approach.  

Our methodology involves using a publicly available dataset from CrowdFlower and applying Natural Language Processing (NLP) techniques. We begin by analyzing the dataset, followed by text pre-processing to refine the data by removing noise such as punctuation, stopwords, URLs, and mentions. After obtaining a cleaner dataset, we proceed with feature engineering, where we extract key linguistic and statistical features. These features are grouped into different sets and evaluated using various machine learning classifiers to assess their impact on classification performance. Finally, we conduct a detailed analysis of the results, examining cases of misclassification and their underlying causes.  

### **Key Findings**  

- **Logistic Regression** performs well across most feature sets, except for F7, where it fails to classify the “hate” label accurately.  
- **Random Forest** delivers strong performance, particularly with F1 (TF-IDF scores), but its accuracy drops when TF-IDF features are excluded.  
- **Naïve Bayes** struggles with overall classification but performs better with feature set F7.  
- **Support Vector Machine (SVM)** maintains consistent accuracy across all feature sets, except for F4 and F7.  
- **TF-IDF scores (F1)** emerge as the most influential feature for effective hate speech detection.  
- **Sentiment scores** help distinguish between hate speech and offensive language, while **Doc2Vec embeddings** have minimal impact.  
- **Random Forest** demonstrates the best overall performance across all feature sets.  

### **Summary**  

The project begins with data collection, a challenging task due to the subjective nature of hate speech. To enhance data quality, we apply text pre-processing techniques such as tokenization, stopword removal, and stemming. Feature extraction follows, incorporating n-gram TF-IDF weights, sentiment polarity scores, Doc2Vec embeddings, and readability metrics. These features are grouped into various sets and tested across multiple machine learning models.  

The study highlights the complexity of distinguishing hate speech from offensive language. Our findings emphasize the value of the selected features in improving classification accuracy and contribute to the ongoing efforts in detecting toxic language on social media. Further analysis of feature selection and error patterns could lead to more robust classification techniques and improved hate speech detection methods.
