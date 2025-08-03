# ProposalPal AI

[Buy ProposalPal AI on Gumroad](https://aivorasol.gumroad.com/l/proposalpal)

[![QA‑Validated](https://img.shields.io/badge/QA--Validated-brightgreen)](https://aivorasol.gumroad.com) [![Operator‑Built](https://img.shields.io/badge/Operator--Built-blue)](https://github.com/Bigmannot23)

ProposalPal AI is a Streamlit application that automatically crafts polished freelance proposals from your client's project brief using GPT‑4. Select a built‑in template or allow the AI to compose a custom proposal including an introduction, problem statement, solution overview, deliverables, timeline, pricing and a clear call to action — all tailored to the tone you specify.

## Who It's For

Freelancers, agencies and indie consultants who spend too much time writing proposals instead of delivering work. Whether you need a quick template or a custom AI draft, ProposalPal AI helps you respond faster and win more projects.

## Key Features

- AI‑Generated Proposals – Generate comprehensive proposals from client briefs using GPT‑4. Choose your tone, price and expected duration.
- Built‑In Templates – Three ready‑to‑use proposal templates (basic, startup and agency) in Markdown and DOCX that you can customise without invoking the AI.
- Pricing & Timeline Presets – Pre‑fill line items and pricing tiers; adjust manually or let AI suggest numbers.
- One‑Click Export – Export your proposal as a polished PDF, Markdown or DOCX file with your branding.
- Multiple Tones – Choose from Formal, Friendly, Persuasive or Custom; supports multiple languages.
- Collaboration Ready – Provide an editable document you can share or convert to Notion.
- Local & Private – Runs entirely on your machine; only uses your OpenAI key when generating AI proposals.

## How To Install & Use

1. **Prerequisites:**
   - Python 3.9 or higher installed.
   - Modern web browser.
   - Optional: OpenAI API key to enable AI‑generated proposals.
2. **Install Dependencies:**
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
3. **Configure:**
   - Copy `.env.example` to `.env` and set `OPENAI_API_KEY`.
   - Adjust `config.yml` to customise default sections, pricing tiers and available tones.
4. **Run:**
   Start the app:
   ```
streamlit run app.py
```
5. **Manage & Use:**
   - Enter the client's name, project brief, expected duration and pricing details in the form.
   - Select a tone and whether to use AI or a built‑in template.
   - Click **Generate Proposal**. Review the generated proposal, edit as needed and export it in your desired format.

For a full walkthrough, see the QuickStart and Troubleshooting guides included.

## Refund & Support Policy

We stand behind our tools. If this product doesn’t save you time or deliver results within 60 days, contact us for a full refund. For support or questions, email [theaivorasol@gmail.com](mailto:theaivorasol@gmail.com) or connect on [LinkedIn](https://www.linkedin.com/in/lexvion).

## Attribution

Built by Lexvion Solutions. Explore more tools and automations at [https://aivorasol.gumroad.com](https://aivorasol.gumroad.com).
