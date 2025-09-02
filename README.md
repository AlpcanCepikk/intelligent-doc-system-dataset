# Intelligent Document System Dataset

A small multi-format dataset prepared for **Intelligent Document System** experiments and **synthetic data generation**.  
This dataset is designed for testing **RAG pipelines, embeddings, and multi-format document loaders**.

## Contents
- 33 × PDF (academic papers from arXiv)
- 2 × DOCX (engineering reports/templates)
- 1 × TXT (SMS Spam Collection dataset)

## Structure

my_dataset/

├── pdfs/ # arXiv PDFs

├── docx/ # engineering reports

├── txt/ # SMS Spam Collection

You can review or download the dataset from the link below.
https://huggingface.co/datasets/CepikAlpcan/Intelligent-Document-System-Dataset/tree/main

from datasets import load_dataset

dataset = load_dataset("CepikAlpcan/Intelligent-Document-System-Dataset", streaming=True)
first_sample = next(iter(dataset))
print(first_sample)
