# Deep Learning for NLP — Sentiment Analysis

This project classifies Yelp restaurant reviews into **Positive (1)** or **Negative (0)** using PyTorch and NLP feature representation techniques.

---

### Features & Workflow

1. **Text Preprocessing**: Lowercasing, removing special characters/punctuation, and whitespace normalization using Regex.
2. **Feature Extraction**:
   - **TF-IDF**: Standard baseline converting text into numerical feature vectors.
   - **Word2Vec (Skip-gram)**: Custom-trained embeddings (`vector_size=200`, `window=5`, `sg=1`) averaged to represent full reviews.
3. **Neural Network Models (PyTorch)**:
   - **TF-IDF Model**: Fully connected network with 2 hidden layers (64, 32 neurons) trained using Adam and `BCEWithLogitsLoss`.
   - **Word2Vec Model**: Deep architecture with 3 hidden layers (128, 64, 32 neurons) trained over 15 epochs.
4. **Evaluation**: Assessed using Accuracy, Precision, Recall, F1-Score, and Confusion Matrix.

---

### Requirements

- Python 3.x
- PyTorch
- Gensim
- Scikit-learn
- Pandas, NumPy

```bash
pip install torch gensim scikit-learn pandas numpy
