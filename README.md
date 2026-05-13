# Intelligent Legal Document Analyzer

An AI-powered system that analyzes legal contracts and identifies risks.

## What It Does
- Extracts text from any legal PDF
- Identifies key entities (people, dates, money, organizations)
- Classifies clauses as High Risk, Caution, or Safe
- Summarizes contracts in plain English
- Answers questions about the document
- Generates a professional PDF analysis report

## Technologies Used
| Tool | Purpose |
|------|---------|
| Google Colab | Development environment |
| pdfplumber | PDF text extraction |
| spaCy | Named Entity Recognition |
| Hugging Face bart-large-mnli | Zero-shot risk classification |
| Sentence Transformers | Text embeddings for Q&A |
| ChromaDB | Vector database for Q&A search |
| Groq API | Free AI for summarization and Q&A |
| fpdf2 | PDF report generation |

## How to Run
1. Open legal_analyzer.ipynb in Google Colab
2. Set runtime to T4 GPU
3. Add your GROQ_API_KEY to Colab Secrets
4. Upload a legal PDF to Google Drive
5. Run all cells in order

## Sample Output
Tested on a Chase Bank Affiliate Agreement:
- 3 High Risk clauses detected
- 1 Caution clause detected
- Key entities, dates and financial terms extracted
- Full plain English summary generated
