# PDF Data Extraction Notebook

This notebook demonstrates three methods to extract text from PDFs, especially those with Khmer and English content.

## Methods

1. **Google Cloud Vision**: API-based text detection, processes PDFs in chunks.
2. **Gemini API**: AI-powered extraction using Google's Gemini model.
3. **Tesseract OCR**: Open-source OCR with multi-language support.

## Requirements

- Python packages: `google-cloud-vision`, `PyPDF2`, `google-generativeai`, `pytesseract`, `pdf2image`, `pillow`
- API keys for Google services
- Tesseract OCR installed with Khmer data

## Installation

```bash
pip install google-cloud-vision PyPDF2 google-generativeai pytesseract pdf2image pillow
```

For Tesseract:
```bash
apt-get install tesseract-ocr libtesseract-dev poppler-utils
wget -O tessdata/khm.traineddata https://github.com/tesseract-ocr/tessdata/raw/main/khm.traineddata
```

## Usage

Run the notebook cells for each method. Set your API keys and PDF paths as needed.

## Google Colab

Try it interactively: [Extract Data Notebook](https://colab.research.google.com/drive/1S05o6CGhWDI7ZtZqUeozd-RZzQgTgfJh?usp=sharing)

## Notes

- Google APIs require internet and keys
- Tesseract works offline
- For large PDFs, processing may take time
