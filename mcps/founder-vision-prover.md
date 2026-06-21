# Founder Vision Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/founder-vision-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business & strategy](../categories/business-strategy.md)

A pitch deck said '1% of a $10B market' and 'run Facebook ads.' That is not a startup — that is a PowerPoint. This tool forces it to prove behavioral pain, calculate bottom-up TAM, show cohort retention, build a $0 CAC moat, and model unit economics that recycle capital in under 12 months.

## Description
## The Problem

Ask an LLM to evaluate a startup idea. It will say: "This addresses a large and growing market. Consider running Facebook ads to acquire initial users." That is not strategy — that is flattery followed by a cash incinerator.

Every LLM commits five startup reasoning failures:
1. **Behavioral Void** — it describes pain no one is hacking a solution for today.
2. **Top-Down Delusion** — it cites "$10B market" instead of calculating N × Price.
3. **Retention Blindness** — it skips cohort retention and margin physics entirely.
4. **Distribution Naivety** — it defaults to "run ads" as the growth plan.
5. **Zombie Economics** — it ignores CAC payback and never models when revenue crosses burn.

## How It Works

The Founder Vision Prover forces the LLM to fill 5 reflection fields and commit to 5 Decision Pivots before concluding any startup idea is viable.

### The 5 Decision Pivots

| Pivot | Question |
|---|---|
| **Behavioral Pain Proven** | Is there PRESENT-TENSE evidence the customer is hacking a solution TODAY? |
| **Market Sized Bottom-Up** | Is TAM calculated as [N customers] × [Price] — no Gartner? |
| **Retention Proven** | Is M3 cohort retention above threshold AND gross margin above 80%? |
| **Distribution Owned** | Is there a STRUCTURAL $0 CAC loop — not paid ads? |
| **Unit Economics Viable** | Is CAC payback <12 months AND crossover month defined? |

### The Verdict Matrix

```
Pivot 1 fails → BEHAVIORAL_VOID
Pivot 2 fails → TOP_DOWN_DELUSION
Pivot 3 fails → RETENTION_DEATH
Pivot 4 fails → DISTRIBUTION_NAIVE
Pivot 5 fails → ZOMBIE_ECONOMICS
All pass      → VISION_PROVEN
```

## Why It Works

Tool calls are obligations — instructions are suggestions. The LLM cannot skip a field. It must describe the customer hack, show the multiplication, prove retention with cohort data, name the structural distribution loop, and model the payback timeline. Every rejection names the exact startup physics violation.


## Available Tools (1)
- **validate_founder_vision**: Think like a ruthless YC partner — the one who has seen 10,000 pitches and knows that 95% fail on the same 5 axes. You must: (1) describe the CUSTOMER HACK — what the customer does TODAY to survive the pain. Present tense only. WHO does WHAT with WHAT tool for HOW MUCH? If no hack exists, they do not care enough to pay, (2) calculate BOTTOM-UP TAM — [N reachable customers] × [Annual Contract Value]. No Gartner, no Forrester, no "1% of $10B." Show the multiplication. If TAM is <$100M, it needs a wedge-and-expand story, (3) prove RETENTION — Month 3 cohort retention with specific numbers. >30% consumer, >80% SaaS. Gross margin >80% for software. Downloads and signups are vanity — retention is truth, (4) describe the DISTRIBUTION MOAT — how each user brings the next at $0 CAC. Network effects, virality, product-led growth, UGC SEO. "Facebook Ads" is a tax that scales linearly — it is rejected, (5) model UNIT ECONOMICS — CAC payback <12 months, crossover month (revenue > burn). If payback >12 months, capital cycles too slowly for venture scale. If rejected, your startup physics are fatally flawed.

