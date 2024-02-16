The language Hinglish involves a hybrid mixing of Hindi and English within conversations, individual sentences and even words. 
An example: “nahi mei nahi aa sakta”. Translation: “no, i cannot come.” It is gaining popularity as a way of speaking that demonstrates you are modern, yet locally grounded.

Our program aims to detect two things:

1) Whether the word typed is either english or hindi written in english
2) To translate the hinglish word to both: english and hindi

To tackle the first we built a sequence to sequence architecture using tensorflow. 
Sequence-to-sequence learning (Seq2Seq) is about training models to convert sequences 
from one domain (e.g. sentences in English) to sequences in another domain (e.g. the same sentences translated to French).
Seq2Seq is a method of encoder-decoder based machine translation and language processing that maps an input of sequence to 
an output of sequence with a tag and attention value. The idea is to use 2 RNNs that will work together with a special token 
and try to predict the next state sequence from the previous sequence.
