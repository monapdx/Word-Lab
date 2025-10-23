# 🧪 Streamlit Word Lab

**Streamlit Word Lab** is a text-analysis web app built with [Streamlit](https://streamlit.io/) that helps you explore and visualize language patterns in any text or document.  
Upload TXT, PDF, or HTML files (or paste text) to:

- 🔤 **Extract hyphenated words** — find single or multi-hyphen terms  
- 🧍 **Identify proper nouns or named entities** — using rule-based detection or spaCy NER  
- 📊 **Generate word frequency tables**  
- ☁️ **Create a word cloud** with optional stopword filtering  
- 💾 **Download CSV exports** for each analysis  

---

## 🚀 Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/streamlit-word-lab.git
cd streamlit-word-lab
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the app
```bash
streamlit run streamlit_app2.py
```

Then open the local URL shown in your terminal (usually http://localhost:8501).

---

## 🧩 Features

| Feature | Description |
|----------|--------------|
| **Multi-format upload** | TXT, PDF, HTML, MD, or CSV supported |
| **Text normalization** | Converts smart quotes/dashes and removes formatting |
| **Hyphenated word finder** | Detects words with 1+ or 2+ hyphens |
| **Word frequency explorer** | Displays a ranked list of token frequencies |
| **Named entity extraction** | Uses spaCy if installed, otherwise a rule-based fallback |
| **Word cloud generation** | Adjustable size, transparency, and stopword list |
| **CSV export** | Download results for any analysis |

---

## ⚙️ Dependencies

Core libraries are listed in [`requirements.txt`](./requirements.txt):

```
streamlit
beautifulsoup4
pdfminer.six
PyPDF2
pandas
wordcloud
matplotlib
```
Optional:
- `spacy` + model `en_core_web_sm` (for enhanced entity extraction)

---

## 📘 Tips & Notes

- **PDFs:** Scanned (image-based) PDFs require OCR before use.  
- **Entity extraction:** For best accuracy, install spaCy:
  ```bash
  pip install spacy
  python -m spacy download en_core_web_sm
  ```
- **Word cloud transparency:** Toggle *Transparent background* for easy export.  
- **Performance:** Large files may take longer to process in Streamlit.  

---

## 🧠 About the App

This tool was designed to make lightweight linguistic exploration accessible to anyone — writers, editors, linguists, or developers — without needing complex NLP pipelines.

---

## 🖋 License

MIT License © 2025 Ashly Lorenzana
