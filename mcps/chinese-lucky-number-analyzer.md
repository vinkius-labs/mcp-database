# Chinese Lucky Number Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/chinese-lucky-number-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Analyze the numerological significance of numbers based on Chinese cultural symbolism.

## Description
This MCP server provides deterministic tools to evaluate the luck and cultural meaning of numeric strings like phone numbers or license plates. Using `analyze_digit_composition`, you can find the frequency of wealth-bringing 8s or inauspicious 4s. Use `analyze_patterns` to detect specific sequences like '168' for prosperity. Finally, `calculate_auspiciousness` provides a complete summary including a lucky score and an auspiciousness rating.


## Available Tools (3)
- **analyze_patterns**: Identify specific culturally significant sequences of digits within a string
- **analyze_digit_composition**: Determine the raw frequency of specific culturally significant digits within a numeric string
- **calculate_auspiciousness**: Provide a high-level summary of the number's luck, combining digit weights and pattern analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chinese Lucky Number Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How lucky is the number 168?"

**🤖 AI Agent:**
> The number 168 is highly auspicious, representing a road to prosperity.

---

**👤 You:**
> "Analyze the number 514."

**🤖 AI Agent:**
> The number 514 is considered inauspicious and may signify bad luck.

---

**👤 You:**
> "What is the composition of 8869?"

**🤖 AI Agent:**
> The number 8869 contains two 8s, one 6, and one 9.


## ❓ FAQ

**Q: What digits are considered lucky?**
The digits 8 (wealth), 6 (smoothness), and 9 (longevity) are considered highly auspicious.

**Q: How is the lucky score calculated?**
The score is calculated by weighting 8s (+10), 6s (+5), and 9s (+5), while subtracting 15 for every 4 found.

**Q: Can I use this for license plates?**
Yes, any numeric string including license plates, phone numbers, or addresses can be analyzed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/chinese-lucky-number-analyzer](https://vinkius.com/ai-agent-connect/chinese-lucky-number-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chinese Lucky Number Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chinese-lucky-number-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chinese Lucky Number Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chinese-lucky-number-analyzer": {
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
