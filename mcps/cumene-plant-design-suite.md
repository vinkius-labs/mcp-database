# Cumene Plant Design Suite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cumene-plant-design-suite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tools for designing cumene production plants using alkylation kinetics.

## Description
This MCP server provides a complete suite of chemical engineering tools for designing cumene (isopropylbenzene) production facilities. It uses precise alkylation kinetics to determine reactor specifications via `calculate_reactor_design`, estimates zeolite catalyst needs with `estimate_catalyst_requirements`, predicts chemical outputs using `calculate_yield_and_byproducts`, and optimizes feedstock ratios with `optimize_feedstock_ratio`. It accounts for critical processes like transalkylation and PDPB removal to ensure high yield and product purity.


## Available Tools (4)
- **calculate_reactor_design**: Determines the physical specifications of the alkylation reactor required to meet target production
- **calculate_yield_and_byproducts**: Predicts the chemical output of the plant, including cumene, PIPB, and PDPB
- **estimate_catalyst_requirements**: Calculates the specific mass and type of zeolite catalyst needed for the plant
- **optimize_feedstock_ratio**: Determines the ideal molar ratio of benzene to propylene to maximize cumene selectivity and minimize byproducts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cumene Plant Design Suite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reactor design for a capacity of 50000 tons per year with 60000 tons of benzene and 30000 tons of propylene available."

**🤖 AI Agent:**
> The required reactor volume is 125 m³, with a residence time of 2.5 hours and a catalyst mass of 15,000 kg.

---

**👤 You:**
> "What is the expected yield if I have a target capacity of 10000 units, 0.95 transalkylation efficiency, and 0.98 PDPB removal rate?"

**🤖 AI Agent:**
> The predicted cumene yield is 9,450 units with an overall efficiency of 94.5%.

---

**👤 You:**
> "Find the ideal benzene to propylene ratio for a target capacity of 20000 with a desired selectivity of 0.98."

**🤖 AI Agent:**
> The ideal benzene to propylene ratio is 6:1, requiring 120,000 units of benzene and 20,000 units of propylene.


## ❓ FAQ

**Q: How do I calculate the required reactor size?**
You can use the `calculate_reactor_design` tool by providing your target capacity and the availability of benzene and propylene.

**Q: Can I optimize the feedstock to reduce byproducts?**
Yes, the `optimize_feedstock_ratio` tool calculates the ideal benzene to propylene ratio to maximize selectivity and minimize PIPB formation.

**Q: Does this tool account for catalyst degradation?**
Yes, `estimate_catalyst_requirements` provides an expected lifespan for the zeolite catalyst based on standard degradation rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cumene-plant-design-suite](https://vinkius.com/en/ai-agent-connect/cumene-plant-design-suite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cumene Plant Design Suite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cumene-plant-design-suite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cumene Plant Design Suite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cumene-plant-design-suite": {
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
