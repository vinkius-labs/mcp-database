# Wine Appellation Brand Value MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-appellation-brand-value)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify the economic value and brand strength of wine appellations using hedonic regression.

## Description
This MCP server provides tools to calculate the economic impact of wine appellations. By applying hedonic regression principles, it isolates the price premium attributable to a specific region's reputation. Use `get_appellation_metrics` to retrieve baseline data like recognition scores and quality perception. Determine market power with `calculate_brand_strength`, or quantify the exact monetary value added per bottle using `calculate_appellation_value_contribution`. For nested regions, `analyze_appellation_hierarchy` reveals how sub-appellations capture prestige from their parent zones.


## Available Tools (4)
- **analyze_appellation_hierarchy**: Explores the relationship between a sub-appellation and its parent
- **calculate_appellation_value_contribution**: Quantifies the specific economic value added by the appellation
- **calculate_brand_strength**: Determines the market power of an appellation
- **get_appellation_metrics**: Retrieves the core baseline data for a specific appellation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Appellation Brand Value** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the brand strength of the Napa Valley appellation?"

**🤖 AI Agent:**
> The Brand Strength Index for Napa Valley is 0.92, placing it in the Tier 1 market tier.

---

**👤 You:**
> "How much value does the Bordeaux appellation add to a bottle of wine?"

**🤖 AI Agent:**
> The value contribution per bottle for the Bordeaux appellation is $15.50 USD.

---

**👤 You:**
> "Show me the hierarchy details for the Margaux sub-appellation."

**🤖 AI Agent:**
> Margaux is a sub-appellation of the Bordeaux parent region with a relative prestige score of 0.85.


## ❓ FAQ

**Q: How is the brand strength calculated?**
The Brand Strength Index is derived from the product of the appellation's recognition score and its quality perception score.

**Q: Can I account for sub-appellation prestige?**
Yes, by using `calculate_appellation_value_contribution` with the `includeHierarchyAdjustment` parameter enabled, the tool factors in the parent appellation's prestige.

**Q: What data is required to start?**
You only need a valid `appellationId` to begin retrieving metrics or performing calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-appellation-brand-value](https://vinkius.com/en/ai-agent-connect/wine-appellation-brand-value)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Appellation Brand Value** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-appellation-brand-value` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Appellation Brand Value** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-appellation-brand-value": {
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
