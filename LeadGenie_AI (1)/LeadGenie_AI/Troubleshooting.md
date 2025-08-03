# Troubleshooting

This page lists common issues you might encounter when using LeadGenie AI and how to resolve them.

## No Messages Generated

- Check that your CSV contains the required columns (`name`, `company`, `job_link`, `angle`).
- Ensure you selected at least one output channel and a template.
- If using AI assist, verify your API key is set and valid.

## AI Errors

- Invalid API key: Ensure `OPENAI_API_KEY` is present in `.env`.
- API rate limits: Too many requests may result in 429 errors. Wait and try again.
- Unexpected content: If AI returns unusable text, the app will default to the base template.

## Export Problems

- PDF export requires `reportlab` and `pdfkit`; DOCX export requires `python-docx`. Install optional deps.
- Ensure `wkhtmltopdf` is installed for PDF export.

## UI Issues

- Copy the local Streamlit URL (e.g., `http://localhost:8501`) into your browser if it doesn't open automatically.
- If widgets freeze, refresh the browser tab or restart the app.

