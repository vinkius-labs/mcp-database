# Wax Selection Guide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wax-selection-guide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Recommends specialized ski waxes based on real-time snow and environmental conditions.

## Description
This MCP server provides expert-level ski wax recommendations by analyzing snow temperature, air temperature, humidity, and snow type. It uses a specialized performance model to determine the best wax chemistry for your specific conditions. You can use `get_wax_recommendation` to find the ideal wax type, `get_application_instructions` for step-by-step physical application guides, `calculate_durability_estimate` to predict how long your wax will last, and `compare_wax_options` to evaluate hydrocarbon versus fluorocarbon performance.


## Available Tools (4)
- **calculate_durability_estimate**: Predicts how long the wax will remain effective under current conditions
- **compare_wax_options**: Compares a hydrocarbon-based wax against a fluorocarbon-based wax for a specific scenario
- **get_application_instructions**: Details how to physically apply the recommended wax for optimal performance
- **get_wax_recommendation**: Provides the primary recommendation for wax type and application based on environmental data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wax Selection Guide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What wax should I use for -5°C snow, -2°C air temperature, 40% humidity, and powder snow?"

**🤖 AI Agent:**
> For these conditions, a high-performance hydrocarbon wax is recommended to handle the cold, dry powder snow.

---

**👤 You:**
> "How long will my wax last in icy snow at -10°C?"

**🤖 AI Agent:**
> Under icy conditions at -10°C, the wax is expected to remain effective for approximately 4 hours due to high snow abrasiveness.

---

**👤 You:**
> "Give me instructions for applying a fluorocarbon wax on slushy snow."

**🤖 AI Agent:**
> To apply fluorocarbon wax on slush, first clean the base, then use a high-temperature iron to melt the wax into the base, followed by a thorough scrape and brush.


## ❓ FAQ

**Q: How does the tool determine the wax recommendation?**
The system analyzes the relationship between snow temperature (hardness) and humidity (hydrophobicity) to select the optimal wax chemistry.

**Q: Can I get application steps for the recommended wax?**
Yes, you can use `get_application_instructions` to receive detailed steps and tool requirements for applying your specific wax.

**Q: How accurate is the durability estimate?**
The estimate is based on a model that accounts for snow abrasiveness and temperature, providing a predicted number of hours remaining for the wax.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wax-selection-guide](https://vinkius.com/en/ai-agent-connect/wax-selection-guide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wax Selection Guide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wax-selection-guide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wax Selection Guide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wax-selection-guide": {
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
