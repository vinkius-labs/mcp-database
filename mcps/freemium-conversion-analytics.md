# Freemium Conversion Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/freemium-conversion-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Quantify user transitions from free tiers to paid subscriptions using a multi-stage funnel model.

## Description
This MCP server provides a specialized analytics engine to measure the health of your freemium funnel. It allows AI agents to calculate conversion rates, identify upgrade triggers, and evaluate funnel leakage. By using tools like `calculate_conversion_metrics` and `identify_upgrade_triggers`, agents can diagnose why users are hitting usage thresholds or being blocked by feature gating. It also enables forecasting future growth through `project_future_conversion` based on current trends.


## Available Tools (4)
- **analyze_funnel_efficiency**: Evaluates the "leakage" in the funnel to find where users are dropping off
- **calculate_conversion_metrics**: Provides a high-level overview of the current conversion health across the entire funnel
- **identify_upgrade_triggers**: Diagnoses why users are (or are not) converting by looking at usage patterns
- **project_future_conversion**: Estimates future paid user growth based on current conversion trends and user growth


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freemium Conversion Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current conversion health for the last 30 days? We have 1000 free users, 200 paid users, 150 trial users, and a 20% trial conversion rate."

**🤖 AI Agent:**
> The current free-to-paid conversion rate is 20%, with a trial success rate of 20% and a daily conversion velocity of 6.67 new paid users per day.

---

**👤 You:**
> "Analyze our funnel efficiency. We started with 5000 free users, 500 moved to trial, and 100 became paid subscribers."

**🤖 AI Agent:**
> The free-to-trial rate is 10%, the trial-to-paid rate is 20%, and the total funnel yield is 2%.

---

**👤 You:**
> "Predict our paid users for next month. We have 500 paid users, 2000 free users, a 5% historical conversion rate, and we expect 500 new free users."

**🤖 AI Agent:**
> The estimated number of paid users is 525, with 25 expected new conversions.


## ❓ FAQ

**Q: How does the tool identify why users aren't upgrading?**
The `identify_upgrade_triggers` tool analyzes usage levels and feature access attempts to determine if users are hitting limits or experiencing friction from gated features.

**Q: Can I forecast my subscriber growth?**
Yes, the `project_future_conversion` tool estimates future paid user growth by applying historical conversion rates to projected free user growth.

**Q: What metrics are included in the conversion summary?**
The `calculate_conversion_metrics` tool provides the free-to-paid rate, trial success rate, and the daily conversion velocity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/freemium-conversion-analytics](https://vinkius.com/en/ai-agent-connect/freemium-conversion-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freemium Conversion Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freemium-conversion-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freemium Conversion Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freemium-conversion-analytics": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
