# Project 1 Generative Text

Chandhini Grandhi, cgrandhi@ucsd.edu


## Abstract

Are you one of those people who felt sad when the popular 90s sitcom - FRIENDS ended? Machine Learning to the rescue! In this project, I will be generating a fake script for the popular TV series. 

![Alt Text](https://in.pinterest.com/pin/462815299207862711/?nic=1)

The dataset that will be used in this project is 10 seasons of Friends episodes obtained from https://fangj.github.io/friends/ .The project builds a 2 layer RNN based on LSTM. The data is processed and  tokenized to be represented as a bag of words. The processed data will then be fed to a 2-layer neural network implemented in Pytorch. I plan to experiment with it by changing the number of training epochs, Embedding dimensions and Batch size. Once the hyperparameters are finalized, the project will generate 100 scenes with each character as key word, which will be combined and cleaned to generate one episode. 


## Model/Data

The files included in this repository are
- Dataset - ./data/friends.txt
- Preprocess data - ./preprocess.p
- trained data - ./trained_rnn.pt
- Intermediate Outputs - ./Output
- Final episode - The Fake Script.txt

## Code

The code for generating this project is present in  :
- Generative-text-TVscript.ipynb 

## Results

The results are present in the Generated test folder. Below are the statistics for each result which was obtained by modifying the hyper parameters

> generated_script_1.txt
>> Dataset:10,000,
>> Epochs: 10, 
>> Batch size:128,
>> Loss: 3.98

> generated_script_2.txt
>> Dataset:30,000,
>> Epochs: 10,
>> Batch size:128,
>> Loss: 3.23

> generated_script_3.txt
>> Dataset:30,000,
>> Epochs: 20,
>> Batch size:128, 
>> Loss: 2.74

> generated_script_4.txt
>> Dataset:30,000,
>> Epochs: 10,
>> Batch size:64, 
>> Loss: 2.664

> generated_script_5.txt
>> Dataset:100,000 
>> Epochs: 20 
>> Batch size:128 
>> Loss: 3.161

> generated_script_6.txt:
>> Datatset : 100,000,
>> Epochs : 20,
>> Batch size: 64,
>> Loss: 3.397


## Technical Notes

The code requires the following versions of packages installed on the Datahub
1. torch : 1.2.0
2. numpy : 1.16.4


## Reference

References to any papers, techniques, repositories you used:
- Blog posts<br />
  -[Building RNN with Pytorch](https://blog.floydhub.com/a-beginners-guide-on-recurrent-neural-networks-with-pytorch/)<br />
  -[Understanding LSTM](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)<br />
  -[Understanding RNN](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)<br />
  -[NLP with Pytorch](https://pytorch.org/tutorials/intermediate/char_rnn_classification_tutorial.html)<br />
