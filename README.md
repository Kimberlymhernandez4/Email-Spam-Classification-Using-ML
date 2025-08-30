# Email-Spam-Classification-Using-ML
Multivariable Classification Project to detect spam emails using Spambase, a dataset provided by the University of California Irvine's Machine Learning Repository. 


Access the dataset from UCI'S Machine Learning Repository: https://archive.ics.uci.edu/dataset/94/spambase

# Overview 
---------------------------------------------------------------------------------------

# Problem Domain
Email spam detection is one of the most important features for mailbox websites such as Gmail, Outlook, and Yahoo Mail. These platforms serve a large number of users globally, and unwanted emails can raise serious risks (i.e., phishing attacks, fraud, and malware spread), where safe communication can become compromised. 

Machine learning can offer a reliable solution to this problem domain as it can learn directly from historical data and identify patterns that can distinguish whether an email can (or cannot) be labeled as spam. This supervised learning approach would include using logistic regression, as it is designed for binary classification modeling (1 = True, 0 = False), where true (1) values would confirm spam, and false (0) values would detect that an email is not spam. Furthermore, using numerical features that include the frequency of words, characters, and capital letter usage can be applied to a logistic regression model to estimate the probability that a message belongs to the spam category. 

---------------------------------------------------------------------------------------

# Objective
The main objective for this analysis is to apply logistic regression in order to classify emails as spam or non-spam using the Spambase dataset from the UCI Machine Learning Repository (University of California, Irvine, 1999). The main research question for this project is: “Can Logistic Regression predict the likelihood that an email is spam based on text-related features with great accuracy?” The Logistic Regression model will specifically examine how patterns such as word frequencies, capitalization behaviors, and character frequencies can influence the likelihood of a message being classified as spam. The overall purpose of this study is to evaluate the model’s accuracy, interpretability, and suitability for spam classification, while also identifying which features are most predictive of spam content. 

---------------------------------------------------------------------------------------

# Analysis

---------------------------------------------------------------------------------------

# Exploratory Analysis

The dataset used for this model is the Spambase dataset, which was collected by researchers and made public in 1999 through the UCI Machine Learning Repository. The dataset contains 4,601 mail entries and 57 columns. Independent variables are comprised of 48-word frequency attributes, 6 character frequency attributes, and 3 attributes that measure capitalization patterns (i.e., the avg. length of consecutive capital letters, the longest run of capital letters, and the sum of capital letters in each message). The dependent variable (y label) is the binary classification, which identifies whether the email is spam (1 = True) or non-spam (0 = False). 

---------------------------------------------------------------------------------------

<img width="950" height="342" alt="image" src="https://github.com/user-attachments/assets/6ccd1001-f50a-4d1c-83b0-4b4af4ab627c" />

The three boxplots above provide data visualizations of how selected features are distributed across the binary classification: Spam (1) and Non-Spam (0). 

## **1st Boxplot: Word Frequency**
- Displays the distribution of the variable ‘word_freq_1” by each binary class. Most values for both spam and non-spam emails are below two and are concentrated near zero. More outliers can be seen in the non-spam distribution, with some present in the spam classification. 
---------------------------------------------------------------------------------------

## **2nd Boxplot: Character Frequency:**
- Displays the distribution of the variable ‘char_freq_1’ against each binary class. Similar to the 1st boxplot, most values are closer to zero, and a cluster of outliers can be seen in the non-spam category. This confirms that specific characters are more often used in spam emails and are more commonly found in low-frequency sequences. 

---------------------------------------------------------------------------------------

## **3rd Boxplot: Capitalization:**
- Provides the distribution of  “capital_run_length_average” against each binary class, which measures the average length of consecutive capital letters in an email. The results show that spam emails contain much higher average runs of capital letters compared to non-spam emails. This finding is consistent with the common observation that spam messages often use excessive capitalization for emphasis, which can be seen in the wide range and extreme outliers within the spam class. 

---------------------------------------------------------------------------------------

## **Key Insights Summary from Boxplots:**
- Overall, these visualizations reveal that while most feature values are concentrated near zero, spam emails are more likely to contain higher word frequencies, unusual character usage, and excessive capitalization. These patterns suggest that logistic regression can assess the performance of these specific features to separate spam from non-spam messages effectively.

---------------------------------------------------------------------------------------





---------------------------------------------------------------------------------------


