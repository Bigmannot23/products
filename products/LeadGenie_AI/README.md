# LeadGenie AI

[![Buy LeadGenie AI](https://img.shields.io/badge/Buy_on_Gumroad-leadgenie-brightgreen?logo=gumroad&style=for-the-badge)](https://aivorasol.gumroad.com/l/leadgenie)

LeadGenie AI is a local Streamlit application that helps you craft personalized cold‑outreach messages at scale. Whether you’re sending a single note or a mail merge to hundreds of leads, LeadGenie guides you through template selection, optional research enrichment, tone selection and multi‑channel copy generation — all in your preferred language.

## ✨ Key Features

- **Single & Bulk Mode** – Generate a message for one lead or upload a CSV of hundreds of leads and download a mail‑merge‑ready file.
- **AI Research Assist** – Optionally enrich your message with a company tagline, recent press or social posts (stubbed; plug in your own APIs).
- **Template Library** – Five proven outreach templates (book a call, audit offer, direct pitch, free resource, networking) editable in the `/templates` folder.
- **Tone/Persona Switcher** – Choose from Friendly, Formal, SaaS Founder, Copywriter or define your own tone.
- **Multi‑Channel Output** – Generate copy tailored for Email, LinkedIn DM, Twitter DM and Upwork.
- **Follow‑Up Sequence** – Generate up to three follow‑up messages per lead to continue the conversation.
- **Exports & CRM Ready** – Download messages as TXT/MD/PDF/DOCX for individual leads or as a CSV (Notion‑ready template included) for bulk sends.
- **Multilingual UI** – Switch between English, Español, Français and Deutsch from the sidebar.

Your data stays local — only your OpenAI API key is used for generation, and you can easily plug in your own data enrichment.

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

5. In Single Mode, fill out the lead details, choose a template, tone and channels, then click **Generate messages**. In Bulk Mode, upload a CSV with columns `name,company,job_link,angle` and download your CSV of generated messages.

### Troubleshooting & Tips

- If the sidebar warns that the API key is missing, ensure your `.env` contains a valid `OPENAI_API_KEY`. Without a key the app falls back to deterministic templates.
- Install `python-docx` for Word export and `matplotlib` for PDF export.  A Notion CRM template CSV is located in `/assets`.
- When using bulk mode, ensure your CSV contains the required columns and is properly formatted.

---

Purchase the full LeadGenie AI package on Gumroad for templates, assets and email scripts: [LeadGenie AI on Gumroad](https://aivorasol.gumroad.com/l/leadgenie).
