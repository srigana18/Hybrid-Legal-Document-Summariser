# Hybrid-Legal-Document-Summariser
Project Members
Srigana Pulikantham
Eshika Sanjana Konyala
Sowmya Sri Regu
Rohith Nagapuri
**1. Overview**
This project implements a hybrid summarization pipeline for long legal documents using:
1. Extractive summarization — KMeans clustering over Sentence-BERT embeddings
2. Abstractive summarization — nsi319/legal-pegasus
3. Hybrid summarization — Pegasus run on the extractive output
4. Automated evaluation — Gemini-2.5-Flash scoring summaries on:
    factual accuracy
    coverage of important points
    clarity/readability
The entire workflow was developed and tested in Google Colab and packaged so anyone can reproduce the pipeline by downloading or cloning the repository.
