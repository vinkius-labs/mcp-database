# Xiaohongshu (RED) Title Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/xiaohongshu-red-title-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Transform base headlines into viral Xiaohongshu titles using weighted character counts and keyword density rules.

## Description
This MCP server provides a deterministic engine to optimize headlines specifically for the Xiaohongshu (RED) platform. It uses a unique weighted character count (Chinese=1, English=0.5, Emoji=2) to ensure optimal visual density. The engine applies viral formatting rules, including mandatory hooks and emotive punctuation, while calculating a CTR score based on keyword density and visual weight. Use `optimize_title` to generate high-engagement headlines, `analyze_keyword_density` to measure keyword integration, or `calculate_visual_weight` to check visual length.


## Available Tools (3)
- **calculate_visual_weight**: 
- **analyze_keyword_density**: 
- **optimize_title**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Xiaohongshu (RED) Title Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Optimize this title for Xiaohongshu: 'My trip to Paris'"

**🤖 AI Agent:**
> Paris trip guide! 🇫🇷✨

---

**👤 You:**
> "Calculate the visual weight of 'Hello World 😊'"

**🤖 AI Agent:**
> 5.0

---

**👤 You:**
> "Check the keyword density for 'Best coffee in town' with keywords ['coffee', 'best']"

**🤖 AI Agent:**
> 1.0


## ❓ FAQ

**Q: How is the character count calculated?**
The engine uses a weighted system: Chinese characters count as 1, English letters count as 0.5, and emojis count as 2 to reflect visual density on the platform.

**Q: What does the CTR score represent?**
The CTR score is an estimate of engagement probability based on keyword presence, emoji usage, and how close the title is to the optimal visual weight of 15-20 units.

**Q: Can I check the keyword density of an existing title?**
Yes, you can use the `analyze_keyword_density` tool to calculate the ratio of matched target keywords within any title string.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/xiaohongshu-red-title-optimizer](https://vinkius.com/ai-agent-connect/xiaohongshu-red-title-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Xiaohongshu (RED) Title Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `xiaohongshu-red-title-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Xiaohongshu (RED) Title Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "xiaohongshu-red-title-optimizer": {
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
