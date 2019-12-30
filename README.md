# NLP for Bengali

This repository contains State of the Art Language models
 and Classifier for Bengali language, which is primarily spoken by the Bengalis
  in South Asia.

The models trained here have been used in [Natural Language Toolkit for Indic Languages
 (iNLTK)](https://github.com/goru001/inltk)

## Dataset

#### Created as part of this project
1. [Bengali Wikipedia Articles](https://www.kaggle.com/disisbig/bengali-wikipedia-articles)

#### Open Source Datasets
2. [Bengali News Articles](https://www.kaggle.com/csoham/classification-bengali-news-articles-indicnlp)

## Results

#### Language Model Perplexity

| Architecture/Dataset | Bengali Wikipedia Articles |
|:--------:|:----:|
|   ULMFiT  |  41.2  |
|  TransformerXL |  39.3  |

#### Classification Metrics

##### ULMFiT

| Dataset | Accuracy | Kappa Score |
|:--------:|:----:|:----:|
| Bengali News Articles |  93.8  |  92  |

#### Visualizations
 
##### Embedding Space

| Architecture | Visualization |
|:--------:|:----:|
| ULMFiT | [Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-bengali/master/language-model/embedding_projector_config.json) |
| TransformerXL | [Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-bengali/master/language-model/embedding_projector_transformer_config.json)  |



## Pretrained Language Model

Download pretrained Language Model from [here](https://drive.google.com/open?id=13zyTFh-0p886o7ycMBxI3Vb0uVos_fbH)


## Classifier

Download classifier from [here](https://drive.google.com/open?id=1DzNZn9jvOeD5HRE-v2NJmxkdnggVZJCs)


## Tokenizer

Trained tokenizer using Google's [sentencepiece](https://github.com/google/sentencepiece)

Download the trained model and vocabulary from [here](https://drive.google.com/open?id=1RlrKSR7MLBaEVrrS_foGja_VCY_enuYB)