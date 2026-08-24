# Numismatic Grading & Value Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/numismatic-grading-value-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Sheldon grades and market values for US coins.

## Description
This MCP server provides professional-grade numismatic analysis for US coinage. Use `calculate_sheldon_grade` to determine a coin's numerical grade and adjectival label based on physical condition like wear and luster. Use `estimate_coin_value` to calculate market value and melt value using current spot prices. You can also use `get_coin_metadata` to retrieve technical specifications like metal content and weight for specific denominations.


## Available Tools (3)
- **get_coin_metadata**: 
- **calculate_sheldon_grade**: 
- **estimate_coin_value**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Numismatic Grading & Value Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the grade of a Lincoln cent with 5% wear, 90% luster, sharp strike, and clean surface?"

**🤖 AI Agent:**
> The calculated grade is MS-65.

---

**👤 You:**
> "Estimate the value of a 1921 Morgan Dollar, grade 60, with silver at $25 per ounce."

**🤖 AI Agent:**
> $35.50

---

**👤 You:**
> "What is the metal content of a Walking Liberty Half Dollar?"

**🤖 AI Agent:**
> Silver (90% fine silver).


## ❓ FAQ

**Q: How do I determine the grade of my coin?**
You can use the `calculate_sheldon_grade` tool. Provide details regarding the wear percentage, luster, strike quality, and surface marks to receive a Sheldon scale grade.

**Q: Does this tool account for precious metal prices?**
Yes. When using `estimate_coin_value`, you provide the current spot price, and the tool will calculate both the numismatic value and the melt value.

**Q: Can I get technical details about specific coins?**
Yes, the `get_coin_metadata` tool provides technical specifications such as metal content and weight for supported US coin types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/numismatic-grading-value-estimator](https://vinkius.com/ai-agent-connect/numismatic-grading-value-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Numismatic Grading & Value Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `numismatic-grading-value-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Numismatic Grading & Value Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "numismatic-grading-value-estimator": {
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
