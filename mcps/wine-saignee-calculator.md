# Wine Saignée Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-saignee-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate juice removal volumes and color impact for rosé production.

## Description
This MCP server provides specialized tools for enologists to manage the saignée (bleeding) process. It calculates precise volumes for juice removal, predicts how increasing the skin-to-juice ratio affects color intensity, and recommends optimal bleeding windows based on whether the goal is color or structure. Use `calculate_saignee_volumes` to determine volumes, `estimate_color_impact` to predict color changes, `optimize_bleeding_timing` for timing advice, and `predict_final_wine_characteristics` to estimate the final properties of the resulting rosé.


## Available Tools (4)
- **estimate_color_impact**: Predicts how the removal of juice will affect the color intensity of the remaining must
- **predict_final_wine_characteristics**: Estimates the final properties of the rosé produced from the remaining must
- **optimize_bleeding_timing**: Recommends the best window for the bleed based on whether the goal is color or structure
- **calculate_saignee_volumes**: Determines the specific volumes involved in the bleeding process based on target removal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Saignée Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 1000 liters of must and I want to remove 20%. How much juice should I take out?"

**🤖 AI Agent:**
> You should remove 200 liters of juice, leaving 800 liters of must.

---

**👤 You:**
> "My initial skin-to-juice ratio is 0.1 and I plan to remove 30% of the juice. What will the color impact be?"

**🤖 AI Agent:**
> The new skin-to-juice ratio will be approximately 0.14, resulting in a color intensity multiplier of 1.43.

---

**👤 You:**
> "I want to prioritize color for my rosé. What is the best time to perform a 25% bleed?"

**🤖 AI Agent:**
> For a color-focused goal, it is recommended to perform the bleed early in the maceration period to maximize skin contact with the concentrated juice.


## ❓ FAQ

**Q: How do I calculate the volume to be removed?**
You can use the `calculate_saignee_volumes` tool by providing the initial must volume and your target removal percentage.

**Q: Can this tool help with color optimization?**
Yes, the `estimate_color_impact` tool predicts how juice removal affects color intensity by calculating the new skin-to-juice ratio.

**Q: What is the difference between color and structure goals?**
Color goals focus on maximizing anthocyanin extraction, while structure goals balance skin contact with the preservation of delicate aromatics. Use `optimize_bleeding_timing` to get recommendations for either.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-saignee-calculator](https://vinkius.com/en/ai-agent-connect/wine-saignee-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Saignée Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-saignee-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Saignée Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-saignee-calculator": {
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
