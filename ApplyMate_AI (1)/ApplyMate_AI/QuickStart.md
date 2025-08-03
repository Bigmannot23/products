# Quick Start Guide

This guide will get you up and running with ApplyMate AI in a few minutes. If you encounter issues, see the Troubleshooting document.

## 1. Prerequisites

- Python 3.9 or higher installed.
- A modern web browser (the app runs locally via Streamlit).
- Optional: An OpenAI API key to unlock AI-powered cover letters, suggestions and Q&A generation. Without it the app falls back to template responses.

## 2. Installation

Create and activate a virtual environment (recommended):
```
python3 -m venv venv
source venv/bin/activate
```
Install the core dependencies:
```
pip install -r requirements.txt
```
For DOCX and PDF export support, install the full set of optional dependencies:
```
pip install -r requirements-full.txt
```

## 3. Configure Environment Variables

- Copy `.env.example` from the product package to `.env` and edit it with your OpenAI API key:
- ```
OPENAI_API_KEY=sk-...
```
- Leave other values blank to disable integrations (email notifications, Slack, etc.).

## 4. Customise Your Setup

- Open `config.yml` to adjust available tones, target languages and batch defaults.
- Add your own cover letter templates in the `templates/` folder (Markdown or plain text).

## 5. Launch the App

Run the Streamlit application:
```
streamlit run app.py
```
Your default browser will open the dashboard automatically. If it doesn't, copy the URL printed in the terminal (usually `http://localhost:8501`).

## 6. Using the App

- Upload or paste your resume (PDF, DOCX or plain text) in the sidebar.
- Paste one or more job descriptions, select your language and tone and click **Generate**.
- Review the match scores, keywords, cover letter and Q&A suggestions. Export any output as Markdown, PDF or DOCX.
- In Batch Mode, upload a CSV with columns `job_title` and `description` to generate content for multiple applications at once.

## 7. Updating & Extending

- To add new tones, edit `config.yml` under the `tones` section.
- For advanced customisation, modify the prompts in `ai_engine/prompts/` or plug in your own LLM via `llm_provider.py`.

Enjoy streamlining your workflow!
