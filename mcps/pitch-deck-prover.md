# Pitch Deck Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pitch-deck-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pitch-deck-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pitch-deck-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

An AI built a pitch deck that claimed a '$4.2B TAM' with no source, described the problem as 'everyone struggles with this,' showed '15K downloads' as traction with 3% D30 retention, and asked for 'funding to accelerate growth' — no amount, no use of funds, no milestones. The deck got rejected in 8 minutes. This tool forces problem validation with evidence, sourced market sizing, defined unit economics, retention-based traction, and a specific fundraising ask.

## Description
AI agents build pitch decks that look professional — and get rejected in the first meeting. They invent TAM numbers from thin air. They describe problems nobody validated with actual users. They skip unit economics entirely. They show vanity metrics as traction. They ask for money without specifying what it buys.

### The Problem

LLMs commit five pitch deck failures that VCs catch in minutes:

- **Unvalidated Problem** — 'Everyone has this problem' without a single user interview, survey, or quantified pain point. The problem slide is a belief statement, not evidence. 42% of startups fail because of no market need — and the deck did nothing to prove one exists.
- **Fictional Market** — '$4.2B TAM' pulled from a Google search with no methodology. No SAM filtering. No SOM grounding. 'We only need 1% of the market' — the most dangerous sentence in fundraising.
- **Undefined Model** — 'We will figure out monetization later.' No pricing tiers. No CAC. No LTV. No margin structure. The business model slide says 'freemium' with no conversion rate assumption.
- **Vanity Traction** — '15K downloads' with 3% D30 retention. 'Strong interest from potential customers.' 'Growing waitlist.' None of these are traction — traction is revenue, retained active users, or contractual commitments.
- **Vague Ask** — 'Seeking $2-5M to accelerate growth.' No specific amount. No use of funds breakdown. No milestones this capital unlocks. No runway calculation. The investor has no basis for evaluation.

### How It Works

Pitch Deck Prover validates fundraising narratives through 5 Decision Pivots:

1. **problemValidated** — Evidence the problem exists at scale. User interviews with count, surveys with sample size, quantified existing spend on workarounds. Not 'we believe.'
2. **marketSized** — TAM/SAM/SOM with sourced data and named methodology (top-down from industry reports or bottom-up from customer count × ACV). Not 'billion dollar opportunity.'
3. **modelDefined** — Revenue mechanic, specific pricing tiers, unit economics (CAC, LTV, LTV/CAC ratio, payback period), and gross margin. Not 'we will monetize later.'
4. **tractionDemonstrated** — MRR/ARR if available, active users with retention cohorts, week-over-week growth rate, engagement frequency. Not downloads or waitlist signups.
5. **askSpecified** — Exact amount, use of funds percentage breakdown, milestones unlocked, runway months, and terms. Not 'seeking funding to scale.'

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| problemValidated = false | PROBLEM_UNVALIDATED | No evidence the problem exists. Building for a belief. |
| marketSized = false | MARKET_FICTIONAL | TAM without sources. Aspirational arithmetic. |
| modelDefined = false | MODEL_UNDEFINED | No pricing, no unit economics. Hope is not a model. |
| tractionDemonstrated = false | TRACTION_ABSENT | Vanity metrics only. Downloads are not traction. |
| askSpecified = false | ASK_VAGUE | No amount, no milestones, no runway. Unevaluable. |
| All pivots pass | PITCH_PROVEN | Validated, sized, modeled, demonstrated, specified. |

### Why It Works

- **Tool calls are obligations.** The agent cannot skip market sizing or claim traction without stating retention rates. Filling the fields IS the fundraising preparation.
- **Consistency engine catches contradictions.** If the agent claims `tractionDemonstrated=true` but lists only waitlist signups, the engine rejects with a specific coaching message.
- **Semantic traps detect hand-waving.** Phrases like 'we only need 1%,' 'growing fast,' or 'seeking funding to scale' trigger automatic rejection. Name the number. Name the source. Name the milestone.


