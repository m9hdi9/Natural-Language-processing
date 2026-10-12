# Lab 7 — Large Language Models (LLMs)

This laboratory explores the three primary Transformer architectural families using the Hugging Face `transformers` ecosystem and PyTorch: **Decoder-only**, **Encoder–decoder**, and **Encoder-only** architectures[cite: 6].

---

## Transformer Model Families Overview

| Family | Mechanism | Primary Use Cases | Evaluated Model |
| :--- | :--- | :--- | :--- |
| **Encoder-only** | Bidirectional self-attention; contextualizes full input representations[cite: 6]. | Text classification, Sentiment Analysis, NER[cite: 6]. | `DistilBERT`[cite: 6] |
| **Encoder–decoder** | Sequence-to-sequence; processes input sequence and decodes an output sequence[cite: 6]. | Translation, Abstractive Summarization, Question Answering[cite: 6]. | `FLAN-T5-small`[cite: 6] |
| **Decoder-only** | Causal autoregression; predicts subsequent tokens sequentially[cite: 6]. | Open-ended text generation, conversational dialogue[cite: 6]. | `DistilGPT-2`[cite: 6] |

---

## Lab Implementation & Tasks

- **Task 1 (Model Selection)**: Mapping distinct NLP tasks (e.g., sentiment analysis, machine translation, text generation) to their optimal transformer architectural paradigm[cite: 6].
- **Task 2 (Sentiment Analysis — Encoder-only)**: Evaluating `DistilBERT` on multiple test utterances to extract binary sentiment classifications and confidence scores[cite: 6].
- **Task 3 (Text Summarization — Encoder–Decoder)**: Generating abstractive summaries of unstructured paragraphs using instruction-tuned `FLAN-T5-small`[cite: 6].
- **Task 5 (Theoretical Reflection)**: Analyzing the operational fit of decoder-only causal language modeling for multi-turn conversational agents (e.g., ChatGPT)[cite: 6].
- **Optional Challenge (Sampling vs. Deterministic Decoding)**: Demonstrating non-deterministic output generation through probabilistic sampling (`do_sample=True`) versus greedy search by omitting static seeds[cite: 6].

---

## Environment & Setup

Install the required dependencies:

```bash
pip install transformers sentencepiece torch
