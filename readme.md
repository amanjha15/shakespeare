# Shakespeare Translation Model

A Transformer-based machine learning model for translating Shakespearean English into modern English.

## Overview

This project trains a Transformer model to convert Shakespeare's original text into more readable modern English.

### Features

* Custom Transformer architecture
* Byte Pair Encoding (BPE) tokenizer
* Shakespearean → Modern English translation
* Gradient clipping
* Learning-rate scheduler
* Weight decay
* Dropout
* Weight tying between token embeddings and the language-model head

## Project Structure

```text
shakespeare/
├── data/
│   ├── hamlet_original.snt
│   ├── hamlet_modern.snt
│   ├── othello_original.snt
│   ├── othello_modern.snt
│   └── ...
├── Data loading.ipynb
├── shakespeare_bpe.json
├── shakespeare_bpe-vocab.json
├── shakespeare_bpe-merges.txt
└── .gitignore
```

## Model

The model is based on a Transformer architecture and is trained using paired Shakespearean and modern-English sentences.

Model improvements include:

* Learning-rate scheduling
* Gradient clipping
* Adjusted weight decay
* Dropout tuning
* Weight tying
* Multiple training epochs

## Example

**Shakespeare:**

> As if time were in debt.

**Modern English:**

> Time isn't the one in debt.

## Training

The model is trained on aligned Shakespearean and modern-English text.

Model checkpoints (`.pth` / `.pt`) are excluded from Git using `.gitignore`.

## Future Improvements

* Improve translation quality
* Reduce repetitive generation
* Improve padding and masking
* Experiment with larger model architectures
* Evaluate using BLEU and other translation metrics
* Add a simple web interface for translation

## License

This project is for educational and research purposes.
