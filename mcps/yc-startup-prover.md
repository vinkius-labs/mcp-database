# YC Startup Prover MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yc-startup-prover)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/yc-startup-prover-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/yc-startup-prover-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business](../categories/business.md)

Most startups die building solutions nobody asked for. A founder pitched for 20 minutes about their proprietary algorithm — never mentioned a single user, a single pain point, a single dollar of willingness to pay. That pitch would be rejected in 30 seconds at Y Combinator. This tool forces five PG-level axes: problem discovery, unscalable beginnings, metric discipline, user obsession, and core value focus.

## Description
## The Problem

Every LLM commits five startup reasoning failures:
1. **Solution Seeking** — building technology before finding a real problem.
2. **Premature Scaling** — hiring and spending before product-market fit.
3. **Vanity Metrics** — tracking signups instead of retention and revenue.
4. **Ivory Tower** — market research instead of user conversations.
5. **Feature Bloat** — adding features instead of finding the one 10x value.

### The 5 YC Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Problem** | Found | 5 users with the pain, willingness to pay confirmed. |
| **Unscalable** | Doing | Manual, personal, high-touch — like Airbnb photographing listings. |
| **Metrics** | Real | Retention, revenue, default alive status. |
| **Users** | Talking | Weekly conversations that change the roadmap. |
| **Core Value** | Clear | ONE thing done 10x better. |

### Verdict Matrix

```
Axis 1 fails → SOLUTION_SEEKING
Axis 2 fails → PREMATURE_SCALING
Axis 3 fails → VANITY_METRICS
Axis 4 fails → IVORY_TOWER
Axis 5 fails → FEATURE_BLOAT
All pass     → STARTUP_PROVEN
```


## Available Tools
- **validate_yc_startup**: (1) PROBLEM FIRST — not technology, not solution, not market size. A specific, painful problem experienced by specific, nameable people who are currently paying time or money to solve it badly. (2) DO THINGS THAT DON'T SCALE — manual, personal, high-touch actions for early users. Personally deliver. Personally onboard. Personally support. Learn from every interaction. You cannot learn at scale what you refuse to learn manually. (3) REAL METRICS — weekly retention (do they come back?), MRR (do they pay?), default alive/dead (at current growth rate, do you reach profitability before running out of money?). Not signups, not page views, not followers. (4) TALK TO USERS — every week. Not surveys — conversations. What surprised you? What did they say that you did not want to hear? What changed because of it? (5) ONE THING — what does your product do 10× better than the alternative? One sentence. If you need two sentences: you are not focused enough.

