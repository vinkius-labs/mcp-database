# Ergonomic Workstation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ergonomic-workstation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates precise ergonomic workstation configurations based on anthropometric measurements.

## Description
This MCP server provides deterministic ergonomic calculations to optimize workstation setups for both seated and standing modes. By providing specific user measurements, you can obtain exact recommendations for desk height, chair seat height, monitor placement, and lumbar support positioning. Use `calculate_seated_setup` for full seated configurations, `calculate_standing_setup` for standing desk heights, and `get_visual_ergonomics` for detailed monitor alignment settings.


## Available Tools (3)
- **calculate_seated_setup**: Calculates all ergonomic parameters for a user in a seated workstation configuration
- **calculate_standing_setup**: Calculates the desk height for a user in a standing workstation configuration
- **get_visual_ergonomics**: Provides specific details regarding monitor placement and viewing angles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ergonomic Workstation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my seated ergonomic setup. I am 180cm tall, my seated eye height is 80cm, my arm length is 75cm, and my lower leg length is 45cm. I am wearing shoes."

**🤖 AI Agent:**
> Your optimal seated setup is: Desk height 111.24cm, Chair seat height 43cm, Monitor height 80cm, Monitor distance 60cm, Monitor tilt 15°, Keyboard tray height 91.24cm, Lumbar support 63cm, and you do not need a footrest.

---

**👤 You:**
> "What is the best desk height for me if I am standing and 175cm tall?"

**🤖 AI Agent:**
> Your optimal standing desk height is 109.375cm.

---

**👤 You:**
> "Give me the visual ergonomics for a seated mode where my eye level is 75cm from the desk."

**🤖 AI Agent:**
> For your seated setup, the monitor top should be at 75cm, the optimal distance is 60cm, and the monitor tilt should be 15° backward.


## ❓ FAQ

**Q: How do I calculate my desk height for standing?**
You can use the `calculate_standing_setup` tool by providing your total height in centimeters.

**Q: What measurements are required for a seated setup?**
For a complete seated configuration via `calculate_seated_setup`, you need your total height, seated eye height, arm length, and lower leg length.

**Q: Does this tool account for footwear?**
Yes, the `calculate_seated_setup` tool includes an optional parameter to adjust for shoe height when calculating chair seat height.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ergonomic-workstation-calculator](https://vinkius.com/ai-agent-connect/ergonomic-workstation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ergonomic Workstation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ergonomic-workstation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ergonomic Workstation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ergonomic-workstation-calculator": {
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
