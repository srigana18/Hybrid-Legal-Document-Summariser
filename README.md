# Hybrid Legal Document Summariser
---

## Project Members
- **Srigana Pulikantham**  
- **Eshika Sanjana Konyala**  
- **Sowmya Sri Regu**  
- **Rohith Nagapuri**

---

## Overview

This project implements a **hybrid legal document summarization pipeline** using:

### Extractive Summarization  
KMeans clustering on Sentence-BERT embeddings  

### Abstractive Summarization  
`nsi319/legal-pegasus`  

### Hybrid Summarization  
Pegasus applied on extractive output  

### Automated Evaluation  
**Gemini-2.5-Flash** scoring summaries on:
- factual accuracy  
- coverage  
- clarity/readability  

Entire workflow developed and tested in **Google Colab**.

---

## How to Run This Project in Google Colab (Preferred)

You can load the project using **any one** of the following:

### Option 1 — Clone the GitHub Repository
`!git clone https://github.com/srigana18/Hybrid-Legal-Document-Summariser.git`
`%cd Hybrid-Legal-Document-Summariser`

### Option 2 — Open Using the Provided Google Drive Link
https://colab.research.google.com/drive/1JHgyCaA6LPykoeskpedx08boJ6DQTisV?usp=sharing

### Required API Keys
Paste this into a Colab cell before running the notebook:

`"GEMINI_API_KEY" = "AIzaSyAN_QefiVDyOwuDO_YIFiVIDmk4y74NTR4""
"HF_TOKEN" = "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"`

### Folder Structure
inputs/          → sample input texts
outputs/         → generated summaries + evaluations
legalsumm.ipynb  → main summarizer notebook
requirements.txt → dependencies

### Running Locally (Optional)
Colab is recommended.
Local setup (optional):
`pip install -r requirements.txt`
Open legalsumm.ipynb in Jupyter or VS Code.
