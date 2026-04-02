# AI Chef — Intelligent Recipe Recommendation Chatbot

A full-stack NLP application combining DistilBERT transformer embeddings and TF-IDF retrieval with live web scraping and a Tkinter desktop GUI — delivering ingredient-aware recipe recommendations through both keyword and semantic search.

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![DistilBERT](https://img.shields.io/badge/DistilBERT-Transformers-f59e0b?style=for-the-badge)](https://huggingface.co/distilbert-base-uncased)
[![NLP](https://img.shields.io/badge/NLP-TF--IDF%20%2B%20Semantic-2563eb?style=for-the-badge)](https://github.com/EoinHoustoun/AI_Chef)
[![Tkinter](https://img.shields.io/badge/GUI-Tkinter-059669?style=for-the-badge)](https://docs.python.org/3/library/tkinter.html)

---

## Overview

- **Problem:** Recipe search engines rely on exact keyword matching, failing to understand user intent — "something spicy with chicken" returns poor results when the user can't name a dish.
- **Approach:** Dual-engine recommendation system: TF-IDF handles fast keyword-based retrieval while DistilBERT transformer embeddings capture semantic meaning. Beautiful Soup scrapes live recipe data. PCA visualises the embedding space. All wrapped in a Tkinter GUI.
- **Result:** A deployable desktop application delivering relevant recipe recommendations through both exact and semantic ingredient/dish queries.

---

## Key Features

- **Dual recommendation engines:** TF-IDF for keyword precision + DistilBERT for semantic understanding
- **Live web scraping:** Beautiful Soup pipeline fetches up-to-date recipe data
- **Full desktop GUI:** Tkinter interface with category selection, free-text input, and random recipe discovery
- **Embedding visualisation:** PCA analysis of DistilBERT embeddings to explore the recipe semantic space
- **Cosine similarity ranking:** Recipes ranked by embedding similarity to user query
- Full-stack project: NLP pipeline + data collection + UI — end to end

---

## Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| NLP Models | DistilBERT (HuggingFace Transformers), TF-IDF |
| Similarity | Cosine Similarity |
| Web Scraping | Beautiful Soup, requests |
| GUI | Tkinter |
| Visualisation | matplotlib, PCA (scikit-learn) |
| Libraries | pandas, NumPy, scikit-learn |

---

## Results

- Dual-engine system outperforms single-model approaches on semantically phrased queries
- PCA of DistilBERT embeddings reveals meaningful clustering of recipes by cuisine and ingredient type
- Live scraping pipeline ensures recipe corpus stays current without manual data collection
- GUI makes the system accessible to non-technical users

---

## How to Run

```bash
pip install -r requirements.txt
python ai_chef.py
```

---

## Project Structure

```
AI_Chef/
├── ai_chef.py              # Main application (GUI + recommendation engine)
├── scraper.py              # Beautiful Soup web scraping pipeline
├── embeddings.ipynb        # DistilBERT embedding analysis and PCA visualisation
├── requirements.txt
└── README.md
```

---

*Part of Eoin Houstoun's Data Science Portfolio — [github.com/EoinHoustoun](https://github.com/EoinHoustoun)*
