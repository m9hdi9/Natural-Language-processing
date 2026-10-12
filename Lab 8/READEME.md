# Lab 8 — Part-of-Speech (POS) Tagging

This lab covers Part-of-Speech (POS) tagging techniques using both **NLTK** and **spaCy** in Python to analyze and extract grammatical structures from text[cite: 7].

---

## Overview & Concepts

- **Coarse-grained Tags (`pos_`)**: General grammatical categories (e.g., `NOUN`, `VERB`, `ADJ`)[cite: 7].
- **Fine-grained Tags (`tag_`)**: Specific grammatical forms based on morphology and tense (e.g., `NN`, `VBZ`, `VBD`)[cite: 7].
- **Dependency Parsing (`displaCy`)**: Visualizing grammatical relationships and syntactic trees between tokens[cite: 7].

---

## Tasks Implemented

- **Task 1 (Token-level POS Analysis)**: Extracted coarse-grained, fine-grained, and tag definitions for specific tokens (e.g., *"play"*), followed by full-sentence morphological breakdown[cite: 7].
- **Task 2 (Contextual Disambiguation)**: Compared ambiguous words (*"Google"*, *"table"*) across distinct sentences to show how grammatical function shifts between nouns and verbs depending on context[cite: 7].
- **Task 3 (Syntactic Visualization)**: Rendered interactive dependency parse trees and POS tags using `displaCy.render`[cite: 7].

---

## Requirements & Setup

```bash
pip install nltk spacy
python -m spacy download en_core_web_sm
