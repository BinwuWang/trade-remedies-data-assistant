# Trade Remedies Data Assistant

The Trade Remedies Data Assistant is an AI-powered system designed to automate the extraction, analysis, and structured management of trade remedy regulatory data.

Trade remedy documents (e.g., WTO reports and national regulations) are often long, complex, and inconsistent in format. Manual processing is time-consuming, error-prone, and difficult to scale.

This system provides an end-to-end pipeline to:
- Collect and manage regulatory documents
- Automatically extract structured product and measure data
- Validate extraction results with AI-assisted review
- Export clean, standardized data into databases

## Key Features

- Dual Pipeline Architecture
  - WTO standardized document processing
  - National regulation parsing with country-specific rules

- Hybrid Extraction Engine
  - Rule-based parsing (regex, structural anchors)
  - LLM-assisted validation and correction

- Structured Data Output
  - Extracts product, HS codes, duties, companies, and measures
  - Supports database-ready schema

- Traceable Results
  - Highlights extracted content in source PDFs
  - Reduces hallucination and improves verification

- Scalable Design
  - Modular parser design for multi-country extension
 
## Tech Stack

- Python
- Flask
- PyMuPDF / pdfplumber
- OpenRouter (LLM integration)
- SQLAlchemy
- HTML / JS (frontend)

## System Architecture

1. Document Ingestion
2. Pipeline Selection (WTO / National)
3. Parsing & Extraction
4. AI Review (LLM)
5. Result Validation & Highlighting
6. Database Export

## Installation

```bash
git clone https://github.com/YOUR_USERNAME/trade-remedies-data-assistant.git
cd trade-remedies-data-assistant

pip install -r requirements.txt
python run.py



## Screenshots

### Pipeline Selection
![pipeline](screenshots/pipeline.png)

### Extraction Interface
![analysis](screenshots/analysis.png)

### Highlighted Results
![highlight](screenshots/highlight.png)

## Future Improvements

- Multi-country adaptive parsing rules
- Multi-model extraction strategy
- Semantic matching for case lifecycle tracking
- Automated update of case timelines in database
