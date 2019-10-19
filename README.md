# Project 1 Generative Text

Chandhini Grandhi, cgrandhi@ucsd.edu


## Abstract

The project I will be working on is  to generate TV scripts for the popular 90s sitcom - FRIENDS. I am a huge fan of the TV series and have watched all 10 seasons multiple times. In this project, I am going to build a 2 layer RNN which can be trained to generate a new script for the series (Hopefully, it will be released as Season 11). The dataset I am going to use is 100,000 line FRIENDS Transcript obtained from https://fangj.github.io/friends/ . The data has to be processed and  tokenized to be represented as a bag of words. The processed data will then be fed to a 2-layer neural network implemented in Pytorch. I plan to experiment with it by changing the number of training epochs, Embedding dimensions and Batch size. 


## Model/Data

The files included in this repository are
- Dataset - ./data/friends.txt
- Preprocess data - ./preprocess.p
- trained data - ./trained_rnn.pt
- Intermediate Outputs - ./Output
- Final episode - The Fake Script.txt

## Code

Your code for generating your project:
- Generative-text-TVscript.ipynb - your generation code

## Results

The results are present in the Generated test folder. Below are the statistics for each result which was obtained by modifying the hyper parameters

> generated_script_1.txt
>> Dataset:10,000 
>> Epochs: 10 
>> Batch size:128 
>> Loss: 3.98

> generated_script_2.txt
>> Dataset:30,000 
>> Epochs: 10 
>> Batch size:128 
>> Loss: 3.23

> generated_script_3.txt
>> Dataset:30,000 
>> Epochs: 20 
>> Batch size:128 
>> Loss: 2.74

> generated_script_4.txt
>> Dataset:30,000 
>> Epochs: 10 
>> Batch size:64 
>> Loss: 2.664

> generated_script_5.txt
>> Dataset:100,000 
>> Epochs: 20 
>> Batch size:128 
>> Loss: 3.161

> generated_script_6.txt:
>> Datatset : 100,000
>> Epochs : 20
>> Batch size: 64
>> Loss: 3.397


## Technical Notes

The code requires the following versions of packages installed on the Datahub
1. torch : 1.2.0
2. numpy : 1.16.4


## Reference

References to any papers, techniques, repositories you used:
- Blog posts
  -[Building RNN with Pytorch](https://blog.floydhub.com/a-beginners-guide-on-recurrent-neural-networks-with-pytorch/)
  -[Understanding LSTM](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)
  -[Understanding RNN](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)
  -[NLP with Pytorch](https://pytorch.org/tutorials/intermediate/char_rnn_classification_tutorial.html)
