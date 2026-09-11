# Waterflood Pattern Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/waterflood-pattern-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimize waterflood pattern design and predict oil recovery.

## Description
This MCP connects AI agents to advanced reservoir engineering calculations. It allows for the evaluation of waterflood patterns by calculating total sweep efficiency using `get_pattern_efficiency`, determining optimal injection rates with `calculate_optimal_injection_rate`, and estimating oil recovery via `predict_recovery_volume`. Users can also use `optimize_pattern_design` to compare different geometric arrangements like 5-spot or 9-spot patterns to maximize recovery based on reservoir characteristics.


## Available Tools (4)
- **calculate_optimal_injection_rate**: Determines the recommended water injection rate to maintain pressure
- **get_pattern_efficiency**: Calculates the total sweep efficiency for a specific pattern configuration
- **optimize_pattern_design**: Compares multiple pattern types to find the one that maximizes recovery
- **predict_recovery_volume**: Estimates the total volume of oil that can be recovered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Waterflood Pattern Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total sweep efficiency for a 5-spot pattern with 0.7 areal sweep and 0.6 vertical sweep?"

**🤖 AI Agent:**
> The total sweep efficiency for the 5-spot pattern is 0.42.

---

**👤 You:**
> "Estimate the oil recovery for 1,000,000 barrels of initial oil with a 0.5 total sweep and 0.8 displacement efficiency."

**🤖 AI Agent:**
> The expected recovery is 400,000 barrels, resulting in a recovery factor of 0.4.

---

**👤 You:**
> "Calculate the optimal injection rate for a reservoir with 500,000 volume, 150 permeability, 2000 current pressure, and 2500 target pressure."

**🤖 AI Agent:**
> The optimal injection rate is 125.5 units, with a pressure delta of 500.


## ❓ FAQ

**Q: How do I find the best pattern for my reservoir?**
You can use the `optimize_pattern_design` tool to compare multiple pattern types against your specific reservoir characteristics and well spacing.

**Q: Can I calculate expected oil recovery?**
Yes, the `predict_recovery_volume` tool estimates the total volume of oil that can be recovered based on initial oil in place and sweep efficiencies.

**Q: What is the purpose of the injection rate tool?**
The `calculate_optimal_injection_rate` tool determines the recommended water injection rate to maintain reservoir pressure effectively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/waterflood-pattern-optimizer](https://vinkius.com/en/ai-agent-connect/waterflood-pattern-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Waterflood Pattern Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `waterflood-pattern-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Waterflood Pattern Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "waterflood-pattern-optimizer": {
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
