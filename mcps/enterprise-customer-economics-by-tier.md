# Enterprise Customer Economics by Tier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-customer-economics-by-tier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze unit economics, LTV:CAC ratios, and tier prioritization for enterprise segments.

## Description
This MCP server provides analytical tools to evaluate the profitability of different customer segments. Use `calculate_tier_economics` to determine LTV:CAC ratios and payback periods, or `get_tier_prioritization` to rank segments for strategic resource allocation. You can also use `simulate_expansion_impact` to predict how changes in expansion rates affect long-term value, or `compare_tiers_efficiency` for side-by-side capital efficiency comparisons.


## Available Tools (4)
- **calculate_tier_economics**: Calculates core unit economic metrics for a specific set of customer tiers
- **compare_tiers_efficiency**: Provides a side-by-side comparison of two specific tiers to determine which is more capital-efficient
- **get_tier_prioritization**: Ranks customer tiers to identify which segments offer the best return on investment
- **simulate_expansion_impact**: Predicts how changes in the expansion rate of a specific tier will affect its overall LTV:CAC ratio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Customer Economics by Tier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the unit economics for SMB, Mid-Market, and Enterprise tiers with the following data: SMB (CAC: 500, LTV: 2000, Retention: 0.8, Expansion: 0.05), Mid-Market (CAC: 5000, LTV: 25000, Retention: 0.9, Expansion: 0.1), Enterprise (CAC: 50000, LTV: 300000, Retention: 0.95, Expansion: 0.15)."

**🤖 AI Agent:**
> The SMB tier has an LTV:CAC of 4.0 with a 3-month payback. Mid-Market shows an LTV:CAC of 5.0 with a 4-month payback. Enterprise leads with an LTV:CAC of 6.0 and a 5-month payback.

---

**👤 You:**
> "Which tier is more efficient: SMB or Mid-Market, given SMB has CAC 500/LTV 2000 and Mid-Market has CAC 5000/LTV 25000?"

**🤖 AI Agent:**
> Mid-Market is the winner with an LTV:CAC ratio of 5.0, compared to SMB's ratio of 4.0.

---

**👤 You:**
> "What happens to the Enterprise tier LTV:CAC if the expansion rate increases from 0.15 to 0.20?"

**🤖 AI Agent:**
> Increasing the expansion rate to 0.20 for the Enterprise tier results in a projected LTV:CAC of 7.2, representing a 20% increase from the original ratio.


## ❓ FAQ

**Q: How do I calculate the health of my customer segments?**
You can use the `calculate_tier_economics` tool. It evaluates the LTV:CAC ratio and returns a qualitative health score like 'Excellent' or 'Critical'.

**Q: Can I predict the impact of upsells on my unit economics?**
Yes, the `simulate_expansion_impact` tool allows you to test how a specific target expansion rate changes the projected LTV:CAC ratio for a tier.

**Q: How can I decide which customer tier to prioritize for marketing?**
Use the `get_tier_prioritization` tool. It ranks tiers based on a composite of LTV:CAC and payback period to identify the most efficient segments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-customer-economics-by-tier](https://vinkius.com/ai-agent-connect/enterprise-customer-economics-by-tier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Customer Economics by Tier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-customer-economics-by-tier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Customer Economics by Tier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-customer-economics-by-tier": {
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
