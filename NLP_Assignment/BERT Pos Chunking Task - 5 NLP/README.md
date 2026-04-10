🧠 Token Classification using BERT (POS Tagging & Chunking)

📌 Project Overview

This project demonstrates the implementation of token classification using transformer-based models. The goal is to perform chunking (sequence labeling) on text data using the CoNLL-2003 dataset.

We fine-tune a pretrained DistilBERT model to classify each token in a sentence into its corresponding label.

---

🎯 Objectives

- Implement token classification using transformer models
- Perform chunking using CoNLL-2003 dataset
- Apply tokenization and label alignment
- Train and evaluate DistilBERT model
- Perform inference on custom input sentences

---

📂 Dataset

We use the CoNLL-2003 dataset, a standard benchmark dataset for sequence labeling tasks.

🔗 Dataset Link:
https://www.kaggle.com/datasets/juliangarratt/conll2003-dataset

---

📁 Dataset Files Description

File Name| Description
"eng.train"| Training dataset containing labeled sentences
"eng.testa"| Validation dataset used for evaluation during training
"eng.testb"| Test dataset used for final performance testing

---

📊 Dataset Format

Each line in the dataset contains:

Word  POS  Chunk  NER

Example:

EU      NNP     B-NP    B-ORG
rejects VBZ     B-VP    O
German  JJ      B-NP    B-MISC

- Word → Token
- POS → Part-of-Speech Tag
- Chunk → Phrase tag (used in this project)
- NER → Named Entity tag

---

🧠 Model Used

- Model: DistilBERT ("distilbert-base-uncased")
- Task: Token Classification
- Library: Hugging Face Transformers

---

📊 Evaluation Metrics

We use:

- Accuracy → Measures correct predictions
- F1 Score → Balances precision and recall

Metrics are computed using the "seqeval" library.

---

🚀 Training Details

- Epochs: 2–3
- Batch Size: 8–16
- Optimizer: AdamW
- Learning Rate: 2e-5

Training is optimized to complete within 20–25 minutes.

---

🔮 Inference Example

Input:  John works at Google
Output: [('John', 'B-PER'), ('works', 'O'), ('at', 'O'), ('Google', 'B-ORG')]

---

📈 Observations

- The model effectively learns token-level patterns
- Label alignment is crucial for performance
- Increasing dataset size improves accuracy
- DistilBERT provides good performance with low training time

---

✅ Conclusion

This project successfully demonstrates the use of transformer models for token classification tasks such as chunking.

The model achieves strong performance while maintaining efficient training time, making it suitable for real-world NLP applications.

---

🛠️ Tech Stack

- Python
- Hugging Face Transformers
- PyTorch
- SeqEval
- NumPy / Pandas

---

🙌 Acknowledgements

- CoNLL-2003 Dataset
- Hugging Face Transformers Library

---