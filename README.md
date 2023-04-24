# Language Translation

This is a repository for a language translation project that uses a deep learning approach. Specifically, it implements a Neural Machine Translation (NMT) system that can translate text from one language to another.

## Overview

The repository contains the following files:

- `data/`: a directory that contains the input data for the NMT system. Specifically, it contains two text files: `eng.txt`, which contains English sentences, and `fra.txt`, which contains corresponding French translations of those sentences.
- `models/`: a directory that contains saved models for the NMT system. Specifically, it contains a PyTorch checkpoint file (`nmt_model.pth`) that contains the trained weights for the NMT model.
- `preprocess.py`: a Python script that preprocesses the input data for the NMT system. Specifically, it tokenizes the sentences, converts them to lowercase, and splits them into training and validation sets.
- `train.py`: a Python script that trains the NMT model using the preprocessed data. Specifically, it defines the model architecture, the loss function, and the optimizer, and then trains the model using mini-batch stochastic gradient descent.
- `translate.py`: a Python script that uses the trained NMT model to translate new sentences from one language to another.

## Dependencies

The project requires Python 3 and the following Python libraries:

- PyTorch
- NumPy
- scikit-learn

These libraries can be installed using pip or conda.

## Usage

To use the NMT system, follow these steps:

1. Download or clone the repository onto your local machine.
2. Download the input data for the NMT system and place the `eng.txt` and `fra.txt` files in the `data/` directory.
3. Open a terminal or command prompt and navigate to the directory containing the repository.
4. Run the `preprocess.py` script to preprocess the input data:
```
python preprocess.py
```
5. Run the `train.py` script to train the NMT model:
```
python train.py
```
6. (Optional) Evaluate the NMT model on the validation set:
```
python evaluate.py
```
7. Run the `translate.py` script to translate new sentences:
```
python translate.py --input <input_file> --output <output_file> --src <source_language> --tgt <target_language>
```
where `<input_file>` is the path to a text file containing sentences to be translated, `<output_file>` is the path to a text file where the translated sentences will be saved, `<source_language>` is the language of the input sentences (either `eng` for English or `fra` for French), and `<target_language>` is the language to which the sentences will be translated (either `eng` or `fra`).

## Acknowledgements

This project was inspired by the PyTorch tutorial on Neural Machine Translation with Attention, available at https://pytorch.org/tutorials/intermediate/seq2seq_translation_tutorial.html. The input data for the NMT system was obtained from the Tatoeba Project, available at https://tatoeba.org/eng/downloads.
