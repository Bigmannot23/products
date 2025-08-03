# Troubleshooting

This page lists common issues you might encounter when using ApplyMate AI and how to resolve them.

## No Results or Low Match Scores

- Ensure the job description includes enough detail (title, responsibilities, required skills).
- Review your keywords in `config.yml` and make them more specific or broad as needed.
- Check that the correct language is selected; mismatched languages can affect keyword extraction.

## API Errors

- Missing or invalid API key: Set `OPENAI_API_KEY` in your `.env` file.
- Rate limits: If you see `429` errors, you may have exceeded your OpenAI quota. Try again later or upgrade your plan.
- Unexpected response: If AI responses cannot be parsed, the app will fall back to template suggestions.

## Export Issues

- DOCX export requires `python-docx` and PDF export requires `reportlab` and `pdfkit`. Install optional deps with `pip install -r requirements-full.txt`.
- Make sure `wkhtmltopdf` is installed and accessible on your system for PDF export.

## UI Problems

- If the app doesn't open automatically, copy the local URL from the terminal and paste it into your browser.
- Widgets unresponsive? Stop and restart Streamlit or clear your browser cache.

