# Chinese Zodiac & Elemental Cycle Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/chinese-zodiac-elemental-cycle-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [astrology](../categories/astrology.md)

Calculate zodiac animals, elements, and compatibility using the sexagenary cycle.

## Description
This MCP server provides precise calculations for the Chinese sexagenary cycle. It connects AI agents to the complex system of ten Heavenly Stems and twelve Earthly Branches. Use `get_zodiac_details` to find a specific animal, element, and polarity for any birth date, accounting for the Lunar New Year shift. Use `get_compatibility_analysis` to identify trine groups and conflicting animals, or `get_cycle_period` to locate a year within its 60-year cycle.


## Available Tools (3)
- **get_compatibility_analysis**: Determines how a specific zodiac animal relates to others through trines and clashes
- **get_cycle_period**: Identifies which 60-year cycle a specific year belongs to
- **get_zodiac_details**: Identifies the specific zodiac attributes for a given date or year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chinese Zodiac & Elemental Cycle Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my zodiac sign if I was born on February 10, 1990?"

**🤖 AI Agent:**
> You were born in the year of the Metal Horse.

---

**👤 You:**
> "Which animals are compatible with the Dragon?"

**🤖 AI Agent:**
> The animals in the same trine as the Dragon are the Rat and the Monkey.

---

**👤 You:**
> "What is the 60-year cycle position for the year 2024?"

**🤖 AI Agent:**
> The year 2024 is at position 45 in its current 60-year cycle.


## ❓ FAQ

**Q: How does the tool handle the Lunar New Year?**
The `get_zodiac_details` tool accounts for the Lunar New Year shift, ensuring the zodiac animal is correctly assigned based on the specific date rather than just the calendar year.

**Q: Can I check animal compatibility?**
Yes, you can use `get_compatibility_analysis` to find compatible trine groups and animals that clash with a specific zodiac sign.

**Q: What information is provided for a specific year?**
You can retrieve the zodiac animal, the heavenly stem element (Wood, Fire, Earth, Metal, or Water), the earthly branch, the yin/yang polarity, and the exact position in the 60-year cycle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/chinese-zodiac-elemental-cycle-calculator](https://vinkius.com/ai-agent-connect/chinese-zodiac-elemental-cycle-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chinese Zodiac & Elemental Cycle Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chinese-zodiac-elemental-cycle-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chinese Zodiac & Elemental Cycle Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chinese-zodiac-elemental-cycle-calculator": {
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
