# Wine Closure Selection Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-closure-selection-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Optimizes wine closure selection by balancing oxygen ingress, aging goals, and cost.

## Description
This MCP server provides specialized decision-support tools for winemakers and enologists to select the ideal bottle closure. By analyzing oxygen transmission rates (OTR), target aging durations, and economic constraints, the tool helps prevent premature oxidation or reductive aromas. Use `get_closure_recommendation` to find the best match for a specific wine style, `calculate_otr_compatibility` to verify oxygen levels, `estimate_bottle_variation` to predict quality divergence, and `analyze_closure_economics` to ensure cost-effectiveness relative to retail price.


## Available Tools (4)
- **analyze_closure_economics**: Compares the cost of various closure options against the wine's price point
- **calculate_otr_compatibility**: Evaluates if a specific closure's oxygen transmission rate aligns with the wine's aging needs
- **estimate_bottle_variation**: Predicts the likelihood of quality divergence across a batch of bottles
- **get_closure_recommendation**: Provides the single best closure recommendation based on all user constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Closure Selection Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best closure for a Bold Red wine intended to age for 10 years with a budget of $0.50 per unit?"

**🤖 AI Agent:**
> The recommended closure is Technical Cork, which provides the necessary oxygen ingress for tannin management over a decade while remaining within your budget.

---

**👤 You:**
> "Is a screw cap compatible with a Light White wine that needs minimal oxygen for 2 years of storage?"

**🤖 AI Agent:**
> Yes, a screw cap is highly compatible as it provides the minimal oxygen ingress required for short-term storage of delicate white wines.

---

**👤 You:**
> "Will a $25 bottle of wine be economically viable if the closure costs $5?"

**🤖 AI Agent:**
> No, a $5 closure for a $25 bottle represents 20% of the retail price, which is flagged as low economic feasibility.


## ❓ FAQ

**Q: How does the tool recommend a closure?**
The tool uses `get_closure_recommendation` to evaluate wine style, intended aging years, oxygen needs, and budget to provide a single optimal recommendation.

**Q: Can I check if a specific closure is suitable for my wine?**
Yes, you can use `calculate_otr_compatibility` to determine if a closure's oxygen transmission rate aligns with your wine's aging requirements.

**Q: How is bottle variation calculated?**
You can use `estimate_bottle_variation` to predict the likelihood of quality divergence across a batch based on the closure type and aging duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-closure-selection-tool](https://vinkius.com/ai-agent-connect/wine-closure-selection-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Closure Selection Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-closure-selection-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Closure Selection Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-closure-selection-tool": {
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
