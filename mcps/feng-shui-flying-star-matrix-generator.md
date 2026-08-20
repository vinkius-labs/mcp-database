# Feng Shui Flying Star Matrix Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/feng-shui-flying-star-matrix-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Generate deterministic annual Xuan Kong Flying Star matrices and analyze sector auspiciousness.

## Description
This MCP server provides precise tools for Xuan Kong Feng Shui practitioners. Use `generate_annual_matrix` to calculate the 3x3 Lo Shu square based on a target year and building mountain direction. You can then use `analyze_sector_auspiciousness` to identify beneficial stars like 1, 8, and 9, or problematic stars like 2 and 5. Additionally, `get_direction_metadata` helps translate mountain indices into human-readable compass directions.


## Available Tools (3)
- **analyze_sector_auspiciousness**: Evaluates which sectors of a generated matrix are considered favorable or unfavorable
- **get_direction_metadata**: Translates mountain numbers into human-readable compass directions and cardinal sectors
- **generate_annual_matrix**: Generates the complete 3x3 Flying Star matrix for a specific year and building orientation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feng Shui Flying Star Matrix Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate the flying star matrix for the year 2024 with a facing mountain of 1."

**🤖 AI Agent:**
> The 3x3 matrix for 2024 with mountain 1 has been generated with the center star being 7.

---

**👤 You:**
> "Which sectors are inauspicious in this matrix: [[8, 1, 9], [3, 7, 4], [2, 5, 6]]?"

**🤖 AI Agent:**
> The inauspicious sectors are those containing stars 2 and 5.

---

**👤 You:**
> "What is the direction for mountain index 5?"

**🤖 AI Agent:**
> Mountain index 5 corresponds to the East-Southeast direction.


## ❓ FAQ

**Q: How do I calculate the annual star for a specific year?**
You can use the `generate_annual_matrix` tool by providing the target Gregorian year and the building's facing mountain direction (1-24).

**Q: What are considered auspicious sectors?**
Sectors containing stars 1, 8, or 9 are considered auspicious for prosperity and stability.

**Q: Can I find the compass direction for a mountain index?**
Yes, use the `get_direction_metadata` tool with the mountain index (1-24) to get the descriptive name and cardinal sector.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/feng-shui-flying-star-matrix-generator](https://vinkius.com/ai-agent-connect/feng-shui-flying-star-matrix-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Feng Shui Flying Star Matrix Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `feng-shui-flying-star-matrix-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Feng Shui Flying Star Matrix Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "feng-shui-flying-star-matrix-generator": {
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