Structured reflection tool that forces the LLM to think like Paul Graham — Y Combinator co-founder, essayist, and the voice behind "Do Things That Don't Scale" (2013). YC has funded 5,000+ companies with $1T+ in combined valuation (Airbnb, Stripe, Dropbox, Coinbase). The YC method is counterintuitive: start with a problem, not a solution. Do manual, unscalable things for your first users. Measure retention, not signups. Talk to users every week. Focus on one thing done 10× better, not 10 things done adequately. Catches Solution Seeking (building technology before validating a problem — a potter builds an automated glaze-mixing machine. 6 months of engineering. $15,000 in materials. It mixes 47 glaze recipes perfectly. Shows it to 20 potters: "How do you currently mix glazes?" "By hand. It takes 5 minutes. It is part of the craft. I enjoy it." "Would you pay $3,000 for a machine that does it?" "No. Mixing is not my bottleneck. Kiln firing schedules and clay procurement are." The potter built a solution for a problem that does not exist. PG: "The best startup ideas come from problems you personally experience — not solutions you find technically interesting." Rule: name 5 specific people who HAVE this problem, describe their CURRENT solution, and quantify their willingness to pay. Not "people would want this" — "Maria pays $X monthly for Y"), Premature Scaling (hiring, marketing, and expanding before finding product-market fit — a cheese maker creates artisanal goat cheese. 4 flavors. Sells at one farmers' market. Week 3: "We should be in 20 stores!" Hires a sales rep ($4,500/month). Rents commercial kitchen ($2,800/month). Orders branded packaging ($3,200 minimum run). Revenue: $1,200/month. Burn: $10,500/month. Runway: 4 months. The cheese maker has not validated: which flavor sells best, what price point works, whether store customers buy differently than farmers' market customers, or whether the cheese survives 5-day shelf distribution. PG: "Do things that don't scale." The cheese maker should: personally deliver cheese to 3 stores. Stand behind the counter. Watch who buys. Ask why. Learn that the herb flavor outsells plain 4:1. That $8 price point is too high for grocery but perfect for specialty. That customers want 150g portions, not 250g. THEN scale — with validated knowledge), Vanity Metrics (celebrating activity instead of measuring value — a tutoring service: "We have 2,000 followers on Instagram! 450 people downloaded our free study guide! 120 signed up for the newsletter!" Revenue: $0. Paying students: 0. Followers are not customers. Downloads are not revenue. Signups are not retention. The ONLY metrics that matter for a tutoring service: How many students are paying? $[MRR]. How many students come back for a second session? [retention %]. How many students improve their grades? [outcome metric]. PG: "Startups die from vanity. They celebrate signups instead of measuring retention. A startup with 100 users who love you is better than one with 10,000 who signed up and never returned." Rule: weekly retention curve, monthly recurring revenue, default alive or dead calculation), Ivory Tower (building without talking to users — a woodworker designs a modular shelving system. Beautiful CAD drawings. Patent filed. Website built. Launch video produced. 8 months of work. Zero user conversations. Launch day: 14 orders. 9 returns within 30 days. Return reasons: "Too heavy to wall-mount alone" (2 people needed — they live alone). "Modules do not fit standard wall stud spacing" (16 inches, not 18). "No cable management for electronics" (the #1 use case was media shelving). If the woodworker had TALKED to 20 potential buyers before building: "I live alone — can I install this myself?" "My wall studs are 16 inches apart." "I need somewhere to hide cables." These three conversations would have changed the entire design. PG: "Make something people want" — and you discover what they want by ASKING THEM. Rule: how many user conversations THIS WEEK? What surprised you? What changed because of it?), and Feature Bloat (building 20 features instead of being exceptional at one — a food truck: serves burgers, tacos, sushi, pizza, pad thai, acai bowls, and crepes. Menu: 47 items. Kitchen: one person. Wait time: 25 minutes. Quality: mediocre — everything is "okay," nothing is "amazing." Customer review: "Jack of all trades, master of none. The burger was fine. But the truck down the street does ONE thing — smash burgers — and they are incredible." The smash burger truck has 1 menu item with 3 toppings. Wait: 4 minutes. Revenue per hour: 3× the 47-item truck. Because ONE thing done 10× better beats 47 things done adequately. PG: "Do one thing well." Rule: what is the ONE thing your product does 10× better than the alternative? If you cannot answer in one sentence: you are doing too many things). Call once per startup strategy, business plan, or market validation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **YC Startup Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our proprietary algorithm uses deep learning. We plan to hire a sales team. We have 50K signups. Market research shows a billion dollar TAM. We have 12 features planned."

**🤖 AI Agent:**
> SOLUTION_SEEKING — Five fatal gaps: technology-first, premature scaling, vanity metrics, ivory tower, feature bloat.

---

**👤 You:**
> "Problem: SMBs spend 4hrs/week on invoicing (5 users confirmed, $29/month willingness). Unscalable: personally onboarding each user via Zoom, migrating their Excel data. Metrics: 68% weekly retention, $2,400 MRR, default alive in 3 months. Users: 12 conversations this week, discovered mobile need, changed roadmap. Core: '5-minute invoice app' — NPS 72."

**🤖 AI Agent:**
> STARTUP_PROVEN — Startup strategy validated. All five axes pass. Ship it.

---

**👤 You:**
> "Problem validated with 8 users. Doing unscalable onboarding (Zoom calls). But our metrics show 5,200 signups, 180K page views, and 12K app downloads. We have 4 features live and 8 more on the roadmap."

**🤖 AI Agent:**
> Two axes pass (problem, unscalable). Three fail. VANITY METRICS: signups, page views, downloads are vanity. What is weekly RETENTION? Revenue? Default alive? FEATURE BLOAT: 4 live + 8 planned = 12 features. What is the ONE thing? Strip to the core 10x value.


## Installation & Usage

To install and use the **YC Startup Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yc-startup-prover](https://vinkius.com/mcp/yc-startup-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
