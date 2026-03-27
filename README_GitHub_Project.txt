# GPT-Style Fantasy Language Model Final Project

This repository contains a graduate final project notebook that builds and trains a custom GPT-style language model on a cleaned corpus of book text.

It has A LOT OF ROOM FOR IMPROVEMENT, but this is what I have so far.

## Project overview
The notebook walks through the full pipeline:
- collecting or loading plain-text books
- cleaning and standardizing text files
- training a BPE tokenizer
- converting text into token tensors
- building autoregressive training sequences
- training a decoder-only transformer in PyTorch
- evaluating with validation loss and perplexity
- generating fantasy-style text from prompts

## Main file
- `Math_579_Final_Project_GitHub_Ready.ipynb` — fully annotated notebook prepared for GitHub

## Expected directory structure
The notebook uses relative paths rooted at `Books_Dataset/`:

```text
Books_Dataset/
├── Original_Text_Downloads/
├── Formatted_Original_Text_Files/
├── Cleaned_Text/
├── Saved_Model_and_Checkpoints/
├── tokenizer.json
├── combined_corpus.txt
├── full_corpus_tokens.pt
├── per_file_token_tensors.pt
└── training_log.csv
```

## Environment
Recommended Python libraries include:
- torch
- transformers
- tokenizers
- pandas
- numpy
- requests
- beautifulsoup4
- matplotlib

## Notes
- The notebook is GPU-aware and will use CUDA when available.
- Cleaning process was specificly made for the books downloaded from Guttenberg. You might need to edit it for the purposes of  your own data set.
- Outputs were cleared before publishing so the notebook is easier to review on GitHub.
- Paths are relative, which makes the project easier to move between machines.
- Checkpoint files are not included in the notebook itself.