# Guerrilla Marketing MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guerrilla-marketing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/guerrilla-marketing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/guerrilla-marketing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Real guerrilla costs nothing — only sweat equity. Most AI-generated tactics quietly sneak in paid spend and call it creative. This tool makes the agent prove zero cost, pinpoint the exact ambush moment, design a sharing trigger, assess risk, and trace every play back to revenue.

## Description
AI agents asked for guerrilla marketing produce the same 5 things every time: "go viral on TikTok", "create shareable content", "leverage social media", "do something creative", "make noise". This is not guerrilla — it's generic advice with a rebellious label. Real guerrilla marketing has three non-negotiable constraints: zero media cost, precision targeting, and built-in amplification.

### The Problem It Solves

AI-generated guerrilla marketing fails on five axes:

- **Budget creep** — "guerrilla" tactics that quietly require $500 in ads. If it costs money, it's paid marketing.
- **Spray-and-pray** — "post everywhere" without knowing WHERE the ICP's attention is unguarded.
- **Dead-on-arrival** — tactics nobody shares. They reach 50 people and die.
- **Reckless execution** — ignoring that guerrilla lives on the edge of ToS, legality, and community norms.
- **Untraceable results** — "generate buzz" with no way to prove it generated a single dollar.

These aren't creativity gaps. They're **discipline gaps.** The agent never asks: is this truly free? Where exactly is the ambush? Why would anyone share this? What could go wrong? How do I prove ROI?

### How It Works

Guerrilla Marketing uses 5 Decision Pivots — boolean checkpoints that force the agent to prove a tactic qualifies as genuine zero-CAC guerrilla before recommending it:

1. **zeroCostVerified** — Is the TOTAL cost literally $0 media spend? Only sweat equity allowed.
2. **ambushPointIdentified** — Have you found the EXACT place and moment where the ICP's attention is unguarded?
3. **viralMechanismDesigned** — Is there a built-in reason to SHARE, not just consume?
4. **riskAssessed** — Have you identified legal, reputational, and platform risks?
5. **attributionPathDefined** — Can you trace from the guerrilla hit to a revenue event?

The tool validates logical consistency. If the agent says `GUERRILLA_APPROVED` but `zeroCostVerified: false`, the tool rejects. If the viral trigger is "go viral" instead of a designed mechanism, it rejects. If the risk profile says "no risk", it rejects.

### Why It Works

- **Tool calls are obligations, instructions are suggestions.** The agent can ignore "make sure it's free" in a prompt. It cannot ignore a schema that demands proving zero cost, naming the ambush point, and designing the sharing trigger.
- **The commit pattern.** The agent proposes its own verdict, then the server validates it against the pivots. This forced commitment surfaces contradictions the agent would otherwise gloss over.
- **Semantic traps.** The engine catches 4 categories of anti-patterns: budget language in "zero cost" plans, vague channels as ambush points, wishful thinking as viral mechanisms, and dismissive risk assessments.
- **13 consistency rules.** Not just pivot-verdict matching — field quality validation and semantic analysis that catch lazy reasoning at every level.


## Available Tools
- **validate_guerrilla_tactic**: You must: (1) confirm ZERO media spend — only sweat equity (time + creativity). "Low cost" fails. "$50 on promoted posts" fails. $0 on creation + distribution, (2) identify the EXACT ambush point — where and when is the ICP's attention unguarded? Not "social media" — the specific subreddit, HN comment thread, Slack channel, or conference hallway. Guerrilla is a sniper, not a shotgun, (3) design the viral MECHANISM — not "go viral" but WHY Person A shares with Person B. Name the psychological trigger: social currency, emotion, utility, controversy, identity, (4) assess RISKS honestly — legal (trademark, defamation), reputational (backlash), platform (ToS violation, account ban). Every guerrilla tactic has risk. "No risk" = rejection, (5) define ATTRIBUTION — trace the guerrilla hit to a revenue event. UTM links, dedicated landing pages, referral codes, survey fields. If rejected, the tactic has a fatal flaw.

Structured reflection tool for guerrilla marketing with zero CAC — forces validation that a tactic is truly $0 media cost, precisely ambush-targeted, inherently shareable, risk-aware, and traceable to revenue. Based on Levinson (1984), Hutter & Hoffmann (2011), and modern zero-CAC growth. Catches Budget Bloat ("low-cost" is not guerrilla — guerrilla is ZERO media spend. Only sweat equity: time and creativity. The moment you spend $1 on promotion, it is paid marketing with a guerrilla costume. $50 on Reddit ads = paid. $0 on a Reddit teardown post = guerrilla), Spray-and-Pray (posting on "social media" without precision targeting — guerrilla is an AMBUSH, not a broadcast. You need the exact subreddit, HN thread type, Slack community, or conference hallway where the ICP's attention is unguarded. "Social media" is a continent, not a coordinate), Dead-on-Arrival (no viral mechanism — "it will go viral" is not a strategy. WHY does Person A share this with Person B? Social currency (looks smart sharing it), emotion (outrage/delight/surprise), practical value (genuinely useful), controversy (forces response), or identity signal (aligns with self-image). Without a designed trigger, content dies silently), Reckless Execution (ignoring legal, reputational, and platform risks — every guerrilla tactic has risk. Competitor name-drops can trigger trademark claims. Platform ToS violations get accounts banned. "No risk" means you have not thought about it), and Untraceable Results (no attribution path from guerrilla hit to revenue — "we got exposure" is not a business outcome. Unique UTM links, dedicated landing pages, referral codes, "how did you hear about us" fields — without attribution, you cannot tell if the tactic worked). Call once per guerrilla marketing tactic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guerrilla Marketing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to grow my SaaS by creating viral content on social media. Validate this guerrilla tactic."

**🤖 AI Agent:**
> Verdict: SPRAY_AND_PRAY. 'Social media' is not an ambush point — it's a continent. Where EXACTLY is your ICP's attention unguarded? Which subreddit, which Slack community, which HN thread type? Guerrilla is a sniper shot, not carpet bombing. Name the exact place and moment.

---

**👤 You:**
> "My ICP is 'DevOps engineers at Series A startups who monitor r/devops and HN daily, frustrated with $200/month observability bills.' I'll write a detailed teardown of a competitor's pricing page, post it on r/devops the day they announce a price increase, with a UTM-tagged link to our free tier. The sharing trigger is outrage at price gouging. Risk: could be seen as competitor bashing — mitigated by keeping the tone factual and data-driven."

**🤖 AI Agent:**
> Verdict: GUERRILLA_APPROVED. Zero cost (writing is sweat equity). Ambush point is precise (r/devops, timed to competitor's price increase announcement). Viral mechanism is designed (outrage at price gouging = high share trigger in DevOps community). Risk identified and mitigated (factual tone prevents bashing perception). Attribution path defined (UTM-tagged link to free tier). CAC = $0. Execute.

---

**👤 You:**
> "I want to boost our brand awareness by doing a creative stunt at a tech conference. We'd hire actors to wear branded t-shirts and hand out stickers in the hallway. Validate as guerrilla."

**🤖 AI Agent:**
> Verdict: BUDGET_BLOAT. Multiple failures. (1) Hiring actors is paid spend — not guerrilla. (2) 'Boost brand awareness' is a vanity outcome with no attribution path to revenue. (3) Handing out stickers is the oldest conference play in history — zero shareability, zero surprise factor. Strip the budget: do it yourself, in your own t-shirt, with a controversial sign that people photograph and share because it says something nobody else will say.


## Installation & Usage

To install and use the **Guerrilla Marketing** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guerrilla-marketing](https://vinkius.com/mcp/guerrilla-marketing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
