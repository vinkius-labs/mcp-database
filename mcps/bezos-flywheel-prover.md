# Bezos Flywheel Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bezos-flywheel-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business](../categories/business.md)

A startup benchmarked against 5 competitors instead of talking to a single customer. It proposed standalone initiatives instead of a flywheel. It built an end-user product instead of infrastructure. It formed a committee instead of a two-pizza team. It optimized for this quarter instead of a 7-year thesis. That is not strategy — that is a project list. This tool forces five Bezos-level axes: customer obsession, flywheel design, infrastructure-first, Day 1 culture, and long-term compounding.

## Description
## The Problem

Every LLM commits five strategic reasoning failures:
1. **Competitor Obsession** — benchmarks rivals instead of working backward from customer pain.
2. **Linear Thinking** — standalone initiatives instead of flywheel loops.
3. **Surface Building** — end-user products instead of infrastructure platforms.
4. **Day 2 Bureaucracy** — committees and approval workflows instead of speed.
5. **Short-Term Focus** — quarterly optimization instead of 7-year compounding.

### The 5 Flywheel Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Customer** | Obsessed | Work backward from pain, not forward from technology. |
| **Flywheel** | Spinning | Each element accelerates every other. |
| **Infrastructure** | Built | Internal infra becomes platform for others. |
| **Day 1** | Maintained | Two-pizza teams, 70% decisions, no committees. |
| **Long-Term** | Committed | 7-year thesis, reinvest all profit. |

### Verdict Matrix

```
Axis 1 fails → COMPETITOR_OBSESSED
Axis 2 fails → LINEAR_THINKING
Axis 3 fails → SURFACE_BUILDING
Axis 4 fails → DAY2_BUREAUCRACY
Axis 5 fails → SHORT_TERM_FOCUS
All pass     → FLYWHEEL_PROVEN
```


## Available Tools (1)
- **validate_bezos_flywheel**: Think like Bezos: (1) CUSTOMER OBSESSION — work backward from the customer pain, not forward from technology. Write the press release first. Name the customer segment, quantify the pain (hours wasted, error rate, cost), and write the one-sentence transformation. "Beat the competition" is not customer obsession — it is competitor obsession, (2) FLYWHEEL DESIGN — each element must accelerate every other element in a virtuous cycle. Lower prices → more customers → more volume → lower costs → lower prices. If it does not loop back to the beginning, it is a project list, not a flywheel. Draw the loop. Identify the entry point. Name the acceleration at each link, (3) INFRASTRUCTURE-FIRST — build internal infrastructure that becomes a platform for others. AWS was Amazon's infrastructure before it was a product. What are you building for yourself that others would pay for? The infrastructure play is the moat, (4) DAY 1 CULTURE — two-pizza teams (max 8 people), decisions at 70% information ("most decisions should be made with around 70% of the information you wish you had"), disagree and commit, six-page memos replace slides, weekly delivery cadence. "Form a committee" is Day 2 — and Day 2 is stasis. Day 2 is followed by irrelevance. Day 2 is followed by decline. Day 2 is followed by death, (5) LONG-TERM COMPOUNDING — state the 7-year thesis. What compounds? "If everything you do needs to work on a 3-year time horizon, then you're competing against a lot of people. But if you're willing to invest on a 7-year time horizon, you're now competing against a fraction of those people." Map years 1-2, 3-4, 5-6, 7+ with milestones. If the tool rejects, the strategy is competitor-focused, linear, or short-term.

Structured reflection tool for Bezos-style business strategy validation. Forces the agent to work backward from customer pain, design self-reinforcing flywheel loops, identify the infrastructure layer that becomes a platform, enforce Day 1 culture practices, and commit to 7-year compounding horizons. Catches Competitor Obsession (benchmarking rivals instead of starting from customer pain), Linear Thinking (standalone initiatives that do not loop — a project list, not a flywheel), Surface Building (end-user products without underlying infrastructure platform play), Day 2 Bureaucracy (committees and consensus instead of two-pizza teams and 70% decisions), and Short-Term Focus (quarterly optimization instead of 7-year compounding thesis). Call once per strategic evaluation, growth plan, or product roadmap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bezos Flywheel Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Beat the competition, launch a standalone project, build an app, form a committee, optimize quarterly results."

**🤖 AI Agent:**
> COMPETITOR_OBSESSED — Five fatal gaps: competitor benchmarking, linear initiatives, surface building, Day 2 bureaucracy, short-term focus.

---

**👤 You:**
> "Customer: SMBs, 4hrs/week manual invoicing, 12% error rate. Flywheel: faster invoicing → more SMBs → more data → better credit scoring → faster payments → supplier referrals → more SMBs. Infrastructure: payment engine offered as a service, 2,400 transactions/day from 12 partners. Day 1: two-pizza teams, 70% decisions, weekly delivery cadence, no committees. Long-term: Year 1-2 infrastructure, Year 3-4 $1M revenue, Year 5-6 platform standard $12M revenue, Year 7 $40M revenue 65% margin."

**🤖 AI Agent:**
> FLYWHEEL_PROVEN — Flywheel strategy validated. All five axes pass. Execute.

---

**👤 You:**
> "We built internal payment processing that handles 2,400 transactions/day from 12 partners. But customer discovery shows SMBs want mobile-first invoicing, not desktop. Do we pivot the infrastructure to mobile?"

**🤖 AI Agent:**
> Partial validation — infrastructure axis passes (platform serves partners). But customer obsession demands the pivot: start from the customer pain, not the infrastructure you already built. Rebuild the press release for mobile SMBs.


## ❓ FAQ

**Q: Why does it reject 'beat the competition'?**
Bezos: 'If you are competitor-focused, you wait until the competitor does something. If you are customer-focused, you are pioneering.' Start from the customer pain. Write the press release first. Work backward to the technology. The customer does not care who you beat — they care about their problem.

**Q: What is DAY2_BUREAUCRACY?**
Day 2 is stasis. Followed by irrelevance. Followed by excruciating, painful decline. Committees, approval workflows, stakeholder alignment, consensus building — all Day 2 signals. Day 1 is: two-pizza teams (max 8), decisions at 70% information, disagree and commit, single-threaded ownership.

**Q: Why 7-year thesis instead of quarterly?**
Bezos: 'If everything you do needs to work on a three-year time horizon, you are competing against a lot of people. If you extend that to 7 years, you are now competing against a fraction of those people.' Amazon reinvested all profit for 20 years. Compounding requires patience.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bezos-flywheel-prover](https://vinkius.com/mcp/bezos-flywheel-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bezos Flywheel Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bezos-flywheel-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bezos Flywheel Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bezos-flywheel-prover": {
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
