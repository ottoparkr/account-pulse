# Advertiser Pulse

A concept dashboard for an account manager overseeing multiple ChatGPT advertisers. It keeps the original three-column account intelligence layout and adapts it to advertiser portfolios, campaign outcomes, budget pacing, and account planning.

## Explore the prototype

- Search eight fictional advertisers and filter by status or account priority.
- Review monthly spend, outcome counts, CPA goals, and budget pacing.
- Filter sample signals across performance, budget, creative, measurement, launches, relationships, and competition.
- Generate a signal-specific action plan and editable advertiser email, or combine multiple signals into one plan.
- Review stakeholder priorities, success criteria, and account strategy.

All advertiser records, metrics, and reporting inputs are sample data. This is an independent concept, with no live ChatGPT advertising integration. Email addresses use the reserved `.example` domain; replace them before sending.

## Run it

No build step or npm installation is required. Serve the checkout with Python:

```sh
python3 -m http.server 8000 --directory .
```

Open `aq-signals-codex.html` from the server. The source version loads React 18.3.1 and ReactDOM from cdnjs.cloudflare.com, so that host must be accessible.

The downloadable standalone version embeds React and ReactDOM and can render without network access. Save it as an `.html` file and open it in a browser. Changes made to source here do not automatically update previously downloaded copies. Draft edits are temporary and reset when switching signals or reloading.

## Stack

React 18 via CDN, inline JavaScript, and CSS custom properties. The application remains in `aq-signals-codex.html`.
