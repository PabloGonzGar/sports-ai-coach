# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

`sports-ai-coach` is a Python AI/ML project. The tech stack (from `requirements.txt`) includes:

- **ML frameworks**: TensorFlow/Keras, PyTorch, Hugging Face Transformers, scikit-learn
- **LLM integration**: Ollama (local LLMs), sentence-transformers
- **Model serving**: FastAPI + Uvicorn, Flask
- **Model optimization**: ONNX, ONNX Runtime, Optimum
- **NLP**: spaCy, Transformers tokenizers
- **Data**: pandas, numpy, datasets (HuggingFace), openpyxl
- **Visualization**: matplotlib, seaborn, plotly
- **PDF/document parsing**: PyMuPDF, pdfplumber, python-docx
- **Notebooks**: JupyterLab

## Environment Setup

```bash
# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
```

A `.env` file is gitignored and expected at the project root for secrets/config.

## Development

Since no build or test tooling is configured yet, commands will be added here as the project matures. For now:

```bash
# Run a Jupyter notebook server
jupyter lab

# Run a FastAPI server (once an entrypoint exists)
uvicorn <module>:<app> --reload
```