Structured reflection tool that forces YC-partner-level scrutiny on startup ideas — validating behavioral evidence, bottom-up market sizing, retention physics, distribution moats, and unit economics before concluding viability. Catches Behavioral Void (no present-tense customer hack — "they are frustrated" is a feeling, not evidence. "Restaurant managers pay an intern $1K/month to manually update a Google Sheet every night because no tool integrates POS, inventory, and labor scheduling" — THAT is behavioral evidence. If nobody is hacking a workaround today, the pain is not severe enough to pay for), Top-Down TAM Delusion ("the market is $10B per Gartner, if we capture 1%..." — top-down TAM is a fantasy that makes every startup look viable. Bottom-up: 15,000 mid-market restaurants × $2,400/year = $36M TAM. That is real, reachable, and small enough to force honest strategy), Retention Death (leaky bucket — signups, downloads, and waitlist size are vanity metrics. Month 3 cohort retention is truth. <30% consumer or <80% SaaS = the product does not retain. Growth cannot outrun churn forever), Distribution Naivety (Facebook Ads is a tax, not a moat — paid acquisition scales linearly with spend. A distribution MOAT is structural: network effects, virality, product-led growth, UGC SEO. How does each user bring the next user at $0 CAC?), and Zombie Economics (CAC payback >12 months means capital cycles too slowly for venture scale — if it takes 18 months to recover customer acquisition cost, the startup needs 3x more capital to reach the same milestone as a competitor with 6-month payback). Call once per startup idea or business model evaluation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Founder Vision Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to build a better CRM. The global CRM market is $50B according to Gartner. If we capture just 1% we'll be a unicorn. We'll acquire users via Google Ads and hire a sales team."

**🤖 AI Agent:**
> TOP_DOWN_DELUSION + DISTRIBUTION_NAIVE — "Gartner says $50B" is top-down nonsense. Count the ACTUAL reachable customers and multiply by your price. And "Google Ads + sales team" is a double tax — both scale linearly with spend and decay with competition. Define a structural $0 CAC loop or accept you're building a lifestyle business.

---

**👤 You:**
> "Restaurant managers pay an intern $1k/month to update inventory in a Google Sheet every night. We charge $200/month. 15,000 mid-market restaurants in the US × $2,400/year = $36M TAM. Month 3 retention: 85%. Gross margin: 92%. Each restaurant invites their suppliers to the platform (network effect), driving CAC to $0. CAC: $300, payback: 1.5 months. Crossover: month 14."

**🤖 AI Agent:**
> VISION_PROVEN — Founder Vision Validated. Behavioral pain: intern hack exists ($1k/month waste). Bottom-up TAM: 15,000 × $2,400 = $36M. Retention: 85% M3 (above 80% SaaS threshold). Margin: 92%. Distribution: supplier network effect drives CAC toward $0. Unit economics: 1.5-month payback, crossover at month 14. Execute.

---

**👤 You:**
> "Users are annoyed that they have to use two different apps to book flights and hotels. We will build an all-in-one travel app. We have 50,000 downloads and a waitlist of 10,000 people."

**🤖 AI Agent:**
> BEHAVIORAL_VOID — "Annoyed" is not a venture-scale pain. Customers are NOT hacking a solution — they are not paying interns or duct-taping spreadsheets to combine flight and hotel bookings. This is a vitamin, not a painkiller. And 50,000 downloads and a waitlist are vanity metrics — they prove interest, not retention. Show Month 3 cohort data.


## ❓ FAQ

**Q: Does it predict if my startup will succeed?**
No. It validates STARTUP PHYSICS — the structural mechanics that make venture-scale growth possible. If your cohort retention leaks, your CAC payback is too slow, or your distribution is paid ads, no amount of vision will save the business. This tool stops the AI from flattering your bad ideas.

**Q: Why does it reject 'downloads' and 'signups' as proof of retention?**
Downloads, signups, and waitlist size are vanity metrics. They measure interest, not retention. The only metric that proves retention is COHORT data: of users who joined in Month 1, what percentage are STILL ACTIVE in Month 3? If you cannot answer that, you have a leaky bucket.

**Q: What is a 'Behavioral Hack'?**
If a problem is truly painful, the customer is already solving it TODAY using a hack — spreadsheets, interns, duct tape, custom scripts. They are spending money or time on an absurd workaround. If they are NOT hacking a solution, the pain is not real enough to justify a purchase.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/founder-vision-prover](https://vinkius.com/mcp/founder-vision-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Founder Vision Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `founder-vision-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Founder Vision Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "founder-vision-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