## Available Tools
- **validate_pitch_deck**: You must: (1) PROBLEM — cite specific evidence: user interviews (count, key quotes where THEY raise the pain), quantified existing spend on workarounds, frequency of pain occurrence. "We believe" is not evidence. "23 of 30 interviewees spend $200+/month on workarounds" IS evidence, (2) MARKET — TAM/SAM/SOM with named sources, year, and methodology. Bottom-up preferred (customer count × ACV). Top-down acceptable if sourced (Gartner, IDC, Statista), (3) MODEL — revenue mechanic, specific pricing, and unit economics: CAC by channel, LTV adjusted for gross margin, LTV/CAC ≥ 3x, payback ≤ 12 months, gross margin ≥ 65%, (4) TRACTION — retention-based metrics: MRR/ARR, NRR, paid conversion, cohort retention. Downloads, signups, and waitlist are NOT traction, (5) ASK — exact amount, allocation by category (%), milestones with measurable targets, runway in months, and the metric milestone that unlocks next round. If rejected, the deck has an investor-visible weakness. Fix before presenting.

Structured reflection tool for pitch deck validation — forces evidence-backed problem validation, rigorous market sizing with named sources, unit economics verification, traction beyond vanity metrics, and specific fundraising asks with milestone-linked runway before any investor-facing deck ships. Catches Problem Fabrication (building a solution for a problem the founder experiences but the market does not — "We built an AI that auto-categorizes Slack messages." Founder's evidence: "I have 47 channels and can never find anything." Reality check: 23 customer discovery interviews revealed 0 people who would pay for this. Why? Heavy Slack users already use channels-as-categories. Light users have 5-8 channels. The "problem" exists for the founder but not at market scale. Evidence required: 30+ user interviews where the INTERVIEWEE raises the pain unprompted (The Mom Test: never ask "would you use this?" — ask "walk me through the last time this happened"), quantified existing spend on workarounds ($X/month on Notion/bookmarks/manual search), and frequency data (how often does the pain occur? Daily = urgent. Monthly = nice-to-have)), Market Fantasy (claiming a TAM without sourcing or methodology — "The global communication tools market is $45B." This number is real (Gartner 2024). But it includes: enterprise telephony ($12B), video conferencing ($8B), unified communications ($15B), and team messaging ($4B). A Slack message categorizer competes in team messaging productivity ($4B). Of that, the segment who would adopt a third-party Slack add-on (not built by Salesforce) in companies with 50-500 employees is approximately $120M (SAM). Achievable in 18 months with current go-to-market: $2M (SOM). "$45B market" vs. "$2M obtainable in 18 months" — investors fund the latter), Unit Economics Absent (showing revenue without proving the business can be profitable — "We have $50K MRR!" Investors ask: CAC? "$1,200 blended." LTV? "$3,600 at 24-month median lifetime." LTV/CAC ratio: 3.0x. Sounds healthy. But: gross margin is 35% (heavy infrastructure costs — GPU compute for AI features). LTV adjusted for gross margin: $3,600 × 0.35 = $1,260. Adjusted LTV/CAC: 1.05x. The business DESTROYS value with every customer acquired. Gross margin below 60% for SaaS is a structural problem — not a growth problem. Raising money accelerates losses, not profits), Vanity Traction (presenting engagement metrics that do not predict revenue — "100,000 downloads! 50,000 signups! 10,000 DAU!" Investors ask: "What percentage converts to paid?" "2%." "What is Day-30 retention?" "8%." 100,000 downloads × 2% conversion × 8% retention = 160 retained paying users. At $10/month: $1,600 MRR. That is the real traction — not 100,000 downloads. Traction metrics that matter: MRR/ARR, net revenue retention (NRR > 100% = expansion revenue), paid conversion rate, cohort retention (Day 1, 7, 30), and payback period. Downloads, signups, waitlist size, and "strong interest" are vanity metrics — they measure curiosity, not commitment), and Vague Ask (requesting capital without specifying allocation, milestones, or runway — "We are raising $2M to scale." Scale what? How? Over what period? Investor-grade ask: "$2M Seed. 18-month runway at $111K/month burn rate. Allocation: 55% engineering (3 senior hires + infrastructure), 25% sales (1 AE + SDR + CRM tooling), 15% marketing (content + paid acquisition at target CAC $800), 5% operations (legal, accounting, office). Milestones: Month 6 — product-market fit signal (NPS > 40, Day-30 retention > 25%). Month 12 — $30K MRR. Month 18 — $80K MRR, position for Series A at 3x revenue multiple = $2.88M ARR." Every dollar has a job. Every milestone is measurable. Every month is accounted for). Call once per pitch deck creation or review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pitch Deck Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We are building an AI-powered project management tool. The market is huge — everyone needs better project management. We have 15,000 downloads and growing fast. We are seeking funding to accelerate growth."

**🤖 AI Agent:**
> PROBLEM_UNVALIDATED — 'Everyone needs better project management' is a belief, not evidence. How many user interviews? What specific pain do they describe? What do they spend today on workarounds? Also: '15K downloads' with no retention data is vanity. 'Seeking funding' with no amount is unevaluable. This deck fails on all 5 axes.

---

**👤 You:**
> "Problem: 47 user interviews with mid-market engineering managers — 89% report spending 6+ hours/week on status updates (survey N=312). Current workaround: $180/user/year on Jira + Confluence + manual reports. Market: TAM $18.7B (Gartner 2025 PM software), SAM $4.1B (mid-market SaaS, 50-500 employees, English-speaking), SOM $82M (2,100 target companies × $39K ACV, 12-month sales cycle). Model: SaaS, $149/user/month Team, $299/user/month Enterprise. CAC $2,400 (LinkedIn + SDR), LTV $21,400 (36-month avg tenure, $149 × 12 × 3), LTV/CAC 8.9x, payback 4.8 months, 78% gross margin. Traction: $48K MRR, 14 paying customers, 92% D30 retention, 18% MoM growth over 6 months, avg 4.2 daily active sessions per user. Ask: $2.4M seed, 60% engineering (8 hires), 25% sales (3 SDRs + 1 AE), 15% marketing (content + events). Milestones: $200K MRR in 12 months, 80 customers, Series A readiness. Runway: 18 months at current burn. Terms: 15% equity at $16M post-money."

**🤖 AI Agent:**
> PITCH_PROVEN — Investor-grade pitch validated. Problem: 47 interviews + N=312 survey, quantified pain ($180/user/year workaround). Market: Gartner-sourced TAM, SAM filtered by segment, SOM grounded in 2,100 targets × $39K ACV. Model: clear tiers, LTV/CAC 8.9x, 4.8-month payback, 78% margin. Traction: $48K MRR, 92% retention, 18% MoM sustained. Ask: $2.4M with 60/25/15 allocation, 18-month runway, $200K MRR milestone. This deck survives the first meeting.

---

**👤 You:**
> "Problem validated: 30 interviews with HR managers, 76% spend 4+ hours/week on compliance tracking (survey N=200, $120/user/year on spreadsheets). Market: TAM $12B (Deloitte 2025 HR tech), SAM $2.8B (US mid-market), SOM $56M. Model: $99/user/month, CAC $1,800, LTV $14,200, LTV/CAC 7.9x, 72% margin. Traction: 2,400 waitlist signups, 3 pilot conversations, strong interest from Fortune 500 companies. Ask: $1.5M pre-seed for product development."

**🤖 AI Agent:**
> TRACTION_ABSENT — Problem, market, and model pass. But traction fails. 'Waitlist signups' and 'pilot conversations' are not traction — they are awareness. 'Strong interest from Fortune 500' without a signed LOI or paid pilot is anecdotal. Show: paid pilots (even at discount), LOIs with company names, or validated waitlist with deposits. Also: ask needs use of funds breakdown, milestones, and runway — '$1.5M for product development' is too vague.


## Installation & Usage

To install and use the **Pitch Deck Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pitch-deck-prover](https://vinkius.com/mcp/pitch-deck-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
