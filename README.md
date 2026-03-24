# 🧠 AI Document Diff Tool — Python App (Archived)

> ⚠️ **This repository is archived.**
> Originally built as a standalone **pure Python** document diff engine.  
> It now lives inside my main Django portfolio project:  
> https://github.com/draprar/django_portfolio-walery (see `/document_diff` app)

## 📖 Overview

AI Document Diff Tool started as a standalone Python CLI utility for comparing **DOCX, XLSX, and TXT** files using structural diffing and lightweight semantic analysis.

Later, the full backend logic was integrated as a Django application inside my modular portfolio.  
The Django version retains the same comparison engine while adding UI and API endpoints.

## 🧠 Project Evolution

- Standalone Python tool → *(this repository)*  
- Enhanced with AI heuristics and interactive HTML reports  
- Integrated into a modular Django portfolio → `/document_diff`

## ✨ Features

- Smart structural diff (text, tables, images)  
- AI semantic heuristics using spaCy  
- Interactive HTML reports (filters, collapsible sections, dark/light mode)  
- JSON export for automation  
- Semantic similarity scoring (0–10)  
  
## 🛠️ Technologies

- Python 3.11+  
- spaCy (`pl_core_news_md`)  
- python-docx, openpyxl, pandas  
- difflib  
- Custom HTML/JS reporting engine  

## 🚀 Installation

1. Clone the repository:

   ```
   git clone https://github.com/draprar/python-text-similarity-analysis.git
   cd python-text-similarity-analysis
   ```
   
3. Install dependencies:
   ```
   pip install -r requirements.txt
   python -m spacy download pl_core_news_md
   ```

4. Run the tool:
   
   ```
   python main.py old.docx new.docx
   ```
   
6. The output report will be saved as:
   
   ```
   raport.html
   raport.json
   ```
   
## ▶️ Usage

### Compare two documents
   ```bash
   python main.py file_old.docx file_new.docx
   ```

Then open `raport.html` to explore:

- Highlighted structural and semantic changes
- Collapsible unchanged content
- Filters (added, deleted, changed, unchanged)
- Block types (paragraph, table, image)
- spaCy entity labels (osoba, organizacja, liczba, data)
- Similarity metrics

## 📌 Notes

- No longer actively maintained
- Lives as a Django module in my main portfolio repo
- This repo remains for archival and standalone CLI usage

## 📜 License

This project is licensed under the **MIT License**.

## 👤 Author

**Developer**: Walery ([@draprar](https://github.com/draprar/))  
