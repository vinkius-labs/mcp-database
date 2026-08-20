# Seimei Handan Fortune Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/seimei-handan-fortune-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Calculate Japanese name fortunes using the traditional Five Grids (Go-Grid) system.

## Description
This MCP server provides tools to perform Seimei Handan, a traditional Japanese practice of determining destiny through name stroke counts. By using `calculate_name_fortune`, an AI agent can determine the five fundamental destiny grids: Heaven, Earth, Person, Outer, and Total. The server also includes `validate_stroke_counts` to ensure inputs are realistic and `get_method_description` to explain the difference between the traditional Kangxi radical system and the modern Japanese counting method.


## Available Tools (3)
- **calculate_name_fortune**: 
- **get_method_description**: Get description of the counting method
- **validate_stroke_counts**: Validate if stroke count is within realistic bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Seimei Handan Fortune Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fortune for a name with 10 family name strokes and 5 given name strokes using the modern method. The first family char has 4 strokes and the last given char has 1 stroke."

**🤖 AI Agent:**
> The Heaven Grid is 11, Earth Grid is 5, Person Grid is 15, Outer Grid is 5, and Total Grid is 15. The overall fortune is auspicious.

---

**👤 You:**
> "What is the difference between the two counting methods?"

**🤖 AI Agent:**
> The Kangxi method is based on traditional radicals, whereas the modern method follows contemporary Japanese stroke counting standards.

---

**👤 You:**
> "Is a total stroke count of 150 valid for a Japanese name?"

**🤖 AI Agent:**
> No, a total stroke count of 150 is outside the realistic bounds for standard Japanese names.


## ❓ FAQ

**Q: What are the Five Grids?**
The Five Grids (Go-Grid) are the Heaven, Earth, Person, Outer, and Total grids used to evaluate a name's fortune.

**Q: What is the difference between Kangxi and modern methods?**
The Kangxi method uses traditional radical-based stroke counts, while the modern method uses standard contemporary Japanese stroke orders.

**Q: How is the overall fortune determined?**
The overall fortune is determined by whether the Total Grid score matches a specific set of auspicious numbers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/seimei-handan-fortune-calculator](https://vinkius.com/ai-agent-connect/seimei-handan-fortune-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Seimei Handan Fortune Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seimei-handan-fortune-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Seimei Handan Fortune Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seimei-handan-fortune-calculator": {
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
