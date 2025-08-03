# ApplyMate AI

[Buy ApplyMate AI on Gumroad](https://aivorasol.gumroad.com/l/lexvion)

[![QA‑Validated](https://img.shields.io/badge/QA--Validated-brightgreen)](https://aivorasol.gumroad.com) [![Operator‑Built](https://img.shields.io/badge/Operator--Built-blue)](https://github.com/Bigmannot23)

ApplyMate AI is a local Streamlit application that helps you land your dream job by automating resume parsing, job description analysis and cover letter generation. It scores how well your resume matches each job, suggests tailored improvements and even prepares interview Q&A and LinkedIn profile tweaks — all running locally on your machine.

## Who It's For

Job seekers, career changers, freelance professionals and recent grads who want to apply smarter, not harder. If you're spending hours tweaking resumes and cover letters for each application, ApplyMate AI helps you stand out with targeted content — without sending your data to the cloud.

## Key Features

- Resume Parser – Upload a PDF/DOCX or paste your resume to extract the plain text for analysis.
- Job Description Analyzer – Paste multiple job descriptions at once and extract keywords and required skills.
- Match Scoring & Keywords – See a percentage match score and a list of matching keywords for every job.
- Cover-Letter Generator – Draft personalized cover letters using GPT-powered prompts. Choose from Professional, Friendly, Technical or Creative tones — or supply your own.
- Resume Suggestion Engine – Get targeted suggestions to tweak your resume for better ATS & recruiter alignment.
- Interview Q&A Generator – Generate potential interview questions with model answers tailored to your resume and the job description.
- Multi-language Support – Switch between English, Español, Français and Deutsch from the sidebar.
- Batch Mode – Process multiple job descriptions in one run and export all letters and Q&A in Markdown, PDF or DOCX.

## How To Install & Use

1. **Prerequisites:**
   - Python 3.9 or higher installed.
   - A modern web browser (the app runs locally via Streamlit).
   - Optional: An OpenAI API key to unlock AI-powered cover letters, suggestions and Q&A generation. Without it the app falls back to template responses.
2. **Install Dependencies:**
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
3. **Configure:**
   - Copy `.env.example` from the product package to `.env` and edit it with your OpenAI API key:
   - ```
OPENAI_API_KEY=sk-...
```
   - Leave other values blank to disable integrations (email notifications, Slack, etc.).
4. **Run:**
   Run the Streamlit application:
   ```
streamlit run app.py
```
   Your default browser will open the dashboard automatically. If it doesn't, copy the URL printed in the terminal (usually `http://localhost:8501`).
5. **Manage & Use:**
   - Upload or paste your resume (PDF, DOCX or plain text) in the sidebar.
   - Paste one or more job descriptions, select your language and tone and click **Generate**.
   - Review the match scores, keywords, cover letter and Q&A suggestions. Export any output as Markdown, PDF or DOCX.
   - In Batch Mode, upload a CSV with columns `job_title` and `description` to generate content for multiple applications at once.

For a full walkthrough, see the QuickStart and Troubleshooting guides included.

## Refund & Support Policy

We stand behind our tools. If this product doesn’t save you time or deliver results within 60 days, contact us for a full refund. For support or questions, email [theaivorasol@gmail.com](mailto:theaivorasol@gmail.com) or connect on [LinkedIn](https://www.linkedin.com/in/lexvion).

## Attribution

Built by Lexvion Solutions. Explore more tools and automations at [https://aivorasol.gumroad.com](https://aivorasol.gumroad.com).
