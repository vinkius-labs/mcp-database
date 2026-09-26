# Wildfire Smoke Logistics Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wildfire-smoke-logistics-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-management](../categories/emergency-management.md)

Generates actionable evacuation and sheltering plans based on smoke alerts and household constraints.

## Description
This MCP server provides a logistics engine to manage wildfire smoke responses. It uses `analyze_smoke_risk` to determine risk levels, `evaluate_indoor_safety` to assess if shelter-in-place is viable, `generate_relocation_plan` to create movement timelines, and `compile_readiness_checklist` to produce essential supply lists. It connects AI agents to critical decision-making logic for household safety during smoke events.


## Available Tools (4)
- **compile_readiness_checklist**: Compile readiness checklist
- **analyze_smoke_risk**: Analyze smoke risk
- **evaluate_indoor_safety**: Evaluate indoor safety
- **generate_relocation_plan**: Generate relocation plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wildfire Smoke Logistics Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the risk for a household with two adults and one elderly person given this alert: 'Smoke concentration increasing in Zone A'."

**🤖 AI Agent:**
> The risk level is Moderate. The recommended action is Prepare. The primary constraint is the mobility of the elderly household member.

---

**👤 You:**
> "Is it safe to stay in a 2000 sq ft house with a HEPA purifier rated at 300 CFM during a Level 2 smoke event?"

**🤖 AI Agent:**
> No, the filtration effectiveness is insufficient for this volume. The safety buffer is estimated at 2 hours before air quality degrades.

---

**👤 You:**
> "Generate a checklist for a relocation action for a family of four."

**🤖 AI Agent:**
> Supply Checklist: 4 days of water, non-perishable food, first aid kit. Document Checklist: IDs, insurance papers, emergency contacts. Equipment Checklist: Portable air purifier, extra batteries.


## ❓ FAQ

**Q: How does the tool determine if I should stay or leave?**
The `analyze_smoke_risk` tool evaluates official alert details against your household composition to recommend staying, preparing, or relocating.

**Q: Can it help me prepare for an evacuation?**
Yes, you can use `compile_readiness_checklist` to generate specific lists of supplies, documents, and equipment needed for your chosen action.

**Q: How is indoor air safety calculated?**
The `evaluate_indoor_safety` tool calculates safety by comparing your air filtration equipment's technical ratings against the volume of your indoor space and the current smoke concentration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wildfire-smoke-logistics-plan](https://vinkius.com/en/ai-agent-connect/wildfire-smoke-logistics-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wildfire Smoke Logistics Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wildfire-smoke-logistics-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wildfire Smoke Logistics Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wildfire-smoke-logistics-plan": {
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
