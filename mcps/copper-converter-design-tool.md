# Copper Converter Design Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/copper-converter-design-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design Peirce-Smith converter circuits for copper smelting.

## Description
This MCP server provides specialized engineering tools for designing Peirce-Smith converter circuits used in copper smelting. It allows users to calculate necessary converter dimensions, estimate blowing times for oxidation phases, determine flux requirements for slag formation, and evaluate environmental impacts like off-gas volume and copper recovery from slag. Use `calculate_converter_dimensions` to size equipment, `estimate_blowing_time` to plan production cycles, `calculate_flux_requirements` for additive calculations, and `analyze_gas_and_slag_recovery` for environmental and recovery modeling.


## Available Tools (4)
- **calculate_converter_dimensions**: Determines the necessary physical size of the converter to meet production targets
- **calculate_flux_requirements**: Determines the amount of flux needed to create sufficient slag
- **estimate_blowing_time**: Calculates how long the oxidation phase will last for a given batch
- **analyze_gas_and_slag_recovery**: Evaluates the environmental and recovery impact of the converter operation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Copper Converter Design Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What size converter do I need for a production rate of 50 tonnes of copper per hour with a matte grade of 45% and a 10 hour cycle time?"

**🤖 AI Agent:**
> The required converter will have a vessel capacity of 650 tonnes, a diameter of 5.2 meters, and a depth of 4.5 meters.

---

**👤 You:**
> "How long will it take to convert a 100 tonne matte batch with 40% copper grade and 80% oxygen availability?"

**🤖 AI Agent:**
> The blowing duration for this batch is estimated to be 145 minutes.

---

**👤 You:**
> "How much flux is needed for a 150 tonne matte batch at 35% copper grade with a silica ratio of 0.25?"

**🤖 AI Agent:**
> The required flux mass is 42.5 tonnes, resulting in a slag volume of 38.2 cubic meters.


## ❓ FAQ

**Q: How do I determine the size of my converter?**
You can use the `calculate_converter_dimensions` tool by providing the target production rate, matte grade, and the total cycle time.

**Q: Can I calculate the amount of silica needed?**
Yes, the `calculate_flux_requirements` tool calculates the required flux mass and slag volume based on the matte mass and desired silica content.

**Q: How is environmental impact assessed?**
The `analyze_gas_and_slag_recovery` tool evaluates off-gas volume and sulfur dioxide mass to help manage environmental compliance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/copper-converter-design-tool](https://vinkius.com/ai-agent-connect/copper-converter-design-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Copper Converter Design Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `copper-converter-design-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Copper Converter Design Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "copper-converter-design-tool": {
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
