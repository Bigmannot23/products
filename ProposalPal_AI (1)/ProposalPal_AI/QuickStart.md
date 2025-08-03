# Quick Start Guide

This guide will get you up and running with ProposalPal AI in a few minutes. If you encounter issues, see the Troubleshooting document.

## 1. Prerequisites

- Python 3.9 or higher installed.
- Modern web browser.
- Optional: OpenAI API key to enable AI‑generated proposals.

## 2. Installation

Create and activate a virtual environment:
```
python3 -m venv venv
source venv/bin/activate
```
Install required packages:
```
pip install -r requirements.txt
```
For PDF/DOCX export and advanced features:
```
pip install -r requirements-full.txt
```

## 3. Configure Environment Variables

- Copy `.env.example` to `.env` and set `OPENAI_API_KEY`.
- Adjust `config.yml` to customise default sections, pricing tiers and available tones.

## 4. Customise Your Setup

- Edit the templates in `templates/` (Markdown or DOCX) or add your own.
- Modify prompts in `ai_engine/prompts/` to change how the AI structures proposals.

## 5. Launch the App

Start the app:
```
streamlit run app.py
```

## 6. Using the App

- Enter the client's name, project brief, expected duration and pricing details in the form.
- Select a tone and whether to use AI or a built‑in template.
- Click **Generate Proposal**. Review the generated proposal, edit as needed and export it in your desired format.

## 7. Updating & Extending

- Add new proposal templates to the `templates/` folder.
- Implement custom export formats (e.g., HTML, LaTeX) in the `exports/` directory.

Enjoy streamlining your workflow!
