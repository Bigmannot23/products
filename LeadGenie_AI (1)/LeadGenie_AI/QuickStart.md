# Quick Start Guide

This guide will get you up and running with LeadGenie AI in a few minutes. If you encounter issues, see the Troubleshooting document.

## 1. Prerequisites

- Python 3.9 or higher installed.
- A modern web browser.
- Optional: OpenAI API key for AI‑assisted copy generation. Without it the app will use the default template text.

## 2. Installation

Create and activate a virtual environment:
```
python3 -m venv venv
source venv/bin/activate
```
Install core dependencies:
```
pip install -r requirements.txt
```
For PDF & DOCX export and optional features, install full dependencies:
```
pip install -r requirements-full.txt
```

## 3. Configure Environment Variables

- Copy `.env.example` to `.env` and set your `OPENAI_API_KEY`.
- Adjust `config.yml` to define default tones, follow‑up cadences and supported channels.

## 4. Customise Your Setup

- Edit or add outreach templates in the `templates/` folder.
- To plug in research enrichment, implement a provider in `data_enrichment/` and reference it in `config.yml`.

## 5. Launch the App

Run the app:
```
streamlit run app.py
```

## 6. Using the App

- In Single Mode, fill out the lead details, pick a template, tone and channels, then click **Generate**.
- In Bulk Mode, upload a CSV with columns `name,company,job_link,angle` and download your CSV of generated messages.
- Review and edit messages in the UI; export as needed.

## 7. Updating & Extending

- Add new tones or channels by editing `config.yml`.
- Build additional export formats or CRM integrations in the `exports/` directory.

Enjoy streamlining your workflow!
