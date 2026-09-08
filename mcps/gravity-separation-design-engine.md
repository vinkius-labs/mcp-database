# Gravity Separation Design Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gravity-separation-design-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Select optimal gravity separation equipment and estimate recovery performance.

## Description
This MCP server provides specialized tools for mineral processing design. It allows AI agents to calculate the concentration criterion, select the most suitable equipment such as `select_equipment`, predict recovery efficiency using `estimate_recovery`, and evaluate if a mineral stream is viable via `analyze_feed_feasibility`. It also provides process optimization suggestions through `optimize_circuit_parameters` to improve recovery or manage throughput.


## Available Tools (4)
- **estimate_recovery**: Predicts the efficiency of the separation process for a chosen piece of equipment
- **analyze_feed_feasibility**: Evaluates if a specific mineral stream is even capable of being separated via gravity methods
- **optimize_circuit_parameters**: Suggests adjustments to the process to improve recovery or throughput
- **select_equipment**: Determines the most suitable type of gravity separation equipment for a specific mineral feed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gravity Separation Design Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What equipment should I use for a mineral with density 4.5, gangue density 2.7, particle size 50-150 microns, and throughput of 50?"

**🤖 AI Agent:**
> The most suitable equipment for these parameters is spirals.

---

**👤 You:**
> "Is it feasible to separate a mineral with density 3.0 and gangue density 2.6 in water?"

**🤖 AI Agent:**
> The concentration criterion is 1.4, which indicates that separation is possible but may be difficult.

---

**👤 You:**
> "Predict the recovery for spirals with mineral density 4.0, gangue density 2.5, and average particle size of 80 microns."

**🤖 AI Agent:**
> The estimated recovery is 75% with a grade estimate of 0.85.


## ❓ FAQ

**Q: How do I know which equipment to use?**
You can use the `select_equipment` tool by providing the mineral density, gangue density, particle size range, and throughput to find the best fit.

**Q: Can I check if my mineral separation is possible?**
Yes, the `analyze_feed_feasibility` tool evaluates the concentration criterion to determine if gravity separation is feasible for your specific mineral stream.

**Q: How can I improve my recovery rates?**
The `optimize_circuit_parameters` tool provides specific suggested actions to improve recovery or manage throughput constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gravity-separation-design-engine](https://vinkius.com/ai-agent-connect/gravity-separation-design-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gravity Separation Design Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gravity-separation-design-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gravity Separation Design Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gravity-separation-design-engine": {
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
