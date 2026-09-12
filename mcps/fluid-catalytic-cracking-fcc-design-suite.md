# Fluid Catalytic Cracking (FCC) Design Suite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fluid-catalytic-cracking-fcc-design-suite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design FCC units for heavy oil conversion by calculating yields, circulation rates, and thermal balances.

## Description
This MCP server provides a complete suite of engineering tools for designing Fluid Catalytic Cracking (FCC) units. It enables AI agents to model the conversion of heavy hydrocarbons into high-value products like gasoline and olefins. By using `calculate_product_yields`, you can determine the volume distribution of products based on feed properties and conversion targets. The suite also includes `determine_catalyst_circulation` to maintain heat balance, `evaluate_regenerator_conditions` to predict the thermal environment, and `analyze_deactivation_risk` to assess catalyst health based on feed contaminants and temperature.


## Available Tools (4)
- **determine_catalyst_circulation**: Calculates the required mass flow of catalyst to maintain the reaction and heat balance
- **evaluate_regenerator_conditions**: Predicts the thermal and chemical environment within the regenerator
- **analyze_deactivation_risk**: Assesses how quickly the catalyst will lose effectiveness
- **calculate_product_yields**: Determines the expected volume distribution of products based on feed and catalyst inputs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fluid Catalytic Cracking (FCC) Design Suite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the product yields for a VGO feed with density 0.85, CCR of 0.5, and distillation endpoint of 550, targeting 70% conversion with a catalyst activity of 0.9."

**🤖 AI Agent:**
> The predicted yields are: Gasoline 52.5%, LCO 18.2%, HCO 10.3%, Coke 8.5%, and Gas 10.5%.

---

**👤 You:**
> "What is the required catalyst circulation rate for a feed flow of 50,000 kg/h with a coke yield of 0.08 and a heat requirement of 1,200,000 kJ/h?"

**🤖 AI Agent:**
> The required catalyst mass flow rate is 15,000 kg/h, resulting in a circulation ratio of 0.3.

---

**👤 You:**
> "Predict the regenerator conditions for a catalyst flow of 15,000 kg/h, a coke yield of 0.08, and an oxygen availability of 2.0."

**🤖 AI Agent:**
> The predicted regenerator temperature is 695°C, with a flue gas composition of 3% CO and 2% O2.


## ❓ FAQ

**Q: How do I calculate the expected gasoline yield?**
You can use the `calculate_product_yields` tool. Provide the feed properties (density, CCR, and distillation endpoint), the desired conversion target, and the catalyst activity level.

**Q: Can this tool help with heat balance calculations?**
Yes. Use `determine_catalyst_circulation` to calculate the necessary mass flow of catalyst required to satisfy the endothermic heat requirement of the cracking reaction.

**Q: How is catalyst deactivation assessed?**
The `analyze_deactivation_risk` tool assesses risk by evaluating the feed type (VGO or Residue), metal content, and the predicted regenerator temperature.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fluid-catalytic-cracking-fcc-design-suite](https://vinkius.com/en/ai-agent-connect/fluid-catalytic-cracking-fcc-design-suite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fluid Catalytic Cracking (FCC) Design Suite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fluid-catalytic-cracking-fcc-design-suite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fluid Catalytic Cracking (FCC) Design Suite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fluid-catalytic-cracking-fcc-design-suite": {
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
