# Language Translation

This is a repository for a language translation project that uses a deep learning approach. Specifically, it implements a Neural Machine Translation (NMT) system that can translate text from one language to another.

## Overview

The notebook is organized into several sections, each representing a different step in the implementation of the language translation model. Here is a brief summary of each section:

### 1. **Importing necessary libraries:** 
This section imports the required libraries for the implementation of the language translation model, such as NumPy, Pandas, TensorFlow, and Keras.

### 2. **Loading the data:** 
This section loads the language translation dataset, which consists of pairs of sentences in English and Spanish. The dataset is split into training and validation sets.

### 3. **Preprocessing the data:** 
This section preprocesses the text data by removing unnecessary characters, converting the text to lowercase, and tokenizing the text into individual words.

### 4. **Building the language translation model:** 
This section defines the seq2seq neural network architecture for the language translation model using the TensorFlow and Keras libraries.

### 5. **Training the language translation model:** 
This section trains the language translation model on the preprocessed data using the defined neural network architecture.

### 6. **Evaluating the language translation model:** 
This section evaluates the performance of the trained language translation model on the validation set using the BLEU score metric.

### 7. **Generating translations:** 
This section defines a function to generate translations of new sentences using the trained language translation model.
