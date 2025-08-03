# GigNavigator AI

**[Buy GigNavigator AI on Gumroad](https://aivorasol.gumroad.com/l/gignav)**

GigNavigator AI is the ultimate AI‑powered job aggregation and outreach assistant for freelancers and consultants.  It scans 20+ sources including LinkedIn Jobs, Indeed, Upwork, Freelancer, Remote OK, AngelList, Reddit and company career pages.  Using AI summarisation and recency‑aware match scoring, it ranks gigs by how well they fit your skills and even explains the score.  With one click you can generate personalised outreach messages in friendly, formal or persuasive tones and manage your leads through a built‑in pipeline tracker.

## Who It's For

If you're a freelance writer, designer, developer, marketer or consultant who's tired of crowded marketplaces and low‑quality leads, GigNavigator AI helps you discover high‑paying opportunities before everyone else.  It runs locally so your data remains private and you can work offline or online.

## Key Features

- **Multi‑Source Aggregation:** Pull gigs from 20+ sources (LinkedIn, Indeed, Upwork, Freelancer, Reddit, Remote OK, AngelList, custom company sites etc.) in one dashboard.
- **AI Job Description Analyzer:** GPT‑powered summaries, recency‑aware match scoring and highlighted keywords show why each gig matters.
- **Multiple Outreach Tones:** Generate emails, DMs or cover letters in friendly, formal or persuasive styles with proven templates.
- **1‑Click Outreach:** Craft tailored messages instantly; export them as Markdown or text and copy with a click.
- **Pipeline & Export:** Save leads to a Kanban‑style tracker and export to CSV or Notion.
- **Demo Mode & Onboarding:** Guided walkthrough and offline demo dataset so you can explore without setup.
- **Privacy First:** All processing happens locally; no data leaves your machine.  Optional API keys enable AI and source‑specific features.

## How To Install & Use

1. **Prerequisites:** Python 3.10+ and a modern browser.  Optional: OpenAI API key and other API tokens (Twitter, Upwork) in a `.env` file to unlock AI features.
2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   # For optional AI & notifications
   pip install -r requirements-full.txt
   ```
3. **Configure:** Copy `.env.example` from the product package to `.env` and edit your API keys.  Edit `config.yml` to enable or disable sources and set keywords.
4. **Run:** Start the Streamlit app with:
   ```bash
   streamlit run app.py
   ```
   Load your profile in the sidebar, enable Demo Mode for an instant preview or run a scan to find real gigs.
5. **Manage Leads:** Save promising gigs to your pipeline, move them through stages and export when needed.

For a full walkthrough, see the [QuickStart](QuickStart.md) and [Troubleshooting](Troubleshooting.md) guides included.

## Refund & Support Policy

We stand behind our tools.  If GigNavigator AI doesn’t save you time or help you land new work within 60 days, contact us for a full refund.  For support or questions, email [support@lexvion.com](mailto:theaivorasol@gmai.com) or connect on [LinkedIn](https://www.linkedin.com/company/lexvion-solutions/).

## Attribution

Built by Lexvion Solutions.  Explore more tools and automations at **[https://aivorasol.gumroad.com](https://aivorasol.gumroad.com)**.

**[Buy GigNavigator AI on Gumroad](https://aivorasol.gumroad.com/l/gignav)**