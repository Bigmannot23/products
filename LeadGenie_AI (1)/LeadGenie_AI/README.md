# LeadGenie AI

[Buy LeadGenie AI on Gumroad](https://aivorasol.gumroad.com/l/leadgenie)

[![QA‑Validated](https://img.shields.io/badge/QA--Validated-brightgreen)](https://aivorasol.gumroad.com) [![Operator‑Built](https://img.shields.io/badge/Operator--Built-blue)](https://github.com/Bigmannot23)

LeadGenie AI is a local Streamlit application that helps you craft personalised cold‑outreach messages at scale. Whether you're sending a single note or a mail merge to hundreds of leads, LeadGenie guides you through template selection, optional research enrichment, tone selection and multi‑channel copy generation — all in your preferred language.

## Who It's For

Freelancers, consultants, agency owners and indie founders who want to generate leads and nurture relationships without sounding like a robot. If you're tired of copy‑pasting generic messages, LeadGenie AI helps you stand out with tailored copy at scale.

## Key Features

- Single & Bulk Mode – Generate a message for one lead or upload a CSV of hundreds of leads and download a mail‑merge‑ready file.
- AI Research Assist – Optionally enrich your message with a company tagline, recent press or social posts (plug in your own APIs).
- Template Library – Five proven outreach templates (book a call, audit offer, direct pitch, free resource, networking) editable in the `/templates` folder.
- Tone/Persona Switcher – Choose from Friendly, Formal, SaaS Founder, Copywriter or define your own tone.
- Multi‑Channel Output – Generate copy tailored for Email, LinkedIn DM, Twitter DM and Upwork.
- Follow‑Up Sequence – Generate up to three follow‑up messages per lead to continue the conversation.
- Exports & CRM Ready – Export generated messages as TXT/MD/PDF/DOCX for individual leads or as a CSV (Notion‑ready template included) for bulk sends.
- Multilingual UI – Switch between English, Español, Français and Deutsch from the sidebar.
- Data stays local – Only your OpenAI API key is used for generation; you can easily plug in your own enrichment provider.

## How To Install & Use

1. **Prerequisites:**
   - Python 3.9 or higher installed.
   - A modern web browser.
   - Optional: OpenAI API key for AI‑assisted copy generation. Without it the app will use the default template text.
2. **Install Dependencies:**
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
3. **Configure:**
   - Copy `.env.example` to `.env` and set your `OPENAI_API_KEY`.
   - Adjust `config.yml` to define default tones, follow‑up cadences and supported channels.
4. **Run:**
   Run the app:
   ```
streamlit run app.py
```
5. **Manage & Use:**
   - In Single Mode, fill out the lead details, pick a template, tone and channels, then click **Generate**.
   - In Bulk Mode, upload a CSV with columns `name,company,job_link,angle` and download your CSV of generated messages.
   - Review and edit messages in the UI; export as needed.

For a full walkthrough, see the QuickStart and Troubleshooting guides included.

## Refund & Support Policy

We stand behind our tools. If this product doesn’t save you time or deliver results within 60 days, contact us for a full refund. For support or questions, email [theaivorasol@gmail.com](mailto:theaivorasol@gmail.com) or connect on [LinkedIn](https://www.linkedin.com/in/lexvion).

## Attribution

Built by Lexvion Solutions. Explore more tools and automations at [https://aivorasol.gumroad.com](https://aivorasol.gumroad.com).
