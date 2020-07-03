# QA_SQuAD

A Question-Answer system built on the SQuAD 1.1 dataset. 
Uses a doc2vec model trained on the contexts and questions provided in this dataset. 
Given a context and a question based on it, the system computes cosine similarity between each sentence of the context and the question.
Answer index is predicted by finding the index of the sentence with maximum cosine similarity with the question. 
Currently gives a 49% accuracy for the same. 
Create_embeddigs.ipynb, consists of training the model, and then storing the embeddings for the contexts and questions into a pickle file. 
Unsupervised.ipynb, works with the embeddings and finds out the sentence index with maximum similarity to the question.
UI.ipynb is a user interface which uses the trained doc2vec model, infers vectors for new contexts and questions, and finally displays the answer 
after finding the sentence with highest cosine similarity with the question.


 
