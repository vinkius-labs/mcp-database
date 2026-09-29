# Pet Equipment Acquisition Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-equipment-acquisition-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Evaluates pet equipment suitability based on physical constraints, budget, and usage needs.

## Description
This MCP server provides a decision-support engine for pet owners. It uses `evaluate_equipment_fit` to check if items fit in homes or vehicles, `calculate_logistics_impact` to assess space clearance, `validate_vendor_risk` to analyze return policies, and `generate_acquisition_brief` to produce final purchase strategies.


## Available Tools (4)
- **calculate_logistics_impact**: Assesses how the equipment will affect the user's space and movement
- **evaluate_equipment_fit**: Determines if a specific piece of equipment is physically and financially viable for the user's environment and budget
- **generate_acquisition_brief**: Produces the final summary including the decision, vendor queries, and logistics
- **validate_vendor_risk**: Evaluates if the vendor's terms allow for a safe "deferral" or "return" if the item is unsuitable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Equipment Acquisition Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Will this pet crate fit in my SUV?"

**🤖 AI Agent:**
> The crate dimensions are 30x20x25 inches and your SUV cargo area is 40x30x30 inches. It fits with 10 inches of clearance in length.

---

**👤 You:**
> "Is it safe to buy this expensive pet bed with a 3-day return window?"

**🤖 AI Agent:**
> No, the risk level is High because the 3-day return window is too short to verify the fit in your home.

---

**👤 You:**
> "Can I afford the premium climbing tower?"

**🤖 AI Agent:**
> No, the tower costs $450 and your budget limit is $350.


## ❓ FAQ

**Q: How does the tool determine if an item fits?**
The `evaluate_equipment_fit` tool compares the item's dimensions against your available space and budget limits.

**Q: Can I check vendor return risks?**
Yes, `validate_vendor_risk` evaluates return windows and restocking fees to suggest if you should proceed or exercise caution.

**Q: What is the final output of the planner?**
The `generate_acquisition_brief` tool produces a complete strategy including a decision summary, vendor questions, and setup actions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-equipment-acquisition-planner](https://vinkius.com/en/ai-agent-connect/pet-equipment-acquisition-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Equipment Acquisition Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-equipment-acquisition-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Equipment Acquisition Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-equipment-acquisition-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
