# Sentence-Segmentation-in-Roman-Urdu-
Byte Pair  Encoding(BPE) Tokenizer
## Introduction

This project implements subword tokenization using Byte Pair Encoding (BPE) for Roman Urdu, addressing challenges like informal structure and spelling variations.

## Background

### Why Tokenization in Roman Urdu?

Roman Urdu lacks strict spelling rules, leading to multiple variations of the same word, e.g., "Mei" vs. "Mai" vs. "Main" (I).

### What is Byte Pair Encoding (BPE)?

BPE breaks words into frequent subword units, improving tokenization efficiency. Example:

Before BPE: "Karunga" → [Karunga]

After BPE: "Karunga" → [Kar, unga]

## Implementation Steps

This project processes a diary text file and returns tokenized output.

### Preprocessing:

Convert text to lowercase.

Remove punctuation.

Normalize spelling variations.

## BPE Implementation:

Set vocabulary_size = 1000.

Extract unique characters as the initial vocabulary.

Assign IDs to vocabulary items, reserving <UNK> for unknown tokens.

Implement BPE from scratch in Python.

Train on 100 Roman Urdu diary entries.

Test on 14-day diary entries, evaluating <UNK> token occurrences.
