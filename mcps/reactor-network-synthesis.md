# Reactor Network Synthesis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/reactor-network-synthesis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Optimizes reactor configurations, volumes, and sequences to maximize selectivity and economic yield.

## Description
This MCP server provides a specialized optimization engine for chemical engineering. It allows AI agents to determine the most efficient arrangement of reactor types, such as CSTR and PFR, to maximize product selectivity and economic yield. By using `find_optimal_network`, agents can identify the best sequence of reactors for complex reaction networks, including consecutive and autocatalytic reactions. The server also includes `analyze_reaction_dynamics` to simulate behavior in specific environments, `calculate_economic_impact` to quantify financial viability, and `compare_configurations` to rank different reactor setups based on selectivity, conversion, or economy.


## Available Tools (4)
- **compare_configurations**: Ranks multiple different reactor arrangements against each other based on user-defined priorities
- **analyze_reaction_dynamics**: Evaluates how specific reaction types will behave under different reactor environments
- **calculate_economic_impact**: Quantifies the financial viability of a proposed reactor arrangement
- **find_optimal_network**: Identifies the best reactor configuration to meet specific selectivity and conversion goals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reactor Network Synthesis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best reactor configuration for a reaction network with a target selectivity of 0.85 and conversion of 0.90."

**🤖 AI Agent:**
> The optimal arrangement is a PFR followed by a CSTR, with a total volume of 450L, achieving 0.87 selectivity and 0.92 conversion.

---

**👤 You:**
> "What is the economic impact of a 500L CSTR arrangement with a product value of 50 and feed cost of 10?"

**🤖 AI Agent:**
> The proposed arrangement yields a net profit of 1250 with a profit margin of 25%.

---

**👤 You:**
> "Simulate the reaction dynamics for a consecutive reaction in a PFR."

**🤖 AI Agent:**
> The simulation shows a selectivity profile that peaks at 0.75 before declining as the secondary reaction consumes the desired product.


## ❓ FAQ

**Q: What kind of reactor arrangements can be optimized?**
The engine optimizes combinations and sequences of CSTR (Continuous Stirred-Tank Reactor) and PFR (Plug Flow Reactor) units to meet specific selectivity and conversion targets.

**Q: How does the tool handle autocatalytic reactions?**
When using `find_optimal_network`, the engine favors configurations that maintain high product concentrations early in the process to support the autocatalytic nature of the reaction.

**Q: Can I compare the economic viability of different setups?**
Yes, you can use `calculate_economic_impact` to find the net profit and costs for a specific arrangement, or `compare_configurations` to rank multiple setups based on economy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/reactor-network-synthesis](https://vinkius.com/ai-agent-connect/reactor-network-synthesis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reactor Network Synthesis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reactor-network-synthesis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reactor Network Synthesis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reactor-network-synthesis": {
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
