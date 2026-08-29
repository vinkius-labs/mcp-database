# Polymer Additive Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/polymer-additive-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate precise additive concentrations, PHR, and batch sizes for polymer formulations.

## Description
This MCP server provides specialized tools for polymer compounding engineers to determine precise additive concentrations and batch quantities. It handles complex calculations including PHR (Parts per Hundred Resin) to mass conversions, weight percentage concentrations, masterbatch dilution requirements, and scaling theoretical formulations to specific target batch sizes. Use `calculate_phr_to_mass` to find additive weights, `calculate_masterbatch_requirement` to account for carrier resin dilution, and `scale_batch_size` to prepare production quantities.


## Available Tools (4)
- **calculate_concentration**: Determines the weight percentage of an additive in the final formulation
- **calculate_phr_to_mass**: Converts relative additive amounts (PHR) into specific mass values for a given resin quantity
- **calculate_masterbatch_requirement**: Calculates the necessary mass of a masterbatch to achieve a specific PHR of a pure additive
- **scale_batch_size**: Calculates the required mass of all components to reach a specific target finished product weight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polymer Additive Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 500kg of base resin and I need to add an additive at 5 PHR. How much additive do I need?"

**🤖 AI Agent:**
> You need 25kg of the additive.

---

**👤 You:**
> "Calculate the masterbatch needed for 100kg of resin with a target of 2 PHR of an additive that is supplied in a 20% concentration masterbatch."

**🤖 AI Agent:**
> You need 10kg of the masterbatch.

---

**👤 You:**
> "Scale a formulation to a 1000kg total batch. The additives are: UV Stabilizer at 2 PHR and Carbon Black at 3 PHR."

**🤖 AI Agent:**
> For a 1000kg batch, you need 952.38kg of base resin, 19.05kg of UV Stabilizer, and 28.57kg of Carbon Black.


## ❓ FAQ

**Q: What is PHR?**
PHR stands for Parts per Hundred Resin. It is the standard unit in polymer compounding used to express the mass of an additive relative to 100 units of the base polymer mass.

**Q: How does the masterbatch calculation work?**
The `calculate_masterbatch_requirement` tool calculates the total mass of masterbatch needed by first determining the required pure additive mass via PHR and then dividing by the masterbatch's active concentration.

**Q: Can I scale a formulation for a specific production run?**
Yes, use the `scale_batch_size` tool. You provide the target total mass and a list of additives with their PHR values to get the exact mass for every component.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/polymer-additive-calculator](https://vinkius.com/ai-agent-connect/polymer-additive-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Polymer Additive Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `polymer-additive-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Polymer Additive Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "polymer-additive-calculator": {
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
