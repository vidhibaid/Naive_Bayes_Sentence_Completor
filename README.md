# NaiveBayesSentenceCompletor
This project uses naive Bayes probability analysis to predict words to complete incomplete sentences and classify them into categories. 

Text Analysis with Naive Bayes
1) Sentence classification: 

Consider the files traindata.csv and testdata.csv. In these files, each row contains a sentence which belongs to one of 4 categories (science, sports, business, covid crisis). Learn a Naive Bayes classifier to predict the category of each sentence, based on the words in it (neglecting stop words). Use the training set to estimate the prior distribution over the class labels and class-conditional probabilities, i.e. the probability of each word occurring in a sentence having a particular class label. For each test sentence, your output should be the posterior distribution over the labels.

[Trick: never set p(w|Y=k)=0 for any word w and label k, even if word w never exists in any sentence with label k. Assign a small probability like 0.01. Adjust the probabilities of other words too, such that you get a proper conditional distribution]

i) Construct the vocabulary without stop-words

ii) Calculate the prior distribution of the labels

iii) Calculate the class-conditional probabilities of each word in the vocabulary, for each topic

iv) For each test sentence, create the posterior distribution over the labels

2) Sentence Completion

Consider the datasets "40.csv" and "10.csv". In each sentence of "10.csv", the last word is not provided. The task is to predict it based on the remaining words in the sentence. Build your vocabulary from "40.csv" (except stop words). Assume that the missing words are part of this vocabulary. Consider this as a classification problem, where each word in the vocabulary may be considered as a class label. Use the Naive Bayes classifier to make probabilistic estimates of the missing words.

i) Create the vocabulary without stop-words 

ii) Estimate the prior probabilities of all "labels", i.e. words in vocabulary 

iii) Estimate the class-conditional probabilities of all words 

iv) In each test sentence, calculate the most likely word in the missing position along with probability 
