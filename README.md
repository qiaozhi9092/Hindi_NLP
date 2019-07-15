## Hindi NLP project

### The goal of this project is to practice the state-of-art NLP method on Hindi language

#### Intro
The NLP has been widely used and developed in English language, however it is not as developed in other languages as in English. A lot of the time it is simply becasue it takes too much time and data to develope a new text processing tool for each of its language varieties. 

Hindi is one of the most used languages in India. The difficulities of applying NLP tool to Hindi are: 
- Lack of available libraries
- Tokenization
- A lof of NLP processing methods based on English(stemming, lemmatization, TF-IDF, etc.) are not suitable
- Lack of data

To try to tackle the above issues, the SentencePiece tokenizer released by Google is a great option. It has some advantages like:
- Purely data driven: pre-tokenization is not always required. It can train on the raw sentences. 
- Language independent: Works for all the languages. 

To define SentencePiece: it is a re-implementation of sub-word units, an effective way to alleviate the open vocabulary problems in neural machine translation. 

More details about SentencePiece please go to: https://github.com/google/sentencepiece

#### Data
The data consists of 4335 Hindi documents with tags from the BBC Hindi News website. 
There are 14 unique categories. Each document has exactly one tag associated with it. These are the tags: india, pakistan, news, international, entertainment, sport, science, china, learningenglish, social, southasia, business, institutional, multimedia.

More details about the dataset please go to: https://github.com/NirantK/hindi2vec/releases/tag/bbc-hindi-v0.1

#### Result
Accuracy: 0.412240

#### Future Improvement 
This project by no means is a finished project, it can be improved in many aspects, namely:
- To train the SentencePiece on a larger Hindi corpus
- Creating validation set for cross-validation (did not do it becasue of lack of time)
- Try to fine-tune more about the model (very time consuming)
- Maybe try some traditional ML classifier other than RNN 
- Get Kappa to work
