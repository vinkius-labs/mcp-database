# Expansion Joint Design Engineer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/expansion-joint-design-engineer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise expansion joint specifications, including thermal movement, seismic displacement, and sealant requirements.

## Description
This MCP server provides essential engineering tools for designing building expansion joints. It allows users to calculate thermal expansion/contraction using `calculate_thermal_movement`, determine seismic displacement with `calculate_seismic_displacement`, and generate complete physical design parameters via `design_joint_specification`. Engineers can also use `get_sealant_recommendation` to identify the correct material for specific movement capacities. The tool accounts for building irregularities and seismic zones to ensure structural integrity.


## Available Tools (4)
- **calculate_seismic_displacement**: Calculates the additional displacement required for joints located in seismic zones
- **calculate_thermal_movement**: Determines the movement caused specifically by temperature fluctuations
- **design_joint_specification**: Aggregates thermal and seismic data to provide the final physical design parameters for the joint
- **get_sealant_recommendation**: Provides a detailed description of the recommended sealant material for a specific movement capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Expansion Joint Design Engineer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the thermal movement for a 100m building with a temperature range from -10°C to 40°C."

**🤖 AI Agent:**
> The thermal movement for a 100m building with a temperature delta of 50°C is 15.0 mm.

---

**👤 You:**
> "What is the recommended sealant for a joint that needs to withstand 25mm of movement?"

**🤖 AI Agent:**
> For a 25mm movement capacity, a Standard Movement Tier sealant such as Polyurethane is recommended.

---

**👤 You:**
> "Design a joint for a 50m building in a High seismic zone with 10mm of thermal movement and an irregular shape."

**🤖 AI Agent:**
> The final design requires a total movement of 45.0 mm, a required gap of 52.5 mm, a High Performance Tier sealant, and a cover plate width of 60.0 mm.


## ❓ FAQ

**Q: How does the tool handle seismic requirements?**
The `calculate_seismic_displacement` tool calculates additional movement based on the designated seismic zone classification and the building length.

**Q: Can I get specific sealant recommendations?**
Yes, by using `get_sealant_recommendation`, you can receive specific material types and application notes based on the total movement capacity.

**Q: What happens if the building has an irregular shape?**
When using `design_joint_specification`, setting `hasIrregularities` to true will trigger a safety factor increase in the required gap width to prevent structural collision.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/expansion-joint-design-engineer](https://vinkius.com/ai-agent-connect/expansion-joint-design-engineer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Expansion Joint Design Engineer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `expansion-joint-design-engineer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Expansion Joint Design Engineer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "expansion-joint-design-engineer": {
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
