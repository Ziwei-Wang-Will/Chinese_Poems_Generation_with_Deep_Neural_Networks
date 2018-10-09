# Chinese_Poems_Generation_with_Deep_Neural_Networks

<img src="https://github.com/will-zw-wang/Chinese_Poems_Generation_with_Deep_Neural_Networks/blob/master/images/Chinese_Poems_image.jpg" width="800" height="200">

[**Detailed Code and Plotting**](https://github.com/will-zw-wang/Chinese_Poems_Generation_with_Deep_Neural_Networks/blob/master/Chinese_Poems_Generation_with_Deep_Neural_Networks.ipynb)

## Project Objectives

- Constructed a sequence-to-sequence model using Recurrent Neural Network with Long Short-term Memory cells to generate new Chinese poems.
    - We inputed a sequence of words/characters to an RNN so that it could learn the probability distribution of the next word/character in the sequence given the history of previous characters. This would then allow us to generate text one unit at a time.

## Dataset description
- We used [Full Tang poetry(全唐诗)](https://github.com/will-zw-wang/Chinese_Poems_Generation_with_Deep_Neural_Networks/blob/master/data/poetry.txt) as our training data.
- With 49K Chinese poems

## Analysis Structure
1. Preprocessing for language modeling data
2. Constructed a seq2seq model using RNNetwork with LSTM
3. Training and evaluation
4. Output analysis

## Analysis Details

### 1. Preprocessing for language modeling data
- Cleaned noise
- Created a dictionary that maps words to unique IDs
- Converted words to ID
- Reshaped sequences to unified lengths
### 2. Constructed a seq2seq model using RNNetwork with LSTM
- Defined Hyperparameters
- Defined a training operation for an epoch
- Defined an operation for printing test data
- Defined training controller
### 3. Training and evaluation
- Observed loss
- Evaluated on test set
### 4. Output analysis
- Chinese poem generated
    - 君马十年年
    - 时中君安一
    - 里不前既不
    - 龙前食上风
- **Summary**: **Test Perplexity** with 310.66 is too high to generate fluent Chinese poetry, we may need more data to train and improve this model.
