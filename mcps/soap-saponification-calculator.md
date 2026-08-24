# Soap Saponification Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/soap-saponification-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Deterministic cold-process soap formulation calculator for precise lye and water requirements.

## Description
This MCP server provides precise chemical calculations for soap makers. Use `calculate_formulation` to determine exact lye and water amounts, fatty acid profiles, and predicted soap properties like hardness and cleansing. You can also use `get_oil_data` to retrieve specific SAP values and `analyze_soap_quality` to evaluate if your recipe meets industry stability benchmarks based on the INS value.


## Available Tools (3)
- **analyze_soap_quality**: Evaluates predicted soap properties against industry benchmarks
- **calculate_formulation**: Calculates exact chemical requirements and soap quality metrics for a blend of oils
- **get_oil_data**: g., "Olive", "Coconut").

Provides specific chemical constants for a given oil


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Soap Saponification Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a soap recipe with 500g olive oil, 200g coconut oil, and 300g palm oil using 5% superfat and NaOH at 33% concentration."

**🤖 AI Agent:**
> For your recipe, you will need 123.45g of NaOH and 251.23g of water. The fatty acid profile includes high oleic acid, and the predicted hardness score is 65.

---

**👤 You:**
> "What are the chemical properties of coconut oil?"

**🤖 AI Agent:**
> Coconut oil has a NaOH SAP value of 0.190 and a KOH SAP value of 0.175. Its fatty acid profile is primarily composed of lauric and myristic acids.

---

**👤 You:**
> "Is my soap recipe stable with an INS value of 120?"

**🤖 AI Agent:**
> The stability rating is Soft. Since the INS value is below the target range of 136-170, you may want to increase the proportion of harder fats like stearic or palmitic acids to improve stability.


## ❓ FAQ

**Q: How do I calculate the lye needed for my recipe?**
You can use the `calculate_formulation` tool by providing a list of your oil weights, the desired superfat percentage, the lye type (NaOH or KOH), and your target lye concentration.

**Q: What is an INS value?**
The INS value is a composite score used to predict the stability and melting point of soap. A target range of 136 to 170 is generally recommended for balanced bar soap.

**Q: Can I use this for liquid soap?**
Yes, by selecting KOH as the lye type in the `calculate_formulation` tool, the calculator will provide requirements for liquid soap formulations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/soap-saponification-calculator](https://vinkius.com/ai-agent-connect/soap-saponification-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Soap Saponification Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soap-saponification-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Soap Saponification Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soap-saponification-calculator": {
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
