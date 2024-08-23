### Project Tasks Overview

1. **Introduction**
   - This study focuses on emotion classification in tweets, a significant task in Natural Language Processing (NLP). The goal of our project is to perform text classification using advanced artificial intelligence algorithms to accurately label tweets with the emotions expressed by their authors, aiming to achieve increased performance on relevant metrics. Our research investigates and compares various approaches to this task. We evaluate the effectiveness of traditional machine learning methods, such as Logistic Regression and Naïve Bayes, against more advanced deep learning architectures. These include Long Short-Term Memory (LSTM) networks, Gated Recurrent Units (GRU), transformer-based models like BERT, and a more complex model (BERT+BILSTM). By implementing and assessing these diverse AI techniques, we aim to identify the most effective methods for correctly labeling the emotional content of tweets.

2. **Dataset Details**
   - **Name:** EMOTION
   - **Source:** [Hugging Face Datasets](https://huggingface.co/datasets/dair-ai/emotion)
   - **Associated Paper:** ["CARER: Contextualized Affect Representations for Emotion Recognition"](https://aclanthology.org/D18-1404/)
     
3. **Data preprocessing**
   - **Data Cleaning:** Convert to lowercase; Remove punctuation; Remove extra spaces; Stop some words;
   - **Undersamper method:** Use an undersamper method to make the number of train samples of each emotion labels consistent, so that to prevent the model from being biased towards the majority class.

4. **Vectorization**
   We will be employing different vectorization techniques using pretrained embeddings and fine-tuning where necessary:
   - **Word2Vec:** Pretrained vector.
   - **BERT:** Both the use of pretrained vectors and further fine-tuning.

5. **Model Implementation**
   We have been instructed to implement models based on the following architectures:
   - **Transformer-Based Solution:** BERT, BERT-BILSTM.
   - **LSTM/GRU:** LSTM, BI-LSTM, GRU, BI-GRU.
   - **Machine Learning:** Naïve Bayes, Logistic Regression.

6. **Evaluation Metrics**
   - Use the classification report, confusion matrix, and the total F1-score accuracy to evaluate the models' performance initially.
   - Additionally, we use our models to predict some specific sentences to evaluate their performance.

7. **Future work**
   - **Dataset Improvement:** Find or create a richer dataset that does not solely rely on the pattern of "feel" + emotion words. The new dataset should have a more complex structure and accurately label sentiments in sentences with negation.
   - **Model Comparison:** Evaluate the performance of both simple models and complex models (such as BERT-BiLSTM) on this improved dataset. Specifically, assess whether the models can correctly predict sentiments in sentences containing negation.




