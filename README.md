# Scoreme_hack
 
This project extracts **tables** from PDF documents and converts them into structured **JSON** and **Excel** formats using **LLMs (Llama 3.3-70B)**. The script ensures that only valid table structures are extracted, preserving headers and data accurately.

---

## 🚀 Features  
- Extracts tables from **financial PDFs**.   
- Outputs **JSON format** with clearly separated headers and rows.  
- Converts extracted tables into **Excel spreadsheets** for easy analysis.

---
📌 Approach
Extracting Text: The script uses PyPDF2 to extract text from the PDF file, ensuring all content is retrieved accurately.
Processing with LLM: The extracted text is sent to a Large Language Model (LLM) via the Groq API, providing context for structured extraction.
Structured JSON Output: The LLM processes the text and extracts only table data, returning a well-structured JSON format with clearly defined headers and rows.
Excel Conversion: The JSON output is efficiently converted into an Excel file using pandas and openpyxl, preserving tabular data for easy analysis.


---

## 📌 Installation  

Ensure you have **Python 3.8+** installed. Then, install the required dependencies:  

```bash
pip install PyPDF2 pandas openpyxl langchain_groq langchain_core
