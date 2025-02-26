# SQuAD Project - Question Answering with Transformers

## Overview
This project utilizes the **Stanford Question Answering Dataset (SQuAD)** to train a **DistilBERT-based** model for question-answering tasks. The project preprocesses the dataset, tokenizes input data, and prepares it for fine-tuning using **Hugging Face's Transformers** library.

## Features
- Loads and processes the SQuAD dataset using **datasets.load_dataset**.
- Utilizes **DistilBERT** tokenizer for encoding questions and context.
- Implements sliding window tokenization to handle long contexts.
- Extracts start and end positions for answer span detection.
- Prepares the dataset for model fine-tuning.

## Requirements
Install the necessary dependencies using:
```bash
pip install transformers datasets
```

## Dataset
- The dataset used is **SQuAD (Stanford Question Answering Dataset)**.
- It consists of paragraphs of text with corresponding **questions and answers**.
- Answers are extracted from specific spans within the provided context.

## Tokenization and Preprocessing
- Tokenization is performed using **DistilBERT tokenizer**.
- Handles long contexts using **truncation and sliding window approaches**.
- Maps original character positions of answers to token positions.

## How to Run
1. Install required dependencies.
2. Load the SQuAD dataset using `datasets.load_dataset("squad")`.
3. Tokenize and preprocess the dataset using **DistilBERT tokenizer**.
4. Prepare tokenized datasets with start and end token positions.
5. Fine-tune a **transformer model** for question answering (not included in this script but can be done using Hugging Face's Trainer API).

## Output
- Tokenized dataset ready for fine-tuning.
- Mapped answer positions in tokenized input.
- Processed dataset with overflow tokens and offsets for better context handling.

## License
This project is intended for educational and research purposes only. The dataset is publicly available under the SQuAD dataset license.

