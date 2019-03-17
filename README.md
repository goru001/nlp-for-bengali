# NLP for Bengali

This repository contains State of the Art Tokenizer, Language model
 and Classifier for Bengali, which is primarily spoken by the Bengalis in South Asia.

## Dataset

* Download [Bengali Wikipedia Articles Dataset](https://drive.google.com/open?id=1GC76qIGbly4sKX9XsUP_OtsI80nJ6lQ4) (72,374 articles) which I scraped, cleaned and
used to train the language model

Thanks to [Soham](https://github.com/soham96) for making available [these](https://www.kaggle.com/csoham/classification-bengali-news-articles-indicnlp)
Bengali News Articles for classification which I used to train the classifier.

## Results

#### Language Model

`on 30% validation set`

* Perplexity of language model: ~41

#### Classifier

* Accuracy of classification model: ~94%
* Kappa score of classification model: ~92

## Pretrained Language Model

Download pretrained Language Model from [here](https://drive.google.com/open?id=13zyTFh-0p886o7ycMBxI3Vb0uVos_fbH)


## Classifier

Download classifier from [here](https://drive.google.com/open?id=1DzNZn9jvOeD5HRE-v2NJmxkdnggVZJCs)


## Tokenizer

Trained tokenizer using Google's [sentencepiece](https://github.com/google/sentencepiece)

Download the trained model and vocabulary from [here](https://drive.google.com/open?id=1RlrKSR7MLBaEVrrS_foGja_VCY_enuYB)