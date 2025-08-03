# Troubleshooting

This page lists common issues you might encounter when using ProposalPal AI and how to resolve them.

## Empty or Incomplete Proposals

- Ensure you entered a project brief with enough detail; AI needs context to generate relevant content.
- Verify that a tone and template were selected.
- If using AI generation, check that your API key is valid.

## Export Failures

- PDF export requires `reportlab` and `pdfkit`; DOCX export uses `python-docx`. Install optional dependencies.
- Make sure `wkhtmltopdf` is installed and on your PATH for PDF export.

## Formatting Issues

- Try editing the Markdown output directly if the layout isn't perfect.
- Adjust line items or sections in `config.yml` to match your preferred structure.

## App Doesn't Open

- Copy the Streamlit URL from the terminal and paste it into your browser.
- Restart the app if widgets become unresponsive.

