# 🧠 Transformer Components from Scratch using NumPy

A complete implementation of two fundamental components used in modern Transformer-based Large Language Models (LLMs):

* 🔤 **Custom Byte-Pair Encoding (BPE) Tokenizer**
* 🤖 **Autoregressive Language Model**

Both projects are implemented **from scratch using Python and NumPy**, without relying on tokenizer libraries or deep learning frameworks such as TensorFlow or PyTorch. This repository demonstrates the core concepts behind subword tokenization and next-token prediction used in models like GPT, BERT, RoBERTa, and T5.

---

# 📌 Project Overview

Modern Large Language Models consist of two major stages:

1. **Tokenization** – Converting text into meaningful subword tokens.
2. **Language Modeling** – Predicting the next token based on previously generated tokens.

This repository implements both stages from scratch:

### 🔤 Custom Byte-Pair Encoding (BPE)

The BPE tokenizer learns a subword vocabulary by repeatedly merging the most frequent adjacent symbol pairs. It reduces vocabulary size while efficiently handling rare and unseen words.

### 🤖 Autoregressive Language Model

The autoregressive language model predicts the next token in a sequence using embeddings, positional encoding, causal masking, self-attention, linear transformation, softmax, cross-entropy loss, and iterative text generation.

Together, these projects provide a practical understanding of the preprocessing and language modeling pipeline used in Transformer architectures.

---

# 🎯 Objectives

* Implement the Byte-Pair Encoding (BPE) algorithm from scratch.
* Learn subword vocabulary from a text corpus.
* Generate merge rules through iterative pair merging.
* Encode and decode words using learned subwords.
* Build a simplified autoregressive language model.
* Convert tokens into numerical IDs.
* Create embeddings and positional encodings.
* Implement causal masking and self-attention.
* Compute softmax probabilities and cross-entropy loss.
* Perform backpropagation.
* Generate text one token at a time.

---

# ✨ Features

## 🔤 Custom BPE Tokenizer

* 📄 Read corpus from a text file
* 🧹 Text preprocessing
* 🔤 Character-level tokenization
* 📊 Word frequency calculation
* 🔗 Adjacent symbol pair frequency analysis
* 🔄 Iterative pair merging
* 📚 Vocabulary construction
* 🔐 Word encoding
* 🔓 Word decoding

## 🤖 Autoregressive Language Model

* 🔤 Character-level tokenization
* 🔢 Token-to-ID conversion
* 🧩 Input-target pair generation
* 🎯 Embedding creation
* 📍 Positional Encoding
* 🚫 Causal Mask
* 🔍 Self-Attention
* 📈 Linear Layer
* 🎲 Softmax
* 📉 Cross-Entropy Loss
* 🔄 Backpropagation
* 🤖 Next-token generation

---

# 🛠️ Technologies Used

* Python 3
* NumPy
* Jupyter Notebook

---

# 📂 Project Structure

```text
Transformer-From-Scratch/
│
├── corpus.txt
├── Byte pair encoding.ipynb
├── Autoregressive_Model.ipynb
├── BPE_From_Scratch_Implementation_Steps.docx
├── Autoregressive_Implementation_Steps.docx
├── README.md
```

---

# ⚙️ Overall Workflow

```text
                    Text Corpus
                         │
                         ▼
                 Read Text Corpus
                         │
                         ▼
                Preprocess Text
                         │
                         ▼
          Character-Level Tokenization
                         │
                         ▼
           Byte-Pair Encoding (BPE)
                         │
                         ▼
             Learn Merge Rules
                         │
                         ▼
             Build Vocabulary
                         │
                         ▼
            Encode Text into IDs
                         │
                         ▼
         Create Input-Target Pairs
                         │
                         ▼
             Create Embeddings
                         │
                         ▼
          Add Positional Encoding
                         │
                         ▼
            Apply Causal Mask
                         │
                         ▼
         Compute Self-Attention
                         │
                         ▼
              Linear Layer
                         │
                         ▼
                 Softmax
                         │
                         ▼
          Cross-Entropy Loss
                         │
                         ▼
            Backpropagation
                         │
                         ▼
          Update Parameters
                         │
                         ▼
       Generate Next Token Iteratively
```

