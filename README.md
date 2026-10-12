# Advertiser Pulse

A concept dashboard for an account manager overseeing multiple ChatGPT advertisers. It keeps the original three-column account intelligence layout and adapts it to advertiser portfolios, campaign outcomes, budget pacing, and account planning.

## Explore the prototype

- Search twelve fictional advertisers and filter by status or account priority, including **Newly onboarded** and **Spend opportunity**.
- Scan a compact spend row and thin budget bar alongside performance metrics. Opportunity and approved-expansion badges open the relevant Account context section. Detailed periods, approvals, pacing, and forecasts stay in that panel. Unapproved budgets show no consumption bar.
- Compare Northstar's proposed $20K incremental upsell (excluded from its $60K approved budget) with Bloom's approved $15K expansion ($45K original + $15K approved = $60K current budget).
- Filter sample signals across onboarding, funding, company growth, hiring, performance, budget, creative, measurement, launches, relationships, and competition.
- Explore four newly onboarded accounts with funding announcements, launch and expansion plans, proposed next-test budgets, and account-specific readiness checks.
- Generate a signal-specific action plan and editable advertiser email, or combine multiple signals into one plan.
- Review stakeholder priorities, success criteria, and account strategy.
- Track a sample $400K quarterly quota in a collapsible top bar. It starts collapsed with attainment visible; **Show quota** opens the full forecast and pipeline breakdown. Expansion preference is remembered locally when browser storage is available. Account selection and filters do not change portfolio totals.
- Review each advertiser's quarterly contribution and forecast basis in **Account context**. Proposed next-test budgets are compared with their current starter-budget baseline to show incremental potential, with future-test opportunities kept outside the current-quarter pipeline.

All advertiser records, metrics, and reporting inputs are sample data. This is an independent concept, with no live ChatGPT advertising integration. Email addresses use the reserved `.example` domain; replace them before sending.

Spend-opportunity ranges are illustrative proposals, not approved budgets or performance forecasts. Funding and company-growth signals support discovery; they do not establish available advertising allocation. Newly onboarded accounts label CPA as early and omit monthly projections during their first seven days.

The budget cards use dated sample periods and a sample snapshot of September 18, 2026. Only approved increases effective in the current period are included in the budget denominator. Next-test proposals refer to a separate future period. Budget consumed measures spending rather than campaign success; review CPA and outcome quality alongside it.

The sample quota period is Q3 2026 (July 1–September 30), as of September 18. Credit equals 100% of delivered ad spend on assigned accounts. Approved budgets do not earn credit by themselves. Expected finish adds only estimated remaining-quarter delivery within approved budgets to actual credited spend; open upsells are excluded. Forecast amounts are illustrative account assumptions, not performance predictions or live revenue data.

## Run it

No build step or npm installation is required. Serve the checkout with Python:

```sh
python3 -m http.server 8000 --directory .
```

Open `aq-signals-codex.html` from the server. The source version loads React 18.3.1 and ReactDOM from cdnjs.cloudflare.com, so that host must be accessible.

The downloadable standalone version embeds React and ReactDOM and can render without network access. Save it as an `.html` file and open it in a browser. Changes made to source here do not automatically update previously downloaded copies. Draft edits are temporary and reset when switching signals or reloading.

## Stack

React 18 via CDN, inline JavaScript, and CSS custom properties. The application remains in `aq-signals-codex.html`.
