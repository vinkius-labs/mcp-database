# Tech Trigger Radar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tech-trigger-radar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lead-generation](../categories/lead-generation.md)

Keyless technical and demand signals for outbound targeting — subdomains that just appeared, the stack behind a domain, its public age, how the market phrases a need, and what is trending now. No key, no account.

## Description
The best outbound openings are not in your CRM — they are in what targets do to their websites, products and the market's own search behavior. This MCP reads those footprints from public sources, with no key and no account anywhere in the chain.

### What you can do

- **Catch new surface** — every subdomain a domain has ever served a TLS certificate for shows up in the public certificate log. Reading the ones first seen inside your window is the "they just launched something" trigger: new product, new region, new portal.
- **Finger the stack** — where the domain is hosted, what mail it runs, which recognizable systems it exposes, from its own published DNS records. Targeting language, not claims: every detection is labelled as a heuristic.
- **Measure public age** — how long the domain has been publicly serving TLS. A young reading is a real "just launched" signal; the tool says plainly it is an observation, not the registration date.
- **Read the market's wording** — what people actually type after your product phrase, in frequency order, optionally scoped to a country. That is the language to mirror in subject lines and the queries to qualify active lookers.
- **Watch what is trending** — the live trending-searches feed for a region, plus a demand pulse that says whether commercial variants (alternatives, pricing, best-of) of your keyword are being searched at all.

### How it works

The server combines the public certificate-transparency log, public DNS lookups, the public autocomplete endpoint and the public trending feed. Certificate readings are cached for an hour; when a source is slow or rate-limited the result says "source unavailable — retry in a few minutes" instead of returning a fake empty, so an unavailable reading is never mistaken for a negative signal.

### Who is this for

Outbound teams and founders who need technical and demand triggers: which targets just shipped something, what they run, how the market phrases the need and what is hot right now — all from public data, no credentials.


## Available Tools (6)
- **search_suggestions**: This is how the market phrases the need: the top lines are the exact search terms to use for target qualification and the wording to mirror in subject lines and ads. An empty list is a signal in itself — the phrase carries little search weight, either because the need is unfamiliar or the phrase is too generic. If the source does not answer, the result says it is unavailable rather than empty.

What people actually type after a product phrase, in frequency order — the market's own wording. Keyless
- **subdomain_watch**: A new subdomain is new surface: a new product, region, portal or integration, and the name itself ("ai-", "beta-", "api-") is the read. This is the "they just launched something" trigger for an outreach. Two caveats to carry: the dates are first observations in the public log, not exact deploy dates, and if the log is rate-limited the result says the source is unavailable and to retry in a few minutes — that answer is not the same as "no new subdomains", so do not report it that way.

Subdomains of a domain whose certificates first appeared inside a window — new product surface, keyless, from the public certificate log
- **demand_pulse**: The pulse field is the read: "active" means commercial variants are being searched, which is live buying intent to intercept; "quiet" means the commercial variants have no weight, so lead with the product phrasing instead; "partial" means some sources did not answer. Use the returned phrasings verbatim as targeting language. The phrase list for the base term tells you the shape of the need itself.

How the market phrases a keyword right now, whether commercial variants are searched, and if it is trending. Keyless
- **domain_age**: A young reading is a real "just launched" signal — a brand-new product surface is a warm target. Read it as an observation, not a fact: it is the earliest certificate in the public log, not the registration date, so a mature domain can read younger than it is. A domain with no observations is reported as such (often new or low-traffic), and a rate-limited log is reported as unavailable, never as "new".

How long the domain has been publicly serving TLS — its first observed certificate, keyless
- **stack_fingerprint**: Every detection is a pattern match on records the domain itself publishes: use it for targeting language ("you run X, we do Y"), not as a claim. An empty detection list means nothing recognizable matched, not that nothing is running; if the DNS lookups fail, the result says the source is unavailable and to retry. The raw records are included so the agent can reason over them directly.

Where the domain is hosted and whose mail it runs, heuristically from public DNS records. Keyless
- **trending_now**: A trending term adjacent to your product is a top-of-funnel window: timely content, an ad hook or a "saw this, thought of you" outreach line. Traffic is an approximation, not a count. If the feed does not answer, the result says it is unavailable, not that nothing is trending.

The live trending searches for a region, with approximate traffic. Keyless


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tech Trigger Radar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Has Figma launched anything new in the last month? Check its new subdomains."

**🤖 AI Agent:**
> 🕸️ **New surface: figma.com · last 30 days**

2 subdomains first observed in the window:
- `community-ai.figma.com` — first seen 2026-09-12, 10 days ago
- `status-eu.figma.com` — first seen 2026-09-05, 17 days ago

Read: a new AI-adjacent product surface and a new EU region both shipped in the last three weeks. The AI-surface launch is the warm hook — reach them while it is new.

---

**👤 You:**
> "What does acme.com run on, and whose mail does it use?"

**🤖 AI Agent:**
> 🔍 **Stack fingerprint: acme.com**

Detected (heuristic): AWS CloudFront (CDN) · Google / Firebase
Mail system: Google Workspace mail
Raw: CNAME `www` → d1234.cloudfront.net · MX → aspmx.l.google.com

Targeting read: they front with CloudFront and run Google mail — a "we integrate with the stack you already publish" angle is grounded.

---

**👤 You:**
> "How do people phrase "crm for startups" in search? Give me the language to mirror."

**🤖 AI Agent:**
> 📈 **Autocomplete: "crm for startups"**

Top phrasings, in frequency order:
1. crm for startups free
2. crm for startups small business
3. best crm for startups under 10 employees

Mirror these exactly in subject lines — "free" and "small business" lead the need, so lead with cost and team-size, not features. Use query 1 to qualify who is actively looking.


## ❓ FAQ

**Q: Do I need an API key or an account?**
No. Every source is public: the certificate-transparency log, public DNS, the public autocomplete endpoint and the public trending feed. There is no credential anywhere in the chain — nothing to issue, rotate or store.

**Q: What exactly is a "new subdomain" signal?**
Every website that serves HTTPS issues a public certificate, and every certificate is recorded in the public transparency log. A subdomain whose certificate first appears inside your window is new public surface: a new product, region, portal or integration. The tool returns them newest first with their first-observed date — and says plainly that the date is an observation, not the exact deploy time.

**Q: Is the stack fingerprint a fact about the company?**
No — it is a labelled heuristic. The engine matches the domain's own published DNS records (CNAME, MX, TXT) against known provider patterns, so each detection means "very likely this provider", never "confirmed". Use it for targeting language — "you run X, we do Y" — and lean on the raw records in the result when you want to reason further.

**Q: What happens when a source is slow or rate-limited?**
Certificate readings are cached for an hour, so repeating a scan minutes apart is free. When a source does not answer, the result carries an explicit "source unavailable" flag and a note to retry in a few minutes — it is never reported as "no data", because an unavailable reading and a genuine negative are different facts and mixing them up would mislead the outreach.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tech-trigger-radar](https://vinkius.com/en/ai-agent-connect/tech-trigger-radar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tech Trigger Radar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tech-trigger-radar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tech Trigger Radar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tech-trigger-radar": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
