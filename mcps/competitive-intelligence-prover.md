# Competitive Intelligence Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/competitive-intelligence-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI agents fabricate competitor data, list vague weaknesses, propose fantasy strategies, and ignore your own gaps. This tool forces fact-grounded competitive analysis: verifiable sources, measurable weaknesses, feasible attack plans, self-aware assessment, and kill criteria with deadlines.

## Description
AI agents analyzing competitors produce the most dangerous type of output: confident-sounding fiction. They fabricate market share numbers, invent revenue figures, list vague weaknesses like "poor UX" without evidence, propose strategies requiring resources you don't have, and ignore your own vulnerabilities entirely.

### The Problem

AI competitive analysis fails on six axes:

- **Hallucinated data** — "They have approximately $50M in revenue" — from WHERE? SEC filing? Crunchbase? Or did the AI make it up?
- **Vague weaknesses** — "They have poor UX" is an opinion, not intelligence. Intelligence: "14-step onboarding, 23-min setup (we tested), G2 review #12345 confirms."
- **Fantasy strategies** — "Build an enterprise platform" when you have 3 engineers.
- **Missing evidence** — Claims without verifiable sources. If you can't cite it, you can't claim it.
- **Self-deception** — Analyzing their weaknesses while ignoring your own.
- **Generic playbooks** — "Better product, better marketing" applies to ANY company.

### How It Works

6 Decision Pivots force reality-grounded competitive strategy:

1. **evidenceBased** — Every claim cites verifiable source?
2. **weaknessesSpecific** — Weaknesses are observable, cited, quantified, verified?
3. **strategyFeasible** — WHO executes, TIMELINE, COST, DEPENDENCIES defined?
4. **selfAware** — Your weaknesses acknowledged? Their strengths recognized?
5. **differentiated** — Exploits a SPECIFIC gap only YOU can attack?
6. **metricsAttached** — Leading/lagging indicators + kill criteria with deadlines?


## Available Tools
- **validate_competitive_intel**: You must: (1) EVIDENCE: every claim about a competitor cites a VERIFIABLE source — their website, G2/Capterra reviews (with IDs), GitHub issues, Reddit threads, Crunchbase, your own testing. ZERO "approximately", "reportedly", "sources suggest", fabricated numbers. (2) SPECIFIC WEAKNESSES: measurable, observable, cited. "Bad UX" is opinion. "14-step onboarding, 23-min setup, G2 review #12345 confirms" is intelligence. (3) FEASIBLE STRATEGY: executable with current resources. Define WHO, TIMELINE, COST, DEPENDENCIES. (4) SELF-AWARE: acknowledge YOUR weaknesses and THEIR strengths. How would THEY attack you? (5) DIFFERENTIATED: exploit a SPECIFIC competitive gap only YOU can attack. (6) METRICS: leading indicators, lagging indicators, kill criteria with deadlines.

Validates competitive intelligence analysis for fact-grounded, anti-hallucination strategic planning. Forces every competitor claim to cite a VERIFIABLE source (pricing pages, G2 reviews, Crunchbase, your own testing). Eliminates vague weaknesses, fantasy strategies, self-deception, and generic playbooks. Ensures attack strategies are feasible with current resources (WHO/WHEN/COST) and include measurable success metrics with kill criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Competitive Intelligence Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Competitor X has approximately $50M in revenue and about 30% market share. They have poor UX and limited features. We should build a better product and outspend them on marketing to win the market."

**🤖 AI Agent:**
> Verdict: EVIDENCE_MISSING. Triple failure. (1) '$50M revenue' and '30% market share' — WHERE? No SEC filing, no Crunchbase link, no source. Likely fabricated. (2) 'Poor UX' and 'limited features' — vague opinions, not intelligence. Test their product and document specifics. (3) 'Build better and outspend' — generic playbook, no WHO/WHEN/COST. Rewrite with verifiable sources, measured weaknesses, and execution plan.

---

**👤 You:**
> "Competitor: Acme CI/CD. Evidence: pricing page shows $49/user/month (verified 2024-01-20). G2 reviews #14523, #14601, #14789: 'slow builds', 'no ARM support', 'expensive for small teams'. Our testing (2024-01-18): build time 12min vs our 3min for identical repo. GitHub issues: 234 open about ARM (#4521, #4589). Job postings: 0 DevRel, 3 enterprise sales. Weakness: no ARM (verified), 4x slower builds (tested), no free tier (pricing). Attack: 'Migrate from Acme' page targeting 'acme..."

**🤖 AI Agent:**
> Verdict: STRATEGY_PROVEN. Evidence-based (pricing verified, G2 with IDs, hands-on testing with dates, GitHub issues cited). Weaknesses quantified (no ARM — 234 issues, 4x slower — tested, no free tier — pricing). Strategy feasible (1 engineer, 5 days, $0). Self-aware (SOC2/SAML gap). Differentiated ('acme alternative ARM' keyword). Metrics with kill criterion. Execute.

---

**👤 You:**
> "Competitor Y's onboarding has issues (we heard from users). They're expensive. We should target their unhappy customers with a better price and better experience."

**🤖 AI Agent:**
> Verdict: VAGUE_WEAKNESS. Three gaps: (1) 'Has issues' and 'expensive' — WHAT issues? HOW expensive vs you? No G2 reviews, no testing, no pricing comparison. (2) 'We heard from users' is not evidence. Cite specific Reddit threads, G2 reviews with IDs, or your own testing with dates. (3) 'Better price and better experience' is a generic playbook — this applies to any competitor. Define: WHAT specific onboarding problem? HOW MANY steps vs yours? WHAT exact price comparison? HOW do yo...


## ❓ FAQ

**Q: How does it prevent hallucination?**
The engine detects 16+ hallucination markers: 'approximately', 'reportedly', 'sources suggest', 'believed to', 'likely has', 'probably', etc. Any hedging language triggers rejection. Every claim must cite a verifiable source: their website, G2/Capterra reviews with IDs, Crunchbase, SEC filings, Reddit threads, or your own hands-on testing. If you can't cite the source, you must delete the claim.

**Q: What sources are acceptable?**
Seven categories: (1) Their website — pricing pages, feature docs, changelogs. (2) Review platforms — G2, Capterra, TrustRadius with specific review IDs. (3) Public financials — Crunchbase funding, SEC filings, press releases. (4) User complaints — Reddit threads, GitHub issues, support forums. (5) Job postings — reveals tech stack, team gaps, growth areas. (6) Your own testing — 'We signed up and tested on [date].' (7) App Store/Play Store reviews. Minimum 3 independent sources to triangulate.

**Q: Why does it require self-assessment?**
Because competitors also analyze YOU. An analysis that only shows 'they're bad, we're good' is self-deception that leads to strategic blindness. The tool forces you to acknowledge: (1) Where are YOU vulnerable? (2) What do THEY do better? (3) How would THEY attack your weak points? (4) What blind spots exist? The best competitive strategies are brutally honest about both sides.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/competitive-intelligence-prover](https://vinkius.com/mcp/competitive-intelligence-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Competitive Intelligence Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `competitive-intelligence-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Competitive Intelligence Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "competitive-intelligence-prover": {
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
