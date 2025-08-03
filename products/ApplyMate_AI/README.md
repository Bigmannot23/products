# ApplyMate AI

[![Buy ApplyMate AI](https://img.shields.io/badge/Buy_on_Gumroad-lexvion-brightgreen?logo=gumroad&style=for-the-badge)](https://aivorasol.gumroad.com/l/lexvion)

ApplyMate AI is a local Streamlit application that helps you land your dream job by automating resume parsing, job description analysis and cover‑letter generation. It scores how well your resume matches each job, suggests tailored improvements and even prepares interview Q&A and LinkedIn profile tweaks — all running locally on your machine.

## ✨ Key Features

- **Resume Parser** – Upload a PDF/DOCX or paste your resume to extract the plain text for analysis.
- **Job Description Analyzer** – Paste multiple job descriptions at once and extract keywords and required skills.
- **Match Scoring & Keywords** – See a percentage match score and a list of matching keywords for every job.
- **Cover‑Letter Generator** – Draft personalized cover letters using GPT‑powered prompts. Choose from Professional, Friendly, Technical or Creative tones — or supply your own.
- **Resume Suggestion Engine** – Get targeted suggestions to tweak your resume for better ATS & recruiter alignment.
- **Interview Q&A Generator** – Receive likely interview questions with model answers tailored to your experience.
- **LinkedIn Optimizer** – Analyse your resume and propose improvements to your LinkedIn headline and summary.
- **Batch Mode** – Process multiple job descriptions in one run and export all letters and Q&A in Markdown, PDF or DOCX.

Everything runs locally and your resume data remains private. The app supports English, Spanish, French and German.

## 🚀 Quick Start

1. Ensure you have **Python 3.9 or higher** installed.  
2. Install the core dependencies:

   ```bash
   pip install -r requirements.txt
   ```

   For DOCX and PDF export support, install the full set of optional dependencies:

   ```bash
   pip install -r requirements-full.txt
   ```

3. Create a `.env` file in the project root and add your OpenAI API key:

   ```ini
   OPENAI_API_KEY=sk-...
   ```

4. Run the app locally with Streamlit:

   ```bash
   streamlit run app.py
   ```

5. Use the sidebar to choose your language and whether you’re working on a single application or batch mode. Upload your resume, paste job descriptions, select a tone and click **Generate**.

### Troubleshooting & Tips

- If the sidebar warns that no API key is configured, add your key to a `.env` file. Without a key the app will use template responses.
- Install `python-docx` for Word export and `matplotlib` for PDF export.
- Ensure your CSV includes required columns (`job_title, description`) when using batch mode.

---

Use [ApplyMate AI on Gumroad](https://aivorasol.gumroad.com/l/lexvion) to get the full codebase, templates and assets.
