# Growth Strategist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/growth-strategist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

AI agents asked for strategy always recommend the same five things: social media, engaging content, brand awareness. None of it is strategy — it's autocomplete. Growth Strategist demands specifics: name the person, prove channel fit, take a unique position, cite evidence, tie the outcome to revenue.

## Description
AI agents generating marketing strategy produce the same 5 things every time: "leverage social media", "create engaging content", "build brand awareness", "use SEO and paid ads", "partner with influencers". This is audience-blind, channel-mismatched, undifferentiated, unvalidated, vanity-driven noise. It's not strategy — it's autocomplete.

### The Problem It Solves

AI-generated marketing fails on five axes:

- **Audience blindness** — "target social media users" without naming who
- **Channel mismatch** — recommending TikTok for B2B enterprise
- **Generic advice** — "leverage content marketing" with no unique position
- **No evidence** — claims without data, case studies, or precedents
- **Vanity metrics** — optimizing impressions instead of revenue

These aren't knowledge gaps. They're **reasoning gaps.** The agent never asks: who exactly is this for? Does this channel actually reach them? What can I say that no competitor can?

### How It Works

Growth Strategist uses 5 Decision Pivots — boolean checkpoints that force the agent to reason through a strategic validation process before outputting any recommendation:

1. **icpNamed** — Can you name the EXACT person? Job title, pain point, where they spend time.
2. **channelFitValidated** — Evidence (not assumption) that this channel reaches the ICP.
3. **differentiationCommitted** — A unique position that NO competitor can truthfully claim.
4. **evidenceCited** — A data point, case study, or precedent supporting this tactic.
5. **outcomeMeasurable** — Expected result tied to a business metric, not a vanity metric.

The tool validates logical consistency. If the agent says `STRATEGY_PROVEN` but `icpNamed: false`, the tool rejects with a clear explanation. If the differentiator is a feature list instead of a position, it rejects. If the expected outcome mentions "brand awareness" or "impressions", it rejects.

### Why It Works

- **Tool calls are obligations, instructions are suggestions.** The agent can ignore "think about the audience" in a prompt. It cannot ignore a schema that requires naming the audience, explaining channel fit, and committing to a verdict.
- **The commit pattern.** The agent proposes its own verdict, then the server validates it against the pivots. This forced commitment deepens the reasoning — the agent must actively decide if its strategy is sound.
- **Semantic traps.** The engine catches domain-specific anti-patterns: generic ICP terms ("everyone", "businesses"), feature-list differentiators ("we offer", "best in class"), and vanity metric language ("impressions", "followers", "brand awareness").


## Available Tools (1)
- **validate_growth_tactic**: Generic, audience-blind, evidence-free growth advice is the most common failure mode in marketing — every startup gets told to "do content marketing" without specifics. You must: (1) name the EXACT person — not "marketers" but a specific title, company stage, pain point, and where they seek solutions. The sharper the ICP, the sharper the tactic, (2) prove CHANNEL FIT with evidence — not "LinkedIn works for B2B." Show search volume, community size, engagement data, or comparable company attribution, (3) commit to a DIFFERENTIATED position that no competitor can truthfully claim — differentiation excludes. If your positioning does not say NO to someone, it says nothing, (4) cite EVIDENCE — a data point, case study, benchmark, or precedent. Not "studies show" — name the study. Not "it works" — show where it worked and the numbers, (5) define a measurable BUSINESS outcome — revenue, CAC, LTV, activation rate, conversion. Not vanity: impressions, likes, followers, "awareness." If rejected, your growth strategy has a blind spot.

