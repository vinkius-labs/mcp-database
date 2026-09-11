# Leaching Circuit Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/leaching-circuit-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design metal extraction leaching circuits by modeling kinetics and equipment requirements.

## Description
This MCP server provides specialized engineering tools for designing metal extraction leaching circuits. It allows users to evaluate ore feasibility using `analyze_ore_feasibility`, calculate physical tank requirements with `calculate_tank_requirements`, estimate chemical reagent needs via `estimate_reagent_needs`, and design heap leach operations using `design_heap_leach`. It bridges the gap between ore mineralogy and practical circuit configuration for gold and copper extraction.


## Available Tools (1)
- **analyze_ore_feasibility**: Determines if a specific ore mineralogy and metal content can realistically meet a given recovery target


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Leaching Circuit Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it feasible to achieve 85% recovery from an ore with gold-bearing pyrite mineralogy and 5g/t gold content?"

**🤖 AI Agent:**
> The target is feasible. The estimated kinetics show a rate constant of 0.15 and a reaction order of 1.2.

---

**👤 You:**
> "Calculate the tank volume needed for a CIP circuit with a feed rate of 500 tonnes/hour, 10 hours retention time, and 40% slurry density."

**🤖 AI Agent:**
> The total volume required is 1250 cubic meters, which would be distributed across 2 tanks of 625 cubic meters each.

---

**👤 You:**
> "How much cyanide is needed for 10,000 tonnes of ore with gold-bearing mineralogy?"

**🤖 AI Agent:**
> The required reagent is cyanide, with a total mass of 5000 kg needed for the batch.


## ❓ FAQ

**Q: What types of leaching configurations are supported?**
The server supports calculations for both Carbon-in-Pulp (CIP) and Carbon-in-Leach (CIL) agitated tank circuits, as well as Heap Leach configurations.

**Q: Can I estimate reagent consumption for gold extraction?**
Yes, you can use `estimate_reagent_needs` to predict the total mass of reagents like cyanide required for gold extraction based on ore mass and mineralogy.

**Q: How do I determine if my recovery target is achievable?**
You can use the `analyze_ore_feasibility` tool, which compares your desired recovery target against theoretical maximum extraction limits defined by the ore's mineralogy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/leaching-circuit-design](https://vinkius.com/en/ai-agent-connect/leaching-circuit-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Leaching Circuit Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `leaching-circuit-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Leaching Circuit Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leaching-circuit-design": {
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
