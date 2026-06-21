# Competitive Intelligence Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/competitive-intelligence-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/competitive-intelligence-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/competitive-intelligence-prover-mcp)
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


## Installation & Usage

To install and use the **Competitive Intelligence Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/competitive-intelligence-prover](https://vinkius.com/mcp/competitive-intelligence-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
