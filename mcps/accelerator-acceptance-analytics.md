# Accelerator Acceptance Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-acceptance-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate acceptance probabilities and cohort composition for accelerator programs.

## Description
This MCP server provides a specialized analytics engine for accelerator program managers. It calculates the probability of application acceptance by factoring in capacity constraints, quality distributions, and strategic referral weighting. Use `get_acceptance_metrics` to determine overall acceptance rates and effective capacity, `analyze_competitive_positioning` to evaluate how specific quality tiers perform against the pool, and `evaluate_diversity_alignment` to ensure the cohort meets specific demographic or sector-based representation goals.


## Available Tools (3)
- **analyze_competitive_positioning**: Determines how a specific applicant's tier affects their chance of success
- **evaluate_diversity_alignment**: Assesses whether the current applicant pool and capacity allow for meeting specific cohort diversity targets
- **get_acceptance_metrics**: Calculates the primary acceptance statistics and the impact of referral weighting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Acceptance Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected acceptance rate for 100 applications with 10 spots available and 20% referrals?"

**🤖 AI Agent:**
> The expected acceptance rate is 8.5% with an effective capacity adjustment for referrals.

---

**👤 You:**
> "How likely is a 'High-Priority' applicant to be accepted if there are 50 applicants and 5 spots?"

**🤖 AI Agent:**
> An applicant in the High-Priority tier has a 75% probability of acceptance given the current distribution.

---

**👤 You:**
> "Will we meet our 20% female founder target with the current pool?"

**🤖 AI Agent:**
> The current alignment score is 0.85, indicating a high probability of meeting the target, with a gap of only 2% remaining.


## ❓ FAQ

**Q: How does the referral multiplier affect acceptance?**
The referral multiplier increases the priority of referred applicants, which effectively reduces the remaining spots available for non-referred applicants when using `get_acceptance_metrics`.

**Q: Can I check if my cohort will meet diversity targets?**
Yes, you can use the `evaluate_diversity_alignment` tool to assess if the current applicant pool and available spots allow for meeting your specific diversity goals.

**Q: How is competitive positioning calculated?**
Competitive positioning is determined via `analyze_competitive_positioning`, which calculates a score based on the availability of spots relative to the volume of applicants in higher-ranked tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-acceptance-analytics](https://vinkius.com/ai-agent-connect/accelerator-acceptance-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Acceptance Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-acceptance-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Acceptance Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-acceptance-analytics": {
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
