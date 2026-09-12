# Ethylene Cracker Design Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ethylene-cracker-design-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

A specialized design engine for modeling steam cracking processes and furnace parameters.

## Description
This MCP server provides advanced modeling for ethylene cracker (steam cracker) design. It allows users to determine physical furnace parameters using `calculate_furnace_parameters`, forecast chemical yields with `predict_product_slate`, evaluate maintenance needs via `estimate_coking_impact`, and test design adaptability with `assess_feedstock_flexibility`. It is designed to handle various feedstocks including naphtha, ethane, and LPG.


## Available Tools (4)
- **assess_feedstock_flexibility**: To check if a designed furnace can handle an alternative feedstock without violating design constraints
- **calculate_furnace_parameters**: To determine the physical and operational design of the furnace based on target capacity and feedstock
- **estimate_coking_impact**: To evaluate the operational lifespan and maintenance requirements of the furnace
- **predict_product_slate**: To forecast the chemical composition of the output based on a specific furnace configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ethylene Cracker Design Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a furnace for 500,000 metric tons of ethane per year."

**🤖 AI Agent:**
> The furnace design for 500,000 metric tons of ethane includes a coil outlet temperature of 820°C and a residence time of 0.25 seconds.

---

**👤 You:**
> "What will the product yield be for naphtha at 850°C and 0.3 seconds residence time?"

**🤖 AI Agent:**
> At 850°C and 0.3 seconds, the predicted yields are 32% ethylene, 15% propylene, 5% butadiene, and 12% aromatics.

---

**👤 You:**
> "How much coke will accumulate after 60 days of operating with naphtha at 840°C?"

**🤖 AI Agent:**
> After 60 days of operation, the estimated coke thickness is 1.2mm with a predicted pressure drop increase of 0.05 bar.


## ❓ FAQ

**Q: What feedstocks can I model?**
The engine supports modeling for naphtha, ethane, and LPG feedstocks.

**Q: How do I check if my furnace can handle a different feedstock?**
You can use the `assess_feedstock_flexibility` tool to evaluate if a current design is compatible with an alternative feedstock type.

**Q: Can I predict the chemical output of my furnace?**
Yes, the `predict_product_slate` tool forecasts the chemical composition including ethylene, propylene, and other yields based on temperature and residence time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ethylene-cracker-design-engine](https://vinkius.com/en/ai-agent-connect/ethylene-cracker-design-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ethylene Cracker Design Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ethylene-cracker-design-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ethylene Cracker Design Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ethylene-cracker-design-engine": {
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
