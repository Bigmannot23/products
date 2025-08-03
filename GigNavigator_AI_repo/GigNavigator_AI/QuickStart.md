# Quick Start Guide

This guide will get you up and running with **GigNavigator AI** in a few minutes.  If you encounter issues, see the [Troubleshooting](Troubleshooting.md) document.

## 1. Prerequisites

- **Python 3.10** or higher installed on your system.
- A modern web browser (the UI runs in your browser via Streamlit).
- (Optional) API keys for OpenAI, Twitter, LinkedIn or other services you plan to use.  Without these keys, the app still functions in offline mode using heuristic scoring.

## 2. Installation

Clone or download the repository and create a virtual environment:

```bash
git clone https://github.com/yourname/GigNavigator_AI.git
cd GigNavigator_AI
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
# Optional extras (AI and notifications)
pip install -r requirements-full.txt
```

## 3. Configure Environment Variables

Copy `.env.example` to `.env` and edit it with your API keys and notification settings.  For example:

```ini
OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
TWITTER_BEARER_TOKEN=your-token-here
ENABLE_EMAIL_NOTIFICATIONS=true
EMAIL_USERNAME=you@example.com
EMAIL_PASSWORD=your-app-password
```

Only the OpenAI key is required for AI features.  Leave other values blank to disable those integrations.

## 4. Customise Your Sources

The `config.yml` file controls which sources are enabled and which keywords are used.  Open it in a text editor and modify it to suit your needs.  For example:

```yaml
sources:
  linkedin_jobs:
    enabled: true
    keywords:
      - "freelance marketer"
      - "contract SEO"
    location: "Remote"
  upwork:
    enabled: false  # enable to include Upwork gigs
    keywords:
      - "marketing"
      - "design"
    location: "Remote"
  freelancer:
    enabled: false  # enable to include Freelancer.com gigs
    keywords:
      - "wordpress"
      - "graphic design"
    location: "Remote"
  twitter_search:
    enabled: true
    query: "freelance marketer OR #hiring marketer"
scan_interval_minutes: 120
```

Save the file when finished.  If you add your own adapter under `data_sources/`, add it here and set `enabled: true` to include it in scans.

## 5. Launch the App

Run the Streamlit application:

```bash
streamlit run app.py
```

Your default browser will open the dashboard.  In the left sidebar you can:

- Upload or paste your **profile** (skills, experience, desired rate).
- Choose to run a **manual scan** or enable **Auto‑Scan** for periodic checks.
- Adjust filters like match score threshold and search keywords.

You can also enable **Demo Mode** from the sidebar.  This mode populates the app with a curated set of sample gigs from all available adapters.  It's perfect for offline use or a quick tour of the features without connecting to external services.  When you're ready for real opportunities, simply disable Demo Mode and run a scan.

When results appear, click a lead to view details, generate outreach messages or save it to your pipeline.

## 6. Managing Your Pipeline

Saved leads appear in the **Pipeline** section.  Use drag‑and‑drop to move leads through stages (e.g. **Potential → Contacted → Interviewing → Won/Lost**).  You can export your pipeline as CSV or import it into Notion using the provided template.

## 7. Updating & Extending

To add new sources, create a module in `data_sources/` implementing `fetch_new_posts()`, then enable it in `config.yml`.  For advanced AI behaviour, edit the prompts in `ai_engine/prompts/` or add new templates in `templates/`.

When updating the tool, check the [Changelog](Changelog.md) for new features and migration instructions.

Enjoy streamlining your freelance client search!
