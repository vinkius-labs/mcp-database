# Gua Sha Pressure Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gua-sha-pressure-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Determine precise Gua Sha pressure, stroke direction, and lubricant needs.

## Description
This MCP server provides specialized tools for Gua Sha practitioners and enthusiasts to ensure safe and effective treatments. By analyzing the treatment area, skin condition, tool type, and therapeutic goal, the server calculates exact parameters for each session. Use `calculate_treatment_plan` to receive a complete set of instructions including pressure level, stroke direction, and stroke count. You can also use `get_area_sensitivity_guide` to check pressure limits for specific body parts, `get_tool_compatibility` to verify tool safety, and `estimate_lubricant_needs` to prevent skin tugging.


## Available Tools (4)
- **calculate_treatment_plan**: Generates a complete set of instructions for a specific Gua Sha session
- **estimate_lubricant_needs**: Calculates the necessary amount of oil or balm to prevent skin tugging
- **get_area_sensitivity_guide**: Provides standardized pressure limits for various body parts
- **get_tool_compatibility**: Checks if a specific tool is appropriate for a given skin condition and goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gua Sha Pressure Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to do lymphatic drainage on my face using a jade stone. My skin is normal."

**🤖 AI Agent:**
> For lymphatic drainage on the face with jade stone, use Light pressure. Follow a downward and outward stroke direction. Perform 15 strokes, and use a moderate amount of facial oil.

---

**👤 You:**
> "What is the pressure limit for my neck if I have sensitive skin?"

**🤖 AI Agent:**
> For sensitive skin on the neck, the recommended maximum pressure is Light.

---

**👤 You:**
> "I'm using stainless steel for muscle tension relief on my shoulders. How many strokes do I need?"

**🤖 AI Agent:**
> For muscle tension relief on the shoulders using stainless steel, perform 25 strokes with Medium pressure in an upward direction.


## ❓ FAQ

**Q: How do I get a full treatment plan?**
You can use the `calculate_treatment_plan` tool by providing the treatment area, skin condition, tool type, and your specific goal.

**Q: Can I check if my jade stone is safe for sensitive skin?**
Yes, use the `get_tool_compatibility` tool to verify if your specific tool is suitable for your current skin condition.

**Q: How much oil should I use for my facial massage?**
Use the `estimate_lubricant_needs` tool to get a specific recommendation based on your skin type and the area being treated.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gua-sha-pressure-calculator](https://vinkius.com/en/ai-agent-connect/gua-sha-pressure-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gua Sha Pressure Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gua-sha-pressure-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gua Sha Pressure Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gua-sha-pressure-calculator": {
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
