# ProposalPal AI

[![Buy ProposalPal AI](https://img.shields.io/badge/Buy_on_Gumroad-proposalpal-brightgreen?logo=gumroad&style=for-the-badge)](https://aivorasol.gumroad.com/l/proposalpal)

ProposalPal AI is a Streamlit application that automatically crafts polished freelance proposals from your client’s project brief using GPT‑4. Select a built‑in template or allow the AI to compose a custom proposal including an introduction, problem statement, solution overview, deliverables, timeline, pricing and a clear call to action — all tailored to the tone you specify.

In addition to AI‑generated proposals, ProposalPal includes three professional templates (basic, startup and agency) available in both Markdown and DOCX formats. You can customise these templates with your name and project duration, or let the AI generate everything from scratch.

## ✨ Key Features

- **AI‑Generated Proposals** – Generate comprehensive proposals from client briefs using GPT‑4. Choose your tone, pricing and expected duration.
- **Built‑In Templates** – Three ready‑to‑use proposal templates (basic, startup and agency) in Markdown and DOCX that you can customise without invoking the AI.
- **One‑Click Exports** – Download your proposal as Markdown, PDF or DOCX files. Optional dependencies enable rich PDF & Word output.
- **Local & Private** – All processing runs on your machine. Your project data remains private, and only your OpenAI API key is used for generation.
- **Customisable** – Modify or add your own templates to the `/templates` folder, or extend the prompt logic in `utils/prompt_generator.py`.

## 🚀 Quick Start

1. Ensure you have **Python 3.9 or higher** installed.  
2. Install the core dependencies:

   ```bash
   pip install -r requirements.txt
   ```

   For PDF and DOCX export support, install the full set of optional dependencies:

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

5. Fill out the form with your name, the client’s name, project brief, expected duration, tone, pricing and whether to use the AI or a template. Then download your proposal in the format you prefer.

### Troubleshooting & Tips

- If the app warns that no API key is found, create a `.env` file with `OPENAI_API_KEY=sk-...`. Without a key the app will fall back to templates only.
- Install `reportlab` for PDF export and `python-docx` for Word export. Both are listed in `requirements-full.txt`.
- To add new templates, drop additional Markdown files into the `templates/` folder and they will appear in the UI.

---

Ready to level up your proposals? Get the full ProposalPal AI package here: [ProposalPal AI on Gumroad](https://aivorasol.gumroad.com/l/proposalpal).
