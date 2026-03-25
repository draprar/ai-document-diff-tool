![Python](https://img.shields.io/badge/Python-3.11+-blue)
![spaCy](https://img.shields.io/badge/spaCy-pl_core_news_md-9cf)
![License](https://img.shields.io/badge/License-MIT-yellow)

# 🧠 AI Document Diff Tool — Python App (Archived)
A standalone Python tool for comparing DOCX, XLSX, and TXT files using structural diffing and lightweight semantic analysis.
Smart diffs, AI heuristics, interactive HTML reports, and JSON export — all from the command line.

> ⚠️ This repository is archived.  
> This project has been integrated into my main portfolio:  
> https://github.com/draprar/django_portfolio-walery (see `/document_diff` app)

> 🌐 Live version: https://walery.site/docdiff/

## 📖 Overview

AI Document Diff Tool started as a standalone Python CLI utility for comparing DOCX, XLSX, and TXT files using structural diffing and lightweight semantic analysis.
Later, the full backend logic was integrated as a Django application inside my modular portfolio.
The Django version retains the same comparison engine while adding UI and API endpoints.

## 🧠 Project Evolution

- Standalone Python CLI tool (this repository)
- Enhanced with AI heuristics and interactive HTML reports
- Integrated into the portfolio project as a module
- Archived for historical reference

## ✨ Features

- **Structural Diff**
  - Smart comparison of text, tables, and images across DOCX, XLSX, TXT
- **AI Semantic Heuristics**
  - Semantic similarity scoring (0–10) powered by spaCy
- **Interactive HTML Reports**
  - Filters, collapsible sections, dark/light mode
  - Block types: paragraph, table, image
  - spaCy entity labels: person, organization, number, date
- **JSON Export**
  - Output for automation and further processing

## 🚀 Installation

### Requirements

- Python 3.11+
- spaCy (`pl_core_news_md`)
- python-docx, openpyxl, pandas, difflib

### Step-by-Step Guide

1. **Clone the repository**:
```
   git clone https://github.com/draprar/python-text-similarity-analysis.git
   cd python-text-similarity-analysis
```

2. **Create and activate a virtual environment**:
```
   python -m venv venv
   source venv/bin/activate   # Windows: venv\Scripts\activate
```

3. **Install dependencies**:
```
   pip install -r requirements.txt
   python -m spacy download pl_core_news_md
```

4. **Run the tool**:
```
   python main.py old.docx new.docx
```

5. **Access the output**:
   - HTML report: `raport.html`
   - JSON export: `raport.json`

## 📜 License

This project is licensed under the MIT License.

## 👤 Author

Developed by Walery ([@draprar](https://github.com/draprar/)).
