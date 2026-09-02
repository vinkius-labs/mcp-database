# Waterproofing Warranty & Maintenance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/waterproofing-warranty-maintenance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Determine warranty durations, maintenance schedules, and risk profiles for waterproofing systems.

## Description
This MCP server provides specialized tools to manage waterproofing system lifecycles. Use `calculate_warranty_period` to determine recommended warranty years based on system type, substrate condition, and exposure. Use `generate_maintenance_plan` to create structured upkeep schedules. You can also use `evaluate_risk_profile` to identify potential failure points and `get_manufacturer_constraints` to retrieve baseline requirements for specific technologies.


## Available Tools (4)
- **calculate_warranty_period**: Determine the recommended warranty duration and exclusion criteria for a waterproofing system
- **evaluate_risk_profile**: Assess the probability of early failure based on installation and environmental factors
- **generate_maintenance_plan**: Generate a structured maintenance schedule and inspection frequency
- **get_manufacturer_constraints**: Retrieve baseline requirements and limitations set by manufacturers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Waterproofing Warranty & Maintenance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the recommended warranty for a Liquid Membrane on an excellent substrate with moderate exposure?"

**🤖 AI Agent:**
> The recommended warranty for a Liquid Membrane under these conditions is 15 years.

---

**👤 You:**
> "Generate a maintenance plan for a Sheet Membrane in an extreme exposure environment."

**🤖 AI Agent:**
> The maintenance plan includes quarterly debris removal, bi-annual surface inspections, and annual sealant checks.

---

**👤 You:**
> "What are the manufacturer constraints for Bituminous Coatings?"

**🤖 AI Agent:**
> Bituminous Coatings have a base warranty of 5 years and require annual cleaning. They are prohibited in high-temperature industrial environments.


## ❓ FAQ

**Q: How do I calculate a warranty for a new installation?**
You can use the `calculate_warranty_period` tool. Provide the system type, substrate condition, exposure conditions, workmanship quality, and installer reputation to get a recommended duration.

**Q: Can I get a maintenance schedule for my specific system?**
Yes, the `generate_maintenance_plan` tool creates a tailored schedule and inspection frequency based on the system type and environmental exposure.

**Q: What factors influence the risk of waterproofing failure?**
The `evaluate_risk_profile` tool analyzes substrate condition, workmanship quality, and exposure conditions to determine the probability of early failure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/waterproofing-warranty-maintenance](https://vinkius.com/ai-agent-connect/waterproofing-warranty-maintenance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Waterproofing Warranty & Maintenance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `waterproofing-warranty-maintenance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Waterproofing Warranty & Maintenance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "waterproofing-warranty-maintenance": {
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
