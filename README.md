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
2. [Bengali News Articles (Soham Articles)](https://github.com/ai4bharat-indicnlp/indicnlp_corpus#publicly-available-classification-datasets)

## Results

### Language Model Perplexity (on validation set)

| Architecture/Dataset | Bengali Wikipedia Articles |
|:--------:|:----:|
|   ULMFiT  |  41.2  |
|  TransformerXL |  39.3  |

### Classification Metrics

##### ULMFiT

| Dataset | Accuracy | MCC | Notebook to Reproduce results |
|:--------:|:----:|:----:|:----:|
| Bengali News Articles (Soham Articles) |  90.71  |  87.92  | [Link](https://github.com/goru001/nlp-for-bengali/blob/master/classification/Bengali_Classification_Model.ipynb) |


### Visualizations
 
##### Word Embeddings

| Architecture | Visualization |
|:--------:|:----:|
| ULMFiT | [Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-bengali/master/language-model/embedding_projector_config.json) |
| TransformerXL | [Embeddings projection](https://projector.tensorflow.org/?config=https://raw.githubusercontent.com/goru001/nlp-for-bengali/master/language-model/embedding_projector_transformer_config.json)  |

### Results of using Transfer Learning + Data Augmentation from iNLTK

##### On using complete training set (with Transfer learning)

| Dataset | Dataset size (train, valid, test) | Accuracy | MCC | Notebook to Reproduce results |
|:--------:|:----:|:----:|:----:|:----:|
| Bengali News Articles (Soham Articles) | (11284, 1411, 1411) | 90.71 | 87.92 | [Link](https://github.com/goru001/nlp-for-bengali/blob/master/classification/Bengali_Classification_Model.ipynb) |
 

##### On using 1% of training set (with Transfer learning)

| Dataset | Dataset size (train, valid, test) | Accuracy | MCC | Notebook to Reproduce results |
|:--------:|:----:|:----:|:----:|:----:|
| Bengali News Articles (Soham Articles) | (112, 1411, 1411) | 69.88 | 61.56 | [Link](https://github.com/goru001/nlp-for-bengali/blob/master/classification/Bengali_Classification_Model_without_Data_Aug.ipynb) |
 
##### On using 1% of training set (with Transfer learning + Data Augmentation)

| Dataset | Dataset size (train, valid, test) | Accuracy | MCC | Notebook to Reproduce results |
|:--------:|:----:|:----:|:----:|:----:|
| Bengali News Articles (Soham Articles) | (112, 1411, 1411) | 74.06 | 65.08 | [Link](https://github.com/goru001/nlp-for-bengali/blob/master/classification/Bengali_Classification_Model_with_Data_Aug.ipynb) |


## Pretrained Models

#### Language Model

Download pretrained Language Model from [here](https://drive.google.com/open?id=13zyTFh-0p886o7ycMBxI3Vb0uVos_fbH)

#### Tokenizer

Trained tokenizer using Google's [sentencepiece](https://github.com/google/sentencepiece)

Download the trained model and vocabulary from [here](https://drive.google.com/open?id=1RlrKSR7MLBaEVrrS_foGja_VCY_enuYB)