# Troubleshooting

This page lists common issues you might encounter when using **GigNavigator AI** and how to resolve them.

## No Gigs Are Returned

- **Check your keywords**: Broad keywords may result in no matches if you’re searching in a niche.  Adjust the `keywords` list in `config.yml` to be more specific or generic depending on your field.
- **Verify sources are enabled**: Ensure the sources you want (e.g. `linkedin_jobs`, `indeed`, `twitter_search`) are set to `enabled: true` in the configuration.
- **API keys or authentication missing**: Some adapters require API tokens (e.g. Twitter) or session cookies (LinkedIn).  Provide these in your `.env` file and restart the app.

## OpenAI Errors

- **API key missing or invalid**: Make sure your `OPENAI_API_KEY` is set correctly in `.env`.  Without a valid key, the app falls back to basic keyword matching.
- **Rate limits**: If you see errors like `429 Too Many Requests`, you may have exceeded your OpenAI quota.  Try again later or upgrade your plan.
- **Unexpected response**: Sometimes GPT responses can’t be parsed.  In this case the app will fall back to heuristic scoring and summarise the description directly.

## Network or Scraping Issues

- **Connection errors**: If the app cannot reach a source, check your internet connection and verify that the site is accessible.  Proxy or VPN settings might block the request.
- **HTML structure changes**: Sites often update their HTML, which can break scrapers.  For first‑party sources (LinkedIn, Indeed, etc.), watch for breaking changes and update the corresponding adapter in `data_sources/`.

## Database or File Errors

- **Cannot open leads.sqlite**: Ensure that the `db/` directory is writable.  If the SQLite file is locked or corrupted, stop the app, delete the file and restart; a new database will be created automatically.
- **Profile not saved**: The user profile is stored in `db/user_profile.json`.  If you see errors when loading the profile, check that the file contains valid JSON.  You can delete it to reset your profile.

## UI or Streamlit Errors

- **App doesn’t open in browser**: Streamlit prints a local URL in the terminal (usually `http://localhost:8501`).  Copy and paste this into your browser if it doesn’t open automatically.
- **Widgets unresponsive**: Refresh the page or stop and restart the Streamlit server.  Sometimes cached state can cause widgets to freeze.

If you encounter a bug not listed here, please open an issue on the repository with as much detail as possible (error logs, OS information, steps to reproduce) so we can investigate.
