The language Hinglish involves a hybrid mixing of Hindi and English within conversations, individual sentences and even words. 
An example: “nahi mei nahi aa sakta”. Translation: “no, i cannot come.” 
It is gaining popularity as a way of speaking that demonstrates you are modern, yet locally grounded.

Our program aims to detect two things:

1) Whether the word typed is either english or hindi written in english
2) To translate the hinglish word to both: english and hindi

To tackle the first we built a sequence to sequence architecture using tensorflow. 
Sequence-to-sequence learning (Seq2Seq) is about training models to convert sequences 
from one domain (e.g. sentences in English) to sequences in another domain (e.g. the same sentences translated to French).
Seq2Seq is a method of encoder-decoder based machine translation and language processing that maps an input of sequence to 
an output of sequence with a tag and attention value. The idea is to use 2 RNNs that will work together with a special token 
and try to predict the next state sequence from the previous sequence.

econd part of the project was to classify if a given language word was english or hindi. 

To make this classification model we used LSTM. Long short-term memory (LSTM) is an artificial recurrent neural network (RNN) architecture used in the field of deep learning. 
Unlike standard feedforward neural networks, LSTM has feedback connections. It can not only process single data points (such as images), but also entire sequences of data (such as speech or video). 
Our LSTM Model has 3 layers with ReLU and sigmoid as activation functions and binary cross entropy for loss parameters. After training it on 20 epochs we got an accuracy of 83.4%. 
We further deployed this on flask using ngrok. 

![image](https://github.com/kopalsharma19/NLP-Hinglish/assets/43065428/46a82427-f71c-4437-9cf4-d9c773887061)


To read a detailed blog on our project please visit - https://kopalsharma.com/2021/04/13/natural-language-processing-on-hinglish/

Thank you. 

Contributors - 
Kopal Sharma (kopalsharma2000@gmail.com)
Sagarika Raje (raje.sagarika@gmail.com)
