# Natural-Language-Processing
This repository contains some assignment for NLP including:
1. Multilabel classification models using linear models to predict tags for a dataset of StackOverflow questions. This notebook compares BOW and TF-IDF approches.
2. A model for Name Entity Recognision NER problem using Bidirectional RNN models such as GRU in keras API. Evaluation of the model shows how the model performance 
on predicting each tag. We use a small dataset from Twitter.  
3. It compares two imbdeddings for finding similarity between texts. This is very importnt problem and the success of the model for large datasets 
greatly depends on the embedding chosen. One embedding is a pre-trained W2V model from Google trained on Google News (about 100 billion words). The second 
representation is using StarSpace that we train over StackOverflow data sample. The benefit of using StarSpace here is that it can be customized for the particular 
task in hand rather than just providing a general purpose embedding. We use a couple of metrics to compare the performance of these embeddings for 
finding duplicate questions in StackOverflow.
4. Legendry Seq2Seq model has many applications such as NMT, Text Summerization or Conversaional Modeling. We use a simple Seq2Seq model to make a 
simple calculator. This model does not use Attention mechanism.
5. Finally, the last notebook combines the result of the previous ones 1-3 into a working chatbot using Telegram Chatterbot specialized for directing 
programming-related questions to related threads on StackOverflow, which I hosted it on AWS. The chatbot consists of a _dialogue manager_ that 
distinguishes general guestions from technical ones using a classification model (intent classifier). If the question is not a ordinary dialogue type, a 
classifier predicts a tag for it and the bot directs the user to the appropriate thread on StackOverflow to see the answer. 
We can also train our own conversational model by a Seq2Seq model instead of using a pretrained model provide by ChatterBot on Telegram (or any pther provider).

These are assignments I did for a course here: https://www.coursera.org/learn/language-processing/home/welcome
