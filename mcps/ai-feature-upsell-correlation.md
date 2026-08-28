# AI Feature Upsell Correlation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ai-feature-upsell-correlation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Quantify the impact of AI features on subscription upgrades.

## Description
This MCP server provides tools to measure how AI feature adoption drives revenue growth in SaaS models. It calculates the upgrade probability lift, attributes revenue to AI usage, and identifies specific user behaviors that trigger upgrade suggestions. Use `calculate_upsell_lift` to find the relative increase in upgrades, `calculate_revenue_attribution` to determine the dollar value of AI-driven growth, and `identify_upgrade_triggers` to detect users ready for a tier upgrade based on their interaction with gated features.


## Available Tools (4)
- **analyze_tier_impact**: Evaluate how different subscription tiers influence the effectiveness of AI features
- **calculate_revenue_attribution**: Translate the abstract lift into actual dollar amounts to justify AI investment
- **calculate_upsell_lift**: Calculate the percentage increase in upgrade probability attributed to AI feature usage
- **identify_upgrade_triggers**: Pinpoint specific conditions that suggest a user is ready to upgrade


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI Feature Upsell Correlation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the upgrade lift if the AI user upgrade rate is 15% and the non-AI user rate is 5%?"

**🤖 AI Agent:**
> The upgrade lift is 200%.

---

**👤 You:**
> "Calculate the revenue attribution for 1000 users with a 20% lift and an average upgrade value of $50."

**🤖 AI Agent:**
> $10,000

---

**👤 You:**
> "Is a user with a usage frequency of 50 on a 'Basic' tier ready to upgrade if 'Pro' features are gated?"

**🤖 AI Agent:**
> Yes, the user is a candidate for an upgrade due to high frequency usage of gated features.


## ❓ FAQ

**Q: How is the upsell lift calculated?**
The `calculate_upsell_lift` tool compares the upgrade rate of users who use AI features against the baseline rate of users who do not.

**Q: Can I identify users ready to upgrade?**
Yes, by using `identify_upgrade_triggers`, you can detect when a user's interaction frequency with gated features suggests they are ready for a higher tier.

**Q: How does this help with revenue forecasting?**
The `calculate_revenue_attribution` tool translates the observed lift into specific dollar amounts, helping you justify AI development costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ai-feature-upsell-correlation](https://vinkius.com/ai-agent-connect/ai-feature-upsell-correlation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI Feature Upsell Correlation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-feature-upsell-correlation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI Feature Upsell Correlation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-feature-upsell-correlation": {
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
