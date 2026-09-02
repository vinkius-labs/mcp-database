# Coffee Brewing Ratio Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/coffee-brewing-ratio-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Deterministic coffee brewing calculator based on SCA Golden Cup Standards.

## Description
This MCP server provides precise brewing calculations following the SCA Golden Cup Standard. It allows AI agents to determine exact coffee doses, water volumes, and temperature targets for various methods. Use `calculate_brew_parameters` to get a full brewing schedule, `get_method_recommendations` to find ideal ratios, or `validate_ratio_compatibility` to check if your chosen ratio fits your method.


## Available Tools (3)
- **get_method_recommendations**: Suggests optimal ratios and temperatures for specific brew methods if the user is unsure
- **calculate_brew_parameters**: Calculates the core ingredients and timing required for a specific brew
- **validate_ratio_compatibility**: Checks if a specific user-provided ratio is appropriate for a chosen brewing method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coffee Brewing Ratio Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to make 300ml of pour-over coffee with a 1:15 ratio. What do I need?"

**🤖 AI Agent:**
> For a 300ml pour-over at a 1:15 ratio, you need 20g of coffee and 300ml of water. The recommended temperature is 93°C. Start with a bloom phase, then follow the pour stages.

---

**👤 You:**
> "What are the recommended ratios for French Press?"

**🤖 AI Agent:**
> Standard ratios for French Press typically range between 1:13 and 1:18.

---

**👤 You:**
> "Is a 1:50 ratio okay for Espresso?"

**🤖 AI Agent:**
> No, a 1:50 ratio is not appropriate for espresso; espresso requires much tighter ratios, typically between 1:1 and 1:3.


## ❓ FAQ

**Q: What standards does this engine follow?**
The engine uses the SCA Golden Cup Standard to ensure optimal extraction and flavor profiles.

**Q: How do I get a pouring schedule?**
You can use the `calculate_brew_parameters` tool, which returns a detailed list of pour stages.

**Q: Can I use this for Espresso?**
Yes, the engine supports espresso with specific temperature and ratio logic designed for high-pressure extraction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/coffee-brewing-ratio-engine](https://vinkius.com/ai-agent-connect/coffee-brewing-ratio-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coffee Brewing Ratio Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coffee-brewing-ratio-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coffee Brewing Ratio Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coffee-brewing-ratio-engine": {
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
