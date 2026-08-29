# Catalyst Performance Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/catalyst-performance-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculates TOF, TON, selectivity, and deactivation rates for heterogeneous catalysis.

## Description
This MCP server provides specialized kinetic calculation tools for evaluating heterogeneous catalyst performance. It allows AI agents to quantify catalytic efficiency by calculating Turnover Frequency (TOF) and Turnover Number (TON) using `get_activity_metrics`. It also determines product yield efficiency via `get_selectivity_profile`, quantifies performance decay with `get_deactivation_analysis`, and identifies physical transport constraints using `evaluate_mass_transfer_impact`.


## Available Tools (4)
- **evaluate_mass_transfer_impact**: Determines if the observed reaction rate is being hindered by physical transport limitations
- **get_activity_metrics**: Calculates the fundamental efficiency metrics (TOF and TON) of the catalyst
- **get_deactivation_analysis**: Quantifies the loss of catalyst performance over the course of operation
- **get_selectivity_profile**: Determines how effectively the catalyst produces the target molecule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Catalyst Performance Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the activity metrics for a reaction with a rate of 0.5 mol/s, 100 active sites, and 10 seconds elapsed."

**🤖 AI Agent:**
> The turnover frequency (TOF) is 0.005 mol/(site·s) and the turnover number (TON) is 0.05 mol/site.

---

**👤 You:**
> "What is the selectivity if 80g of target product is formed out of 100g of total products?"

**🤖 AI Agent:**
> The selectivity is 0.8 (or 80%).

---

**👤 You:**
> "The initial rate was 1.0 and the current rate is 0.8 after 5 minutes. What is the deactivation rate?"

**🤖 AI Agent:**
> The deactivation rate is 0.04 per minute.


## ❓ FAQ

**Q: How do I calculate the turnover frequency?**
You can use the `get_activity_metrics` tool by providing the reaction rate, the number of active sites, and the time elapsed.

**Q: Can this tool detect mass transfer limitations?**
Yes, the `evaluate_mass_transfer_impact` tool determines if the observed reaction rate is being hindered by physical transport limitations.

**Q: How is catalyst deactivation measured?**
Deactivation is quantified using `get_deactivation_analysis`, which compares the initial rate to the current rate over a specific time interval.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/catalyst-performance-evaluator](https://vinkius.com/ai-agent-connect/catalyst-performance-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Catalyst Performance Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `catalyst-performance-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Catalyst Performance Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "catalyst-performance-evaluator": {
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
