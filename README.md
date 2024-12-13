# COVID-19 Text Analysis and Language Modeling Assignments

This repository contains solutions for multiple assignments focused on natural language processing (NLP) tasks using a COVID-19-related dataset. The tasks include pre-processing, clustering, word embeddings, and abstract generation.

---

## Table of Contents

1. [Assignment 1: Text Preprocessing and Zipf's Law](#assignment-1-text-preprocessing-and-zipfs-law)
2. [Assignment 2 & 3: Modified COALS Algorithm](#assignment-2--3-modified-coals-algorithm)
3. [Assignment 4 & 5: Skipgram Model](#assignment-4--5-skipgram-model)
4. [Assignment 6, 7 & 8: Abstract Generation](#assignment-6-7--8-abstract-generation)
5. [Usage Instructions](#usage-instructions)

---

## Assignment 1: Text Preprocessing and Zipf's Law

#### Tasks:

1. **Extract Text Content**:
   - Extract text from the JSON dataset using a Python library (e.g., `json` or `pandas`).

2. **Preprocessing**:
   - Perform case-folding, removal of numbers, stopword elimination, tokenization, and stemming/lemmatization.

3. **Weighted Term Frequency and Zipf’s Law**:
   - Compute term frequencies.
   - Plot frequency vs. rank to validate Zipf's Law.
   - Calculate the exponent \(\alpha\).

4. **Tokens and Vocabulary**:
   - Count the total tokens and unique vocabulary.

5. **Tokens vs. Vocabulary**:
   - Use Heap’s Law to plot vocabulary size as a function of tokens.

---

## Assignment 2 & 3: Modified COALS Algorithm

#### Tasks:

1. **Co-occurrence Matrix**:
   - Build a co-occurrence matrix using the ratio of probabilities instead of correlation.
   - Limit the vocabulary size to ~7K words.

2. **Vocabulary Size**:
   - Display the vocabulary size and matrix dimensions.

3. **Identify Words**:
   - Select five COVID-19-related nouns and verbs.

4. **Word Similarities**:
   - Compute and display five similar words for each selected word using cosine distance.

5. **Visualization**:
   - Use Multi-Dimensional Scaling (MDS) to visualize concepts. Plot three concepts with up to 10 words per concept.

---

## Assignment 4 & 5: Skipgram Model

#### Tasks:

1. **Corpus and Vocabulary**:
   - Extract abstracts and create a vocabulary of ~10,000 words.

2. **One-Hot Vectors**:
   - Implement dynamic or pre-created OHVs for training.

3. **Model Architecture**:
   - Describe the neural network architecture for the Skipgram model.

4. **Training**:
   - Use Stochastic Gradient Descent (SGD) for optimization.

5. **Epoch vs. Training Error**:
   - Plot the relationship between epochs and training error.

6. **Negative Sampling**:
   - Replace naive softmax with negative sampling (5 negative samples per instance).

7. **Word Analogies**:
   - Test analogies with two COVID-19-related words (avoiding commonly restricted terms).

8. **Matrix Comparisons**:
   - Analyze similarities using Win, Wout, and their combinations.

---

## Assignment 6, 7 & 8: Abstract Generation

#### Tasks:

1. **Architecture**:
   - Implement a two-layer vanilla RNN, LSTM, or GRU model.
   - Support both forward and backward passes.

2. **Training**:
   - Train the model using 100 abstracts initially.
   - Plot the error graph during training.

3. **Abstract Generation**:
   - Use the trained model to generate at least three abstracts.

4. **Discussion**:
   - Identify factors contributing to sub-optimal results.
   - Suggest improvements for better performance.

---

## Usage Instructions

#### File Structure:

```plaintext
├── data/
│   ├── covid19_dataset.json
├── src/
│   ├── assignment1_text_preprocessing.py
│   ├── assignment2_3_coals.py
│   ├── assignment4_5_skipgram.py
│   ├── assignment6_7_8_abstract_generation.py
├── results/
│   ├── tokens_vs_vocab_plot.png
│   ├── epochs_vs_error.png
│   ├── coals_visualization.png
├── README.md
