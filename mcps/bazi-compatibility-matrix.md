# BaZi Compatibility Matrix MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bazi-compatibility-matrix)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [astrology](../categories/astrology.md)

Calculate relationship compatibility using Chinese BaZi elemental and zodiac interactions.

## Description
This MCP server provides deterministic relationship analysis based on Chinese BaZi (Four Pillars) principles. It calculates compatibility through two distinct layers: the Five Elements (Wu Xing) interaction and Zodiac Animal (Earthly Branch) harmony or clash. Users can use `get_relationship_compatibility` to receive a full report containing elemental scores, zodiac scores, a total compatibility score, and a qualitative relationship verdict.


## Available Tools (3)
- **calculate_elemental_affinity**: Determine the compatibility score based solely on the Day Master elements of two individuals
- **calculate_zodiac_affinity**: Determine the compatibility score based on the zodiac animals of two individuals
- **get_relationship_compatibility**: Provide the final, comprehensive compatibility assessment by combining elemental and zodiac scores


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BaZi Compatibility Matrix** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How compatible are a Wood Day Master and a Fire Day Master whose zodiac animals are Rat and Dragon?"

**🤖 AI Agent:**
> The elemental score is +20 and the zodiac score is +20, resulting in a total compatibility score of 40. The relationship verdict is Highly Compatible.

---

**👤 You:**
> "What is the compatibility between a Water Day Master and a Fire Day Master with a Horse zodiac?"

**🤖 AI Agent:**
> The elemental score is -20 and the zodiac score is -30, resulting in a total compatibility score of -50. The relationship verdict is Clash.

---

**👤 You:**
> "Check the compatibility for a Metal Day Master and an Earth Day Master with a Tiger and Ox zodiac."

**🤖 AI Agent:**
> The elemental score is +20 and the zodiac score is 0, resulting in a total compatibility score of 20. The relationship verdict is Neutral.


## ❓ FAQ

**Q: How is the compatibility score calculated?**
The score is the sum of the elemental affinity (based on the Five Elements cycle) and the zodiac affinity (based on traditional animal harmonies and clashes).

**Q: What tools are available in this MCP?**
You can use `calculate_elemental_affinity` for element-only scores, `calculate_zodiac_affinity` for zodiac-only scores, or `get_relationship_compatibility` for a complete assessment.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP can be connected to Claude Desktop, Cursor, VS Code, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bazi-compatibility-matrix](https://vinkius.com/ai-agent-connect/bazi-compatibility-matrix)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BaZi Compatibility Matrix** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bazi-compatibility-matrix` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BaZi Compatibility Matrix** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bazi-compatibility-matrix": {
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
