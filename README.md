 Indian Language Transliteration & Lyrics Generator

This repository contains two simple and powerful deep learning projects:

1. Indian Language Transliteration – Converts native script (e.g., Hindi) into Romanized script.
2. Lyrics Generator – Generates song lyrics based on a given input phrase using LSTM.


1: Indian Language Transliteratio🧠 Overview
This  uses a sequence-to-sequence (Seq2Seq) model with LSTM layers to transliterate Indian language words from native script (like Devanagari) to Roman script (Latin characters).
Dataset
- Source: [Dakshina Dataset by Google](https://github.com/google-research-datasets/dakshin
  Files used:
- `hi.translit.sampled.train.tsv`
- `hi.translit.sampled.dev.tsv`
- `hi.translit.sampled.test.tsv`

Each line contains:  
```text
<native_word> <tab> <romanized_word> <tab> <frequency>
python transliteration_model.py
Input: अंकुर
Predicted: ankur

2: Lyrics Generator
Overview
A simple lyrics generator trained on a corpus of song lyrics using LSTM. Given an initial phrase, the model predicts the next few words to continue the lyrics.

Dataset
Use any .txt file of lyrics. For example:
/content/kenya.txt
How to Run
Make sure the lyrics file is available.

Run the lyrics generation script:
python lyrics_generator.py
Example
Seed Text: "I want"
Output: I want it that way forever now baby yeah

Install the required libraries:

pip install tensorflow keras numpy unidecode

  
