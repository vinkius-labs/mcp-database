# Outfit Color Harmony MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/outfit-color-harmony)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Evaluates clothing color combinations using color theory models.

## Description
This MCP server provides tools to evaluate the aesthetic relationship between clothing colors. Use `analyze_color_harmony` to score color pairs, `suggest_complementary_palette` for high-contrast opposites, `verify_neutral_balance` to check accent visibility, and `find_analogous_transitions` for cohesive, low-contrast palettes.


## Available Tools (4)
- **analyze_color_harmony**: Evaluates a specific combination of colors against a chosen harmony model
- **find_analogous_transitions**: Finds colors that are visually adjacent to a given color
- **suggest_complementary_palette**: Generates a high-contrast palette based on a single primary color
- **verify_neutral_balance**: Checks if an accent color effectively stands out against a neutral base


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outfit Color Harmony** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Does a navy blue shirt and an orange tie work well together?"

**🤖 AI Agent:**
> Yes, the combination of navy blue and orange provides a high contrast ratio and a strong complementary harmony score.

---

**👤 You:**
> "Find some colors similar to forest green for a subtle look."

**🤖 AI Agent:**
> The adjacent colors for forest green are olive green and teal.

---

**👤 You:**
> "Is a light grey base with a bright red accent balanced?"

**🤖 AI Agent:**
> Yes, the bright red accent provides significant saturation and brightness compared to the light grey neutral base.


## ❓ FAQ

**Q: How do I check if my accent color works?**
You can use the `verify_neutral_balance` tool to ensure your high-saturation accent color provides enough contrast against your neutral base.

**Q: Can I generate a high-contrast palette?**
Yes, use `suggest_complementary_palette` to find the direct mathematical opposite of your base color.

**Q: What harmony models are supported?**
The server supports complementary, analogous, triadic, and neutral-accent models via the `analyze_color_harmony` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/outfit-color-harmony](https://vinkius.com/en/ai-agent-connect/outfit-color-harmony)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outfit Color Harmony** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `outfit-color-harmony` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outfit Color Harmony** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outfit-color-harmony": {
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
