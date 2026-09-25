# Outbound Hiring Signals MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/outbound-hiring-signals)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lead-generation](../categories/lead-generation.md)

Keyless sales-movement detection from public job boards — open roles, how many days ago they were posted, and the commercial mix per company, straight from public Greenhouse boards. No key, no account.

## Description
Every sales team knows the timing truth: the moment a company starts hiring its commercial organization is when it is spending money, expanding motion and receptive to new vendors. This MCP turns that moment into queryable public data — no key, no account, no scraping setup.

### What you can do

- **Probe a company** — confirm it publishes a public job board under a slug (a careers URL works too), before trusting any signal for it.
- **Read the full board** — every open role with location, deadlines and *days since posted*, paged so a big board never floods context.
- **Classify the mix** — open roles grouped by family (GTM/ops, sales, marketing, engineering, leadership) with a one-line commercial read: a company with open sales and marketing roles is visibly investing in growth — that is your timing window.
- **Find the fresh movement** — roles published or updated inside a 1-to-120-day window: the purest "moving right now" trigger.
- **Scan the tracked set** — ask "who is hiring a sales engineer in remote?" across the 21 major companies whose public boards are confirmed, or any keyword and location combination.

### How it works

The server reads the public job-board endpoint that thousands of companies expose at their own slug, and reduces every posting to the fields an attack motion needs: what is open, where, and how long ago it went up. Postings are cached for an hour so repeated scans do not hammer the public source, and rate-limited boards are reported as skipped, never guessed.

### Who is this for

Outbound sales teams, SDRs and agency operators who need to sequence their attack list from public signals: which targets are in a buying mood, which just opened a motion, which are quiet — before writing a single personalized line.


## Available Tools (7)
- **fresh_hiring**: This is the timing trigger of the whole server: a company posting commercial roles inside the window is actively moving and is the warmest outbound target. An empty result on a confirmed board means the board is quiet inside the window — widen the window before concluding the company is not hiring. If the slug has no public board at all, the result says the signal is unavailable, not zero.

Postings on a company job board published or updated within N days — the purest "moving right now" trigger. Keyless
- **probe_board**: g. "stripe", "figma", "okta") — a full careers URL works too, it is reduced to the slug — and reports whether the company has a public board. When it does you get the official company name and the careers page link, so every later tool call is grounded in a confirmed target. When it does not, the answer says the hiring signal is unavailable for this company, which is a different fact from "no open roles": that company runs a different applicant-tracking system or hides its board, and retrying the same slug will keep failing. Use this before trusting any other result for an unknown company.

Check whether a company publishes a public job board under a given slug, and its official name. Keyless
- **role_breakdown**: Classification is by title keywords, one family per role — "Head of Sales" counts as sales, not leadership. This is the fastest way to answer "is this company in a buying mood" from public data alone.

Count a company public openings per role family — GTM, sales, marketing, engineering, leadership — and what it means commercially. Keyless
- **find_hiring**: Use it for "who is hiring a sales engineer in remote right now" style target discovery. The seed set is a starting point: any other company with a public board can be queried directly with its own slug through the per-board tools. If a board was rate-limited during the scan it is reported in the note and skipped, not guessed at.

Scan the tracked set of major companies for open roles matching a keyword and/or location. Keyless
- **get_job_detail**: Use it to read a specific commercial role — the description reveals the segment the company is hiring against, which is personalization fuel for an outreach. If the posting was filled or closed upstream, the result says so instead of erroring.

Full detail for one job posting: departments, offices, deadlines and the description body, trimmed for context. Keyless
- **list_board_jobs**: Use it to size a hiring push (total tells you how many roles are open at once) and to pick the commercial ones to deepen with get_job_detail. If the company has no public board under the slug, the result says so and carries an empty list — that is not the same as a quiet board, so do not report it as zero hiring.

List every public opening on a company job board, with location and how many days ago each was posted. Paged. Keyless
- **list_seed_boards**: It exists so the agent knows exactly which companies find_hiring covers and which slugs are safe to hand to the per-board tools without a probe round-trip. The set is a starting point, not a closed world — any public board works with its own slug.

List the tracked set of major companies with a confirmed public job board


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outbound Hiring Signals** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is Stripe hiring for sales right now? What is the freshest signal?"

**🤖 AI Agent:**
> 🧲 **Hiring signal: stripe — role mix**

31 open commercial roles (14 sales, 9 marketing, 8 GTM/ops) of 128 total openings. 5 roles were published in the last 7 days — the freshest is "Enterprise Account Executive, Payments" (posted 3 days ago, New York, NY).

Want the full page of fresh postings, or the description of that role?

---

**👤 You:**
> "Which of the tracked major companies is hiring a sales engineer in remote?"

**🤖 AI Agent:**
> 🔍 **Hiring scan: "sales engineer" in remote**

2 matches across 21 boards:
- Okta — "Sales Engineer, EMEA" (Remote — Europe, posted 5 days ago)
- HubSpot — "Senior Sales Engineer" (Remote — US, posted 9 days ago)

Both within two weeks — both in a visible GTM build-out. Want the full posting of either?

---

**👤 You:**
> "I want to pitch Figma. Read their newest commercial opening and give me an angle."

**🤖 AI Agent:**
> 📄 **Job detail: figma — "Head of Sales, Enterprise"**

Posted 2 days ago, San Francisco. Departments: Sales. Offices: San Francisco. The description targets closing enterprise design-system deals and mentions team scaling.

Angle: a newly-created head-of-sales seat means the enterprise motion is being staffed from the top down — vendors that shorten ramp time (deal enablement, CRM ops, sales intelligence) land best right now, while the org chart is still open. Lead with the ramp-time pain, not the feature list.


## ❓ FAQ

**Q: Do I need an API key or an account?**
No. The server reads the public job-board endpoint that companies expose on their own slug. There is no credential anywhere in the chain — nothing to issue, rotate or store.

**Q: Why are job listings a sales trigger?**
Open commercial roles are public proof that a company is investing in its motion: hiring sales or marketing means budget, headcount and an expectation of growth. The tools return both the mix (how many sales/GTM/marketing roles are open at once) and the freshness (days since each posting went up), so you can rank targets by buying mood instead of guessing.

**Q: What happens when a company does not publish a board?**
probe_board reports that no public board exists under the slug and says the hiring signal is unavailable for that company — which is a different fact from a quiet board. The scan tools count those boards as skipped, never as zero hiring, and the seed set (21 confirmed major boards) is a starting point: any company that publishes a board can be probed with its own slug.

**Q: How is the public source protected from repeated scans?**
Each board's listing is cached for one hour, so repeating the same scan minutes apart costs nothing upstream. If the source rate-limits a request, the tools report the board as rate-limited and skipped instead of failing the whole call, and the agent is told to retry later.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/outbound-hiring-signals](https://vinkius.com/en/ai-agent-connect/outbound-hiring-signals)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outbound Hiring Signals** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `outbound-hiring-signals` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outbound Hiring Signals** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outbound-hiring-signals": {
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
