# Sarcastic-Headline-Detection-with-BERT

Original author of this notebook and repository: Derek Lilienthal
Link to original repo: https://github.com/dblilienthal/Sarcastic-Headline-Detection-with-BERT

### Problem
In this noteook, I will be predicting if a news headline is sarcasm. This News Headlines dataset for Sarcasm Detection is collected from two news website.   
**_The Onion_**, which aims at producing sarcastic versions of current events.   
**_The Huffington Post_**, which is a real (non-sarcastic) news outlet.  

### Context
- `is_sarcastic`: 1 if the headline is sarcastic, otherwise 0  
- `headline`: The headline of the news article  
- `article_link`: The link to the original news article  

### Models
This problem is a binary classification problem where I will be using two models. A baseline of **Naive Bayes** and a more advanced **Deep Neural Network (DNN)** design using **BERT** as a base layer with multiple convolutional and dense layers to predict the sarcastic headlines.  
For implementing **BERT**, I will be fine-tuning BERT by freezing it's trainable layers and only training the additional layers underneath.  

*Note: The results from the DNN were trained on two tesla V100 32GB GPU's*  

### Measure of Success
For this problem, I will define the measure of success by using *accuracy* because the dataset contains almost equal numbers of each predictors.

**Number of binary labels**  
Not Sarcastic: 29,970  
Sarcastic: 25,358

The data in this project was provided by kaggle.com  
https://www.kaggle.com/rmisra/news-headlines-dataset-for-sarcasm-detection

## BERT architecture
<img src='Sarcasm img.png'>