Structured reflection tool for growth strategy — forces ICP identification, channel-fit validation with evidence, differentiated positioning, data-backed evidence, and measurable business outcomes. Catches Audience Blindness (targeting "marketers" or "developers" instead of a named person — "Head of Growth at Series A SaaS with <$1M ARR, spending 60% of time in HN/Twitter/ProductHunt, frustrated with $400 CAC from Google Ads, needs to prove channel efficiency to board by Q3" is an ICP. "Marketers" is everyone and nobody. The sharper the ICP, the sharper the tactic), Channel Mismatch (assuming a channel reaches your ICP without evidence — "LinkedIn works for B2B" is a platitude. "Our ICP searches 'SaaS metrics dashboard' 8,100 times/month per Ahrefs, and the top 3 results are 2019 blog posts with no product mention" is channel evidence. Channel fit requires proof the ICP is there AND receptive), Generic Strategy (positioning that any competitor can also claim — "we are faster and easier" is what everyone says. Differentiation EXCLUDES — "we only serve single-operator restaurants, not chains" is a position. If your competitor can truthfully copy your positioning, it is not positioning), Unvalidated Recommendation (citing no evidence — "content marketing works for SaaS" is folklore. "Lemlist grew from 0→$10M ARR via cold email teardowns on YouTube — 47 videos, 3.2M views, 12% of signups from YT attribution" is evidence. Based on ICP validation frameworks and Growth Hacking research: Ziakis 2023, Khosrawi-Rad 2022), and Vanity-Driven Outcome (measuring impressions and followers instead of revenue — "10K impressions" is a number, not a business outcome. "12% of attributed signups from this channel convert to paid within 30 days at $35 CAC vs $400 Google Ads baseline" IS a business outcome). Call once per growth tactic recommendation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Growth Strategist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to grow my developer tool by posting on LinkedIn. Validate this growth tactic."

**🤖 AI Agent:**
> Verdict: AUDIENCE_BLIND. 'Developer tool' is not an ICP. Who exactly? Solo developers? CTOs at Series A startups? DevOps engineers at Fortune 500? Each has different pain points, spends time in different places, and responds to different messaging. Name the exact person first.

---

**👤 You:**
> "My ICP is 'Head of AI at mid-market SaaS companies with 50-200 engineers struggling with agent reliability.' I want to publish a benchmark on Hacker News showing our tools catch 40% more reasoning errors. Validate."

**🤖 AI Agent:**
> Verdict: STRATEGY_PROVEN. ICP is specific (role + company stage + pain point). Channel fits (HN is where technical decision-makers evaluate tools). Differentiator is measurable ('40% more errors caught' — verifiable, not a claim). Evidence is the benchmark itself. Outcome is measurable (benchmark engagement → trial signups → activation). Execute.

---

**👤 You:**
> "I want to 'increase brand awareness through thought leadership content on social media.' Validate this tactic."

**🤖 AI Agent:**
> Verdict: VANITY_DRIVEN. Multiple failures detected. (1) 'Brand awareness' is a vanity metric — tie the outcome to revenue, CAC reduction, or conversion rate. (2) 'Social media' is not a channel — which platform, and why does your ICP spend time there? (3) 'Thought leadership' is not a differentiator — every competitor claims thought leadership. Take a position that excludes.


## ❓ FAQ

**Q: Does Growth Strategist generate marketing strategies?**
No. Growth Strategist performs zero content generation. It forces the AI agent to structure its own strategic reasoning into verifiable fields, then validates that the reasoning is logically consistent. The agent does all the thinking — the tool catches contradictions, generic advice, and vanity metrics.

**Q: What does it catch that a prompt instruction doesn't?**
Prompt instructions are suggestions — agents routinely ignore 'be specific about the audience' or 'cite evidence.' Tool calls are obligations — the agent must fill every field. Beyond that, Growth Strategist has 10 consistency rules that catch domain-specific anti-patterns: generic ICP terms ('everyone', 'businesses'), feature-list differentiators ('we offer', 'best in class'), and vanity metric language ('impressions', 'followers'). A prompt can't enforce these — a tool schema can.

**Q: Can I use this for non-marketing strategy?**
The 5 Decision Pivots are applicable to any domain where recommendations tend to be generic: business strategy, product strategy, sales tactics, partnership proposals. However, the semantic traps (vanity metric blocklist, feature-list differentiator detection) are calibrated for marketing. For other domains, consider building a specialized Reasoning MCP using the same Decision Pivot pattern.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/growth-strategist](https://vinkius.com/mcp/growth-strategist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Growth Strategist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `growth-strategist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Growth Strategist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "growth-strategist": {
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
