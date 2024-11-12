# StockPricePredictorLLM
Our AI project, which is a LLM-based chatbot that acts as a stock price predictor


## References:

LLM Creation: https://www.freecodecamp.org/news/how-to-build-a-large-language-model-from-scratch-using-python/

https://github.com/Abhishekkr3003/Portfolio-Manager/tree/master


## Contents of premade Folder:

### wizard_of_oz.txt:
This hefty text file serves as a large dataset to train the Bigram Language Model, which is designed to predict the next character in a sequence based on the previous character.

### bigram.ipynb:
Idea is to train a model that can predict the next value in a sequence (e.g. stock prices) based on previous values

### bpe.ipynb:
Training a Byte Pair Encoding (BPE) tokenizer. Reads val_split.txt and writes 5% of its content to a new file tokenizer_training.txt - this is done to create a smaller dataset for training the tokenizer on the latter file.
The trained tokenizer is saved to bpe_tokenizer.json, which can be loaded from here for later use.


### chatbot.py:
This script is designed to create a chatbot using a GPT language model.

