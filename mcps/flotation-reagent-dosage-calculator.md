# Flotation Reagent Dosage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/flotation-reagent-dosage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mining](../categories/mining.md)

Calculates precise flotation reagent requirements based on ore mineralogy and plant conditions.

## Description
This MCP server provides specialized tools for mining engineers to determine chemical reagent requirements in flotation processes. By using `calculate_reagent_dosages`, users can determine mass requirements based on ore mineralogy and laboratory test data. The `calculate_operational_requirements` tool adjusts these dosages for plant-specific factors like slurry density and retention time. Finally, `calculate_annual_consumption` predicts yearly procurement needs based on annual throughput.


## Available Tools (4)
- **calculate_operational_requirements**: Adjusts the per-tonne dosages to account for the physical properties of the actual plant slurry
- **calculate_reagent_dosages**: Determines the specific mass of each reagent type required per tonne of ore based on mineralogy and test data
- **get_mineralogy_summary**: Provides a simplified overview of the ore composition to validate input data
- **calculate_annual_consumption**: Predicts the total yearly volume of reagents needed for procurement planning


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flotation Reagent Dosage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reagent dosages for an ore with 30% Chalcopyrite and 70% Gangue, using a collector type 'Xanthate' and test dosages of 50g/t collector, 20g/t frother, and 10g/t modifier."

**🤖 AI Agent:**
> The required dosages are 150g/t for the collector, 60g/t for the frother, and 30g/t for the modifier.

---

**👤 You:**
> "Adjust a dosage of 150g/t collector for a slurry density of 35% and a retention time of 12 minutes."

**🤖 AI Agent:**
> The adjusted collector dosage is 185.5g/t.

---

**👤 You:**
> "What is the annual consumption for a collector dosage of 185.5g/t with an annual throughput of 1,000,000 tonnes?"

**🤖 AI Agent:**
> The total annual volume required for the collector is 185,500 tonnes.


## ❓ FAQ

**Q: How does the tool account for different ore compositions?**
The `calculate_reagent_dosages` tool scales the required mass of collectors and modifiers based on the target mineral concentration provided in the mineralogy input.

**Q: Can I adjust for plant-specific slurry density?**
Yes, use the `calculate_operational_requirements` tool to adjust baseline dosages for the specific slurry density and retention time of your flotation circuit.

**Q: How do I plan for yearly reagent procurement?**
You can use `calculate_annual_consumption` to multiply the adjusted per-tonne dosages by your total annual ore throughput to get the total volume needed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/flotation-reagent-dosage-calculator](https://vinkius.com/en/ai-agent-connect/flotation-reagent-dosage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flotation Reagent Dosage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flotation-reagent-dosage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flotation Reagent Dosage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flotation-reagent-dosage-calculator": {
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