---

# 📖 Implementation Steps

## Part 1 – Byte-Pair Encoding (BPE)

1. Read the input text corpus.
2. Preprocess the text.
3. Split each word into characters.
4. Append the end-of-word symbol (`</w>`).
5. Count word frequencies.
6. Find adjacent symbol pairs.
7. Calculate pair frequencies.
8. Select the most frequent pair.
9. Merge the pair.
10. Update the vocabulary.
11. Repeat merging.
12. Store merge rules.
13. Build the final vocabulary.
14. Encode new words.
15. Decode subword tokens.

---

## Part 2 – Autoregressive Language Model

1. Read the corpus.
2. Tokenize the text.
3. Convert tokens into IDs.
4. Create input-target pairs.
5. Initialize embeddings.
6. Add positional encoding.
7. Apply causal masking.
8. Compute scaled dot-product self-attention.
9. Apply linear transformation.
10. Compute softmax probabilities.
11. Calculate cross-entropy loss.
12. Perform backpropagation.
13. Update model parameters.
14. Generate the next token iteratively.

---

# ▶️ How to Run

Clone the repository.

```bash
git clone https://github.com/nikithanka7-byte/Transformer-From-Scratch.git
```

Navigate to the project folder.

```bash
cd Transformer-From-Scratch
```

Open Jupyter Notebook.

```bash
jupyter notebook
```

Run:

* **Byte pair encoding.ipynb**
* **Autoregressive_Model.ipynb**

---

# 📊 Sample Output

The implementation displays:

## BPE Tokenizer

* Initial Vocabulary
* Word Frequencies
* Pair Frequencies
* Merge Operations
* Learned Merge Rules
* Final Vocabulary
* Encoded Words
* Decoded Words

## Autoregressive Language Model

* Token IDs
* Input-Target Pairs
* Embedding Matrix
* Positional Encoding
* Self-Attention Scores
* Attention Weights
* Context Vectors
* Softmax Probabilities
* Cross-Entropy Loss
* Updated Parameters
* Generated Tokens

---

# 📚 Key Concepts Covered

* Byte-Pair Encoding (BPE)
* Subword Tokenization
* Vocabulary Learning
* Merge Rules
* Character-Level Tokenization
* Embeddings
* Positional Encoding
* Self-Attention
* Causal Masking
* Linear Transformation
* Softmax
* Cross-Entropy Loss
* Backpropagation
* Autoregressive Language Modeling
* Transformer Fundamentals
* NumPy Programming
* Natural Language Processing (NLP)

---

# 🎓 Learning Outcomes

Through this project, I learned:

* The fundamentals of Byte-Pair Encoding.
* How subword vocabularies are generated.
* Frequency-based pair merging.
* Building merge rules from a text corpus.
* Encoding and decoding text using subword tokens.
* Tokenization techniques used in modern LLMs.
* The working of embeddings and positional encoding.
* The self-attention mechanism in Transformers.
* The role of causal masking in autoregressive models.
* Cross-entropy loss and parameter optimization.
* Next-token prediction.
* End-to-end implementation of key Transformer components using only NumPy.

---

# 📝 Conclusion

This repository demonstrates the implementation of two essential components of Transformer-based language models: a **Custom Byte-Pair Encoding (BPE) Tokenizer** and a **Custom Autoregressive Language Model**, both developed entirely from scratch using Python and NumPy. It covers the complete workflow from text preprocessing and subword vocabulary learning to token embeddings, self-attention, loss computation, and iterative text generation. This project provides a strong practical foundation for understanding the internal workings of modern Large Language Models (LLMs).

---

# 👩‍💻 Author

**Nikitha R**

