# Bread Proofing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bread-proofing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Predict fermentation durations for bulk and final proofing based on yeast concentration and temperature.

## Description
This MCP server provides precise estimation tools for bakers to manage fermentation schedules. Using `get_bulk_fermentation_duration`, you can predict the first rise time based on yeast percentage and ambient heat. The `get_final_proof_duration` tool estimates the second rise after shaping. For cold-retarding techniques, `calculate_cold_delay` determines the extra time needed when moving dough to a refrigerator. Finally, use `validate_fermentation_environment` to check if your yeast and temperature settings are within optimal baking parameters.


## Available Tools (4)
- **get_bulk_fermentation_duration**: Estimates the time required for bulk fermentation
- **calculate_cold_delay**: Calculates the additional time required when moving dough to a refrigerator
- **get_final_proof_duration**: Estimates the time required for final proofing
- **validate_fermentation_environment**: Checks if the provided yeast and temperature settings are within safe or standard baking parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bread Proofing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate bulk fermentation for 2% yeast at 25°C."

**🤖 AI Agent:**
> The estimated duration for bulk fermentation is approximately 120 minutes with a high confidence score.

---

**👤 You:**
> "How much extra time is needed if I move dough from 25°C to a 4°C fridge?"

**🤖 AI Agent:**
> Based on the temperature drop, you will need an additional delay of approximately 180 minutes.

---

**👤 You:**
> "Check if 5% yeast at 35°C is a good environment."

**🤖 AI Agent:**
> The environment is viable, but there is a risk of over-proofing due to the high temperature.


## ❓ FAQ

**Q: How accurate are the fermentation estimates?**
Estimates are based on biological models of yeast activity. Accuracy depends on the stability of your inputs, which is reflected in the confidence score returned by `get_bulk_fermentation_duration`.

**Q: Can I calculate the delay for cold proofing?**
Yes. Use the `calculate_cold_delay` tool by providing your base duration, fridge temperature, and ambient temperature.

**Q: Does the tool check for extreme temperatures?**
Yes, the `validate_fermentation_environment` tool identifies if your yeast and temperature settings are within standard baking parameters or at risk of failure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bread-proofing-calculator](https://vinkius.com/mcp/bread-proofing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bread Proofing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bread-proofing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bread Proofing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bread-proofing-calculator": {
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
