# 🧩 Custom Byte-Pair Encoding (BPE) Tokenizer from Scratch

A Python implementation of the **Byte-Pair Encoding (BPE)** tokenizer from scratch without using any tokenizer libraries or pretrained models. This project demonstrates how BPE learns subword vocabularies through iterative pair merging and applies the learned merge rules to encode and decode words.

---

# 📌 Project Overview

Byte-Pair Encoding (BPE) is a popular subword tokenization algorithm used in modern Natural Language Processing (NLP) models such as GPT, BERT, RoBERTa, and T5. Instead of treating every word as a unique token, BPE builds a vocabulary by repeatedly merging the most frequent adjacent symbol pairs. This enables efficient handling of rare and unseen words while reducing the overall vocabulary size.

This project provides a complete implementation of the BPE tokenizer from scratch using Python.

---

# 🎯 Objectives

* Implement the Byte-Pair Encoding (BPE) algorithm from scratch.
* Learn subword vocabulary from a text corpus.
* Calculate adjacent symbol pair frequencies.
* Generate merge rules through iterative merging.
* Build the final vocabulary.
* Encode new words into subword tokens.
* Decode subword tokens back into the original words.

---

# ✨ Features

* 📄 Read text corpus from a file
* 🧹 Text preprocessing
* 🔤 Character-level tokenization
* 📊 Word frequency counting
* 🔗 Adjacent symbol pair frequency calculation
* 🔄 Iterative pair merging
* 📚 Merge rule generation
* 🗂️ Final vocabulary creation
* 🔐 Encode words into subword tokens
* 🔓 Decode tokens back into original words

---

# 🛠️ Technologies Used

* Python 3
* NumPy
* Jupyter Notebook

---

# 📂 Project Structure

```text
BPE-Tokenizer/
│── corpus.txt
│── Byte pair encoding.ipynb
│── BPE_From_Scratch_Implementation_Steps.docx
│── README.md
```

---

# ⚙️ Algorithm Workflow

```text
Text Corpus
      │
      ▼
Read Corpus
      │
      ▼
Preprocess Text
      │
      ▼
Split Words into Characters
      │
      ▼
Append </w>
      │
      ▼
Count Word Frequencies
      │
      ▼
Find Adjacent Symbol Pairs
      │
      ▼
Count Pair Frequencies
      │
      ▼
Select Most Frequent Pair
      │
      ▼
Merge Pair
      │
      ▼
Update Vocabulary
      │
      ▼
Repeat Until Desired Merges
      │
      ▼
Store Merge Rules
      │
      ▼
Build Final Vocabulary
      │
      ▼
Encode New Words
      │
      ▼
Decode Tokens
```

---

# 📖 Implementation Steps

1. Read the input text corpus.
2. Preprocess the text.
3. Split each word into individual characters.
4. Append the end-of-word symbol (`</w>`).
5. Count the frequency of each word.
6. Identify adjacent symbol pairs.
7. Calculate pair frequencies.
8. Select the most frequent pair.
9. Merge the selected pair.
10. Update the vocabulary.
11. Repeat the merging process until the desired number of merges is reached.
12. Store the learned merge rules.
13. Build the final vocabulary.
14. Encode new words using the learned rules.
15. Decode subword tokens back into words.

---

# ▶️ How to Run

1. Clone the repository.

```bash
git clone https://github.com/nikithanka7-byte/BPE-Tokenizer.git
```

2. Navigate to the project folder.

```bash
cd BPE-Tokenizer
```

3. Open the notebook.

```bash
jupyter notebook
```

4. Run all cells in **Byte pair encoding.ipynb**.

---

# 📊 Sample Output

The implementation displays:

* Initial Vocabulary
* Word Frequencies
* Pair Frequencies
* Most Frequent Pair
* Merge Operations
* Updated Vocabulary
* Final Vocabulary
* Learned Merge Rules
* Encoded Words
* Decoded Words
* Vocabulary Size

---

# 📚 Key Concepts Covered

* Byte-Pair Encoding (BPE)
* Subword Tokenization
* Vocabulary Learning
* Pair Frequency Analysis
* Merge Rules
* Encoding and Decoding
* Natural Language Processing (NLP)
* Python Programming

---

# 🎓 Learning Outcomes

Through this project, I learned:

* The fundamentals of Byte-Pair Encoding.
* How subword vocabularies are generated.
* Frequency-based pair merging techniques.
* Building merge rules from a text corpus.
* Encoding and decoding using learned subword tokens.
* The importance of BPE in Transformer-based language models.
* Practical implementation of an NLP algorithm from scratch.

---

# 📝 Conclusion

This project demonstrates the complete implementation of a **Custom Byte-Pair Encoding (BPE) Tokenizer** from scratch using **Python**. It covers the entire workflow, including corpus preprocessing, vocabulary learning, iterative pair merging, merge rule generation, and encoding/decoding of words. The project provides a strong foundation for understanding subword tokenization techniques used in modern Transformer-based NLP models.

---

# 👩‍💻 Author

**Nikitha R**

