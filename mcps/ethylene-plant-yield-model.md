# Ethylene Plant Yield Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ethylene-plant-yield-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemical-engineering](../categories/chemical-engineering.md)

Simulate and optimize petrochemical product yields from steam cracking processes.

## Description
This MCP server provides advanced simulation tools for ethylene plant operations. It allows AI agents to model the chemical transformation of hydrocarbons by analyzing feedstock composition, cracking severity, and furnace architecture. Use `calculate_yield_profile` to predict product distributions, `optimize_severity` to find the peak yield for specific chemicals, `analyze_feedstock_sensitivity` to understand how feedstock changes impact output, and `compare_furnace_efficiency` to evaluate different furnace designs.


## Available Tools (4)
- **calculate_yield_profile**: 
- **compare_furnace_efficiency**: 
- **optimize_severity**: 
- **analyze_feedstock_sensitivity**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ethylene Plant Yield Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected yield profile for a feedstock with 70% paraffins and 30% olefins at a cracking severity of 50 using a short residence time furnace?"

**🤖 AI Agent:**
> The expected yield profile is: Ethylene 35.2%, Propylene 18.5%, Butadiene 4.1%, BTX 6.2%, and Byproducts 36.0%.

---

**👤 You:**
> "What cracking severity should I use to maximize ethylene yield with this feedstock: {'paraffins': 60, 'olefins': 20, 'naphthenes': 10, 'aromatics': 10} in a standard furnace?"

**🤖 AI Agent:**
> The optimal severity to maximize ethylene yield is 75, which results in an expected ethylene yield of 42.5%.

---

**👤 You:**
> "How sensitive is the ethylene yield to changes in the paraffin content?"

**🤖 AI Agent:**
> Increasing the paraffin content by 5% results in a 3.2% increase in ethylene yield.


## ❓ FAQ

**Q: How can I predict the yield of ethylene?**
You can use the `calculate_yield_profile` tool by providing the feedstock composition, cracking severity, and the furnace type.

**Q: Can I optimize for propylene instead of ethylene?**
Yes, use the `optimize_severity` tool and set the target product to 'propylene'.

**Q: How do I compare different furnace types?**
Use the `compare_furnace_efficiency` tool to evaluate how different furnace architectures perform for your specific feedstock and severity settings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ethylene-plant-yield-model](https://vinkius.com/en/ai-agent-connect/ethylene-plant-yield-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ethylene Plant Yield Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ethylene-plant-yield-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ethylene Plant Yield Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ethylene-plant-yield-model": {
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
