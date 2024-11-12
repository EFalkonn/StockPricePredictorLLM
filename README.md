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

### data-extract.py:
Designed to process and extract text data from compressed .xz files. 
The process_file function reads the content of a compressed .xz file, writes it to an output file, and returns the set of unique characters found in the text. The xz_files_in_dir function scans a directory and returns a list of .xz files. The process_files_in_parallel function processes multiple files in parallel using a ProcessPoolExecutor. It updates the vocabulary set with unique characters from each file.
Basically, this script is used to preprocess large text datasets by extracting and preparing the data for training language models. The extracted text and vocabulary can then be used to train models that predict stock prices based on historical data.


### gpt-v1.ipynb:
Designed to train a GPT language model.
