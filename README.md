# AfterQuery Signals Intelligence

A signal-driven account intelligence tool built to answer one question: **what's happening with this account right now, and what should I do about it?**

## What it does

AfterQuery Signals pulls real-time signals across an account portfolio — funding rounds, hiring patterns, usage anomalies, competitive moves, relationship health — and surfaces them with two outputs:

1. **Outreach draft** — a signal-specific email ready to send, with editable subject, body, and talking points
2. **Relationship intel** — POC profiles with sentiment, communication patterns, and AM coaching notes

The tool is designed for CS and sales teams managing complex accounts where timing is everything. A funding signal at the wrong moment is noise. The same signal paired with a contract renewal 90 days out is an expansion conversation.

## Why I built this

I built this as a forcing function for how I think about account coverage.

Most signal tools tell you what happened. They don't tell you what to do. The gap is context: who are you talking to, what do they actually care about, where are you in the contract cycle, and what's the highest-leverage move right now.

This tool connects those dots. The outreach logic isn't LLM-generated filler — it's templated reasoning that mirrors how a senior CS leader actually thinks about signal response. A competitor signal on a churn-risk account with 4 months to renewal hits differently than the same signal on a healthy expansion account, and the outreach reflects that.

## How to run it

No build step. No dependencies to install.

```
open index.html
```

Or drop it into any static file host (GitHub Pages, Vercel, etc.).

## Stack

- React 18 (CDN, no bundler)
- Vanilla JS — all logic inlined, no framework
- CSS custom properties for the design system
- Zero npm dependencies

## What it demonstrates

- How I think about account segmentation and signal prioritization
- Outreach logic that accounts for contract stage, relationship health, and signal type combinations
- A working prototype built fast, without engineering resources

---

Built by Otto Rojanapairat as a work sample for the OpenAI SMB Innovation Sales and Strategy Lead role.
