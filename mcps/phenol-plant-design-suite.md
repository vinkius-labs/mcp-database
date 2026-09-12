# Phenol Plant Design Suite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/phenol-plant-design-suite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [process-design](../categories/process-design.md)

Engineering tools for designing phenol production plants via cumene oxidation.

## Description
This MCP server provides a complete suite of chemical engineering tools for designing phenol production plants using the cumene oxidation pathway. It allows engineers to `calculate_oxidation_parameters` to set initial reaction conditions, `design_cleavage_reactor` to specify reactor dimensions and heat duty, `estimate_product_yields` to predict phenol and acetone outputs, and `evaluate_purity_compliance` to ensure final product quality meets industrial standards.


## Available Tools (4)
- **calculate_oxidation_parameters**: Determine the necessary physical conditions for the initial cumene oxidation stage
- **design_cleavage_reactor**: Specify the dimensions and operational parameters of the reactor where hydroperoxide is converted to phenol
- **estimate_product_yields**: Calculate the expected output of phenol and acetone based on the design parameters
- **evaluate_purity_compliance**: Check if the designed process can meet specific target purity standards for the final products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Phenol Plant Design Suite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the oxidation parameters for 500 units of cumene with a target capacity of 200 units of phenol."

**🤖 AI Agent:**
> The required oxidation temperature range is 100-120°C with an oxygen requirement of 150 units and a reaction time of 4 hours.

---

**👤 You:**
> "What are the expected yields if I have 100 units of throughput, 0.95 conversion efficiency, and 0.92 cleavage selectivity?"

**🤖 AI Agent:**
> The expected yields are 87.4 units of phenol and 87.4 units of acetone, with a byproduct yield of 7.6 units.

---

**👤 You:**
> "Will my process be compliant if I have 90 units of phenol and a byproduct concentration of 0.005 for a 99% target purity?"

**🤖 AI Agent:**
> No, the process is not compliant. The current purity is approximately 99.5%, but the gap analysis suggests higher purification intensity is needed to meet the strict 99% threshold reliably.


## ❓ FAQ

**Q: How do I determine the initial oxidation conditions?**
You can use the `calculate_oxidation_parameters` tool by providing the available cumene and your target phenol capacity.

**Q: Can I check if my phenol meets purity requirements?**
Yes, the `evaluate_purity_compliance` tool checks your calculated phenol yield and byproduct concentration against your target purity.

**Q: How is the reactor size determined?**
The `design_cleavage_reactor` tool calculates the required reactor volume and heat duty based on CHP concentration and residence time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/phenol-plant-design-suite](https://vinkius.com/en/ai-agent-connect/phenol-plant-design-suite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Phenol Plant Design Suite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `phenol-plant-design-suite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Phenol Plant Design Suite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "phenol-plant-design-suite": {
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
